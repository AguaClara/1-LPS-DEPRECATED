##Dosing Tube Calculations for 1LPS Plant
###Spring 2018
####Erica Marroquin (em628), Sidney Lok (sgl38), Sung Min Kim (sk2795) [STL]

```python
from aide_design.play import*
import aide_design.cdc_functions as cdc

help(cdc.len_cdc_tube)
```

Already known constants needed according to the `len_cdc_tube` function:
```python
FlowPlant = 1*(u.L/u.s)
  #assuming the plant flows at maximum flow rate
DiamTubeAvail = np.array(np.arange(1/16,6/16,1/16))*u.inch
  #diameter of tubing available in lab
  #this indicates an array of tube sizings between 1/16" and 6/16"
  #with a 1/16" interval.
HeadlossCDC = 10*u.cm
  #set by the maximum height of water in the entrance tank
temp = 20*u.degC
  #room temperature
en_chem = 1
  #in cdc_functions, en_chem = 1 designates using PaCl
KMinor = 4
  #comes from Monroe; from two barbed fittings at the beginning
  #and end of the dosing tube. minor losses from CDC apparatus are
  #negligible because they are very small compared to the
  #losses from the CDC tubing.
ConcDoseMax = 20*(u.mg/u.L)
  #set by the maximum dose possible by the lever arm
ConcStock = 70.9*(u.gram/u.L)
  #concentration of stock in the lab
LenCDCTubeMax = 6*u.m
  #any longer than this would be ridiculous
```

Thus, the length of the dosing tube will be:
```python
DosingTubeLength = cdc.len_cdc_tube(FlowPlant, ConcDoseMax, ConcStock,
  DiamTubeAvail, HeadlossCDC, LenCDCTubeMax, temp, en_chem, KMinor)
print('The length of the CDC tube is ',DosingTubeLength,'.')

DTube = cdc.diam_cdc_tube(FlowPlant, ConcDoseMax, ConcStock, DiamTubeAvail,
  HeadlossCDC, LenCDCTubeMax, temp, en_chem, KMinor)
print('The diameter of the CDC tube is ',DTube.to(u.inch),'.')

NTube = cdc.n_cdc_tube(FlowPlant, ConcDoseMax, ConcStock,
  DiamTubeAvail, HeadlossCDC, LenCDCTubeMax, temp, en_chem, KMinor)
print('The number of CDC tubes is ',NTube,'.')
```

Something is wrong with this calculation (as of 2/23/18, 10am). I think this is due to the low flow rate of the plant. Will confirm with Monroe to figure out the issue. -Erica

Issue was fixed (2/23/18, 12pm). Concentration of stock was originally incorrect. -Erica
