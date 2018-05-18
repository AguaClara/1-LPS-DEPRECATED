# 1 LPS Plant Testing
### Manual
#### Sung Min Kim, Sidney Lok, Erica Marroquin
#### May 18th, 2018


## Introduction
The goal of the 1 Liter per Second (1 LPS) Plant Testing team this semester is to complete the fabrication of the current 1 LPS plant. If time permits, the team also has plans to test the performance of the plant. In Fall 2016, the 1 LPS plant was developed based on pre-existing AguaClara technology to bring sustainable water treatment to small communities of about 300 people.

The team's mission is to create inexpensive water plants that treat at a flow rate of 1 liter per second for small towns and villages that do not have the means to finance surface water treatment due to upfront materials and construction costs.


Currently, the 1 LPS plant consists of an entrance tank, flocculator and sedimentation tank. The performance testing will be done using clay and coagulant to mimic real-world conditions, following traditional AguaClara concentrations. In addition to plant testing, the team has been fixing the Enclosed Stacked Rapid Sand (EStaRS) filter in order to observe differences in turbidity and to complete the full water treatment train (flocculation, sedimentation and filtration). However, for now, the plant is being run without the EStaRS as the filter itself has not been performance tested. While the EStaRS has been extensively tested and in use in India, the EStaRS in the DeFrees Lab was built in Spring and Summer 2017 (refer below to EStaRS Testing) specifically to be modular to the 1 LPS plant. Due to scaling dynamics, this current EStaRS needs to be tested but had only been fabricated and minimally water tested.


Here is the picture of the whole plant connected with the EStaRS, shown below in Figure 1.

![Entire 1 LPS plant connected to the EStaRS Filter](https://github.com/AguaClara/1-LPS/blob/master/Images/WholePlant.jpeg?raw=true)



## Chemical Dose Controller (CDC)
### Lever Arm Perforation
One of the first tasks the team had to complete was securing the lever arm onto the side of the entrance tank. The lever arm is a piece of equipment attached to the side of the entrance tank that allows plant operators to control the dose of the coagulant going into the influent water. As pictured in Figure 2, the lever arm consists of a slider on the lever arm that is the moving component controlling the chemical dosage and a metal bar at the back that fits into the hole at the side of the entrance tank pictured in Figure 3.


![Pictured is the lever arm before modification. Note that there is no visible way of securing the lever arm in place after sliding the metal bar into the hole at the side of the entrance tank in Figure 3 (circled in red).](https://github.com/AguaClara/1-LPS/blob/master/Images/1.jpg?raw=true)


At the beginning of the semester, the lever arm and entrance tank were still separate pieces as shown in Figures 2 and 3. At this point, the lever arm could slide into the hole in Figure 3 made on the attachment at the side of the entrance tank, but there was no way to ensure that the lever arm would not slide out of the hole.

![There is a hole (circled in red) in the PVC bar attachment at the side of the entrance tank. This is where the lever arm slides in.](https://github.com/AguaClara/1-LPS/blob/master/Images/2.jpg?raw=true)


The team determined that a perforation should be made in the metal bar of the lever arm so that a pin could be placed inside of it and act as a stopper as illustrated in Figure 4.

![A top down schematic of how the modified lever arm fits into the entrance tank. There was a perforation made in the metal bar of the lever arm in order for a pin to fit inside and act as a stopper. After being slid into the hole shown in Figure 2, a pin was inserted into the perforation to secure the lever arm onto the entrance tank.](https://github.com/AguaClara/1-LPS/blob/master/Images/Lever%20Arm.png?raw=true)


The team first found a piece to act as a pin and determined the size of it. The size of the piece was unimportant as long as its diameter was smaller than that of the metal bar for the lever arm. The lever arm was perforated according to the size of the pin using a mill as shown in Figure 5. The pin fit snugly into the perforation as shown in Figure 6.

![A mill machine in the Machine Shop was used to perforate the metal bar. It was important that the piece was brought to the shop to perforate as a safety precaution because the team did not have experience working with drilling into metal.](https://github.com/AguaClara/1-LPS/blob/master/Images/22.JPG?raw=true)

![Sung Min held up the finished perforation and pin design. The pin fit snugly into the perforation because the team had measured the pin beforehand and determined the size of it.](https://github.com/AguaClara/1-LPS/blob/master/Images/33.JPG?raw=true)


### CDC Placement
During Spring 2017, AguaClara fabricated a new design of the chemical dose controller (CDC). The past research report can be found [here](https://www.overleaf.com/read/zfcbvtrykhwc#/28982452/). The CDC system was designed to maintain a constant chemical dose to the treatment process as the plant flow rate and influent turbidity change. The main difference from the old design and the new is that slimmer PVC pipes were used in the new design. The current CDC system is incomplete for chlorination but is complete for coagulation, which the team is testing this semester.

The CDC works in conjunction with the lever arm on the side of the entrance tank. The team has to ensure that the height of the lever arm when horizontal is the same height as the coagulant level of the CDC when the float values are submerged. The height of the lever arm needs to be the height of the coagulant level of the CDC when the float values are submerged to keep a constant head loss. The CDC apparatus' height can be adjusted by unscrewing the screws in the wooden plate.

Running the 1 LPS plant first with water was the team's priority. In order to do so, the team has not properly made sure that the heights were equal on the pole since adjustment was unnecessary for the water run. The team plans to match the heights as shown in Figure 7 after assembling all the materials needed for the coagulant run.

![Pictured is the Chemical Dose Controller (CDC) in relation to the entrance tank and lever arm. The CDC will need to be shifted up in order to ensure that the height of the lever arm when horizontal is the same as the coagulant level of the CDC as described above.](https://github.com/AguaClara/1-LPS/blob/master/Images/3.JPG?raw=true)


### Dosing Tube Calculations
In order to get the proper flow rate of chemicals into the plant, the team needed to calculate the correct length and sizes for the dosing tubes. The yellow arrows in Figure 9, below, are pointing to the dosing tubes on the CDC apparatus. There are two types of dosing tubes that are two different diameters.

The first tube connects the constant head tank (CHT), which contains the chemical stock, to a tee fitting on the lever arm. The CHT is a type of flow controller that maintains a constant chemical level in its tank. The level is maintained by a float valve connected to a larger stock tank above. Its operation is governed by the Hagen-Poiseuille equation:

$$ Q = \frac{h_f g \pi D^4}{128 \nu L} $$

where $Q$ is flow rate, $h_f$ is the head difference between the water level in the constant head tank and the slider on the lever, $D$ is the diameter of the tubing, $\nu$ is the kinematic viscosity, and $L$ is the length of the tubing.


The head difference can be changed by moving the slider on the lever arm. A change in head, $h_f$, causes an increase in flow rate, $Q$, out of the CHT, therefore increasing the coagulant dosage to the plant. For a deeper explanation of this concept, more information can be found in the [CEE 4540 notes](https://confluence.cornell.edu/display/cee4540/Syllabus) by Monroe Weber-Shirk.

An image of the CHT is shown below, in Figure 8. The CHT is the small container in the upper left corner of each figure.

![Constant head tank (CHT) shown with the rest of the chemical dosing controller. The difference in head can be shown with changing $H$. Images courtesy of Monroe Weber-Shirk, found [here](https://confluence.cornell.edu/display/cee4540/Syllabus)](https://github.com/AguaClara/1-LPS/blob/master/Images/CHT_Schem.png?raw=true)



The second type of dosing tube connects the tee fitting to the influent water coming into the plant. For more information on how the CDC works, the most current research report can be found [here](https://www.overleaf.com/read/zfcbvtrykhwc#/28982452/).

![A schematic of the CDC system, showing the entrance tank, lever arm, constant head tank, and the dosing tubes. The dosing tubes are highlighted by the yellow arrows.](https://github.com/AguaClara/1-LPS/blob/master/Images/4.png?raw=true)

The relationship between the flow of the plant and the coagulant dosage needs to be linear in order to be effective. This means that the relationship between flow rate and head loss needs to be linear. The actual head in the dose controller is due to both major and minor losses. In order for the relationship to remain linear, major losses need to dominate, as shown below in Figure 10.

![Flow rate versus head loss while varying types of head loss. Images courtesy of Monroe Weber-Shirk, found [here](https://confluence.cornell.edu/display/cee4540/Syllabus).](https://github.com/AguaClara/1-LPS/blob/master/Images/LinearRelationshipCDC.png?raw=true)


Head loss due to friction, $h_f$, also known as major losses, is

$$ h_f = \frac{128 \nu Q L}{g \pi D^4} $$

Head loss due to expansions, $h_e$, also known as minor losses, is

$$ h_e = \frac{8 Q^2}{g (\pi)^2 D^4} \sum K_e $$

The equation for the actual head loss is shown below, which is a combination of both major and minor losses. This is shown as the blue line in figure 9.

$$ h_L (Q) = (\frac{128 \nu L}{g \pi D^4} + \frac{8Q}{g (\pi)^2 D^4} \sum K_e) Q $$

By minimizing the amount of expansions or contractions in the dose controller tubing, as well as creating more friction by decreasing diameter, $D$, major losses will dominate.

Therefore, the tube that connects the CHT to the tee fitting on the lever arm needs to be a very small diameter. Major losses will then dominate within the tube over the calculated length, leading to the proper flow rate out of the tube. The tube that connects the tee fitting to the influent water needs to be big enough that surface tension will not dominate within the tube, and water and air can flow freely through the tube.

The calculations for the length and diameter of these tubes were done using code written by the [AguaClara Infrastructure Design Engine (AIDE) team](https://github.com/AguaClara/aide_design). The code can be found below in the section "Dosing Tube Calculations" under "Python Code."

The length of the CDC tube connecting the CHT to the tee fitting will be 0.4811 meters long and $\frac{1}{16}$ inches in diameter. The diameter of the tube connecting the tee fitting to the influent water will be $\frac{1}{4}$ inches.

## CDC Plant Integration
The CDC needed to be connected and integrated into the rest of the plant as shown previously in Figure 7. The chemicals would flow from the CHT to the slider on the lever arm and through the dosing tube to the plant. As determined in the section "Dosing Tube Calculations", the size of the dosing tube connecting the CHT to the lever arm needed to be $\frac{1}{16}$ inches in diameter and the dosing tube $\frac{1}{4}$ inches. A plastic tee was acquired to connect the two dosing tubes to the lever arm as shown in Figure 11. The tee acquired was a $\frac{1}{4}$ inch female connector.

![The tee connector was attached to the slider on the lever arm with a flat-headed screw.](https://github.com/AguaClara/1-LPS/blob/master/Images/T.JPG?raw=true)


In order to attach the tee connector onto the slider of the lever arm, a hole was drilled into the side of the piece to Insert a flat-headed screw through it. The dosing tubes had barbed fittings to make water-tight connections to the tee connector. The larger diameter dosing tube connected right above the rapid mix of the first leg of the flocculator. The team drilled a $\frac{1}{4}$ inch hole into the side of the first leg of the flocculator at an arbitrary height above the rapid mix and tapped it as shown in Figure 12.

![The barbed fitting connecting the dosing tube to the first leg of the flocculator is circled in red.](https://github.com/AguaClara/1-LPS/blob/master/Images/5.jpg?raw=true)


## 1 LPS Plant Water Run
The team's main focus was to run water completely through the 1 LPS plant. Depending on the progress of EStaRS testing, the team would like to run the plant with the filter to observe changes in the turbidity results.


The plant has been fully connected to the water source and the drain as shown in Figure 13. Once the DeFrees Lab was cleared, the team water tested the plant and welded two minor leaks at the inlet and outlet. The plant is ready to go through its coagulant run.

![Pictured is the tube connection between the top of the sedimentation tank to the drain. It is connected by a combination of pipes and elbows, reinforced tubing from the DeFrees laboratory, and two male couplings.](https://github.com/AguaClara/1-LPS/blob/master/Images/44.JPG?raw=true)


## EStaRS Testing
The Enclosed Stacked Rapid Sand (EstaRS) Filter is an adaptation of AguaClara's Stacked Rapid Sand (StaRS) Filter. These filters make the process of sand filtration much more effective in terms of filtration time and cost. Sand filters use a large area, and as flow rate through the filter increases, so does the necessary area of the filter. By stacking smaller layers of sand in between inlets and outlets, AguaClara was able the decrease the overall area of a sand filter and the residence time of the filter. The EStaRS Filter can be used by itself as a stand alone filter or at the end of a treatment train. In Figure 14, below, the process of forward filtration is shown.

![EStaRS Filter in forward filtration.](https://github.com/AguaClara/1-LPS/blob/master/Images/EStaRSFilter.png?raw=true)

The current EStaRS filter was built in Spring 2017 with the purpose of accompanying the 1 LPS plant. The design that is now currently used is based off of a successful iteration of a previous EStaRS Filter built in 2013, then known as the Low Flow Stacked Rapid Sand Filter (LFSRSF).

The information used by the 1 LPS team to assemble the filter was found in the EStaRS Spring 2017 research report, found [here](https://www.overleaf.com/8262051cfnxfzxkmnsp#/29239180/). A photo of the filter is shown below, in Figure 15.

![EStaRS Filter in the lab.](https://github.com/AguaClara/1-LPS/blob/master/Images/irlEStaRSFilter.jpeg?raw=true)


Eventually, a filter becomes too clogged to effectively remove particles from the water flowing through it. At this point, the filter needs to be backwashed; the sand bed is fluidized by increasing the up-flow velocity of the filter. In the EStaRS Filter, this is done by pulling all of the influent water into the largest, bottom inlet. The water is pulled because of a pressure difference that occurs once the backwash siphon is opened. Once the sand bed is fluidized, the particles clogging the filter are dislodged and float to the top of the filter to be discharged as waste.


An increase in up-flow velocity also increases the amount of force that inlet and outlet manifolds have to withstand. There was concern that in this new iteration of the EStaRS Filter, the upward force during backwash would cause the manifolds to snap or break. In order to figure out if this was a cause for concern, the team conducted a force analysis on the manifolds.


The code for this analysis can be found below in the section "EStaRS Filter Force Analysis" under "Python Code."

The total force that backwash will exert on the manifolds is 679.8 newtons. Assuming that this force will be equally distributed over each of the seven manifolds, the force exerted on each manifold is 97.11 newtons. When converted to pound-force, this is approximately 21.83 lbf. Dividing that by the force due to gravity, the force exerted on each manifold is about 10 kg.

The team removed the top inlet manifold to test if 10 kg would cause it to break. Since 10 kg is equal to 10 L of water, the team applied a bucket of 10 L to the middle of the manifold. It did not break. Therefore, the team assumed that the filter manifolds can withstand the force of backwash.

The EStaRS filter was also tested for water-tightness. There were leaks on welds, which could have been sealed by re-welding, glue, or epoxy. The team decided to re-weld the leaks.

During re-welding, the filter was put on a small cart for mobility, as it needed to be separate from the 1 LPS plant while each apparatus was being fixed, respectively. Once the leaks were sealed, the team removed the filter from the cart and placed it where it can be connected to the 1 LPS plant. The team filled the filter with sand. It is necessary to fill the filter with sand to just cover the top-most inlet. Any more sand than that would be unnecessary, as the inlets and outlet layers are only located in the bottom half of the filter.

Since there was no easy was to lift or move the filter, the bottom cap moved during placement. This then caused the EStaRS Filter to leak from the bottom. The team was not able to fix this issue despite many attempts.

This leads to the necessity of a filter redesign. The EStaRS Filter needs mobility as well as a guaranteed seal for the top and bottom caps. Working with the machine shop, the team designed a new way of sealing the filter. This is shown below in Figure 16.

![A schematic showing a proposed new design for the EStaRS Filter.](https://github.com/AguaClara/1-LPS/blob/master/Images/NewProposedFilter.png?raw=true)


The eye hooks give the ability to move the filter using a small crane. The flanges can be removed if the team needs to clean out the filter, but still provides a water tight seal with an o-ring on the inside. For additional mobility, the team spoke about potentially adding wheels to the bottom PVC sheet.

In the future, the team needs measure the filter performance by running tests with clay and coagulant. Since this iteration of the EStaRS filter has never been tested, the team will test to see if this filter performs as well as the previous EStaRS filter.


## ProCoDa Setup
The team was able to create and setup a basic ProCoDa file for future test runs of the 1 LPS plant. Pictured in Figures 17, 18, and 19 are screen captures of the team's ProCoDa test file. The 1 LPS plant is set up so that there is little room for automation. The valves used on the plant are not automatic because they are large valves that would be expensive to acquire automated versions of. Therefore, the team's ProCoDa file is simple. The file is set up to automate the clay pump and turbidity pump. The clay pump will be used to pump clay to the entrance tank. The turbidity pump will be used to take influent and effluent from the plant to perform perfomance test analysis.

![The ProCoDa setpoints and variables used for the test file. The variables are Turbidity Flow Rate, Clay Stock Flow Rate, Tubing ID, Turbidity Pump RPM, Turbidity Heads, and Clay Pump RPM. Turbidity Flow Rate and Clay Stock Flow Rate declared the desired flow rates set by the user. The Tubing ID declared the size of the pump tubing used (in this case it was size 19). The Clay Stock RPM and Turbidity RPM were variable set points that used calculations stored in the AguaClara drive to determine RPM from the inputs, as shown in the figure. The Turbidity Heads was set to two because there was a pump head for influent and for effluent.](https://github.com/AguaClara/1-LPS/blob/master/Images/6.PNG?raw=true)

![The ProCoDa rules and outputs list which shows the two pumps being used for clay and turbidity. In the 1 LPS test state, the clay and turbidity pumps will be turned on at the RPM detailed on the interface.](https://github.com/AguaClara/1-LPS/blob/master/Images/7.PNG?raw=true)

![The ProCoDa interface for test runs.](https://github.com/AguaClara/1-LPS/blob/master/Images/procoda3.PNG?raw=true)

## Python Code

### Dosing Tube Calculations

#### Variables
$g$: gravity

${h_L}$: head loss

$D$: diameter of pipe

$\nu$: kinematic viscosity of a fluid

$Q$: flow rate

$K_e$: minor loss coefficient

#### Equations
The equation for the length of a dosing tube is:

$$L = (\frac{g {h_L}_{,Max} \pi D^4}{128 \nu Q_{Max}} - \frac{Q_{Max}}{16 \pi \nu} \sum K_e)$$

where ${h_L}_{,Max}$ is the maximum head loss and $Q_{Max}$ is the maximum flow rate in the tube.

#### Code
```python
#dosing tube calculations
from aide_design.play import*
import aide_design.cdc_functions as cdc

help(cdc.len_cdc_tube)

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

### EStaRS Filter Force Analysis

The purpose of this analysis is to see if the manifolds inside the EStaRS Filter can withstand the force of backwash without breaking. This is a concern because, in Honduras, plant operators noticed in the early iterations of the filter, that the manifolds would snap and disassemble during backwash. This was because the manifolds were not held into place within the filter body.

#### Variables
`EStaRS_height`: Distance from the ground to the top of the entrance tank.

`sand_height`: Height of sand in filter body, from floor to top of first sand bed.

`total_head_available`: Amount of head loss available to power backwash.

`pressure_head`: Total head converted to a pressure.

`force_of_backwash`: Force that will be exerted on the manifold pipes during backwash. It is assumed that this force will be equally distributed over each of the seven manifolds.

$g$: gravity

#### Equations

The equation for finding pressure from head is:

$$ P_h = \rho g h$$

where $h$ is the total head available, and $\rho$ is the density of water.

The equation for finding force from pressure is:

$$ F = P A $$

where $A$ is the area of a cross-section of the filter.

#### Code
```python
rho_water = 1*(u.g/u.cm**3) #density of water
g = pc.gravity #gravity
EStaRS_height = 185*(u.cm) #measured
EStaRS_diameter = 12*(u.inch) #known
EStaRS_area = pc.area_circle(EStaRS_diameter)
sand_height = 6 * 15*(u.cm) #six sand beds each at a height of 15 # cm

total_head_available = EStaRS_height - sand_height

pressure_head = rho_water*g*total_head_available

force_of_backwash = pressure_head*EStaRS_area

print('The total force that backwash will exert on the manifolds is
      ,(force_of_backwash.to(u.N)),'. The force exerted on each manifold is
      ,(force_of_backwash.to(u.N))/7,'.')
```

## Materials List
- EStaRS
  - [Top Plate Air Flow Valve](https://www.mcmaster.com/#catalog/4950K55)
- Plant Body
  - [Flocculator Piping](https://www.mcmaster.com/#catalog/48925K97)
  - [Wood Pole Washers](https://www.mcmaster.com/#catalog/92141A030)
  - [Dosing Tube Barbed Fitting](https://www.mcmaster.com/#catalog/5121K421)
  - [Dosing Tube](https://www.mcmaster.com/#catalog/6516T11)
  - [Lever Arm Slider Tee Connector](https://www.mcmaster.com/#catalog/4596K321)

## Contact Information
The contact information for the Spring 2018 1 LPS Plant Testing Team is as follows:
- Sung Min Kim, EnvE '19
  - Sub-team Lead
  - sk2795
- Sidney Lok, EnvE '19
  - sgl38
- Erica Marroquin, EnvE '18
  - em628
