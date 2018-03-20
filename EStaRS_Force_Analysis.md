```python
from aide_design.play import*
```

### Force Analysis for EStaRS Filter Manifolds
The purpose of this analysis is to see if the manifolds inside the EStaRS Filter can withstand the force of backwash without breaking. This is a concern because, in Honduras, plant operators noticed in the early iterations of the filter, that the manifolds would snap and disassemble during backwash. This was because the manifolds were not held into place within the filter body.

### Variables

`EStaRS_height`: Distance from the ground to the top of the entrance tank.

`sand_height`: Height of sand in filter body, from floor to top of first sand bed.

`total_head_available`: Amount of head loss available to power backwash.

`pressure_head`: Total head converted to a pressure.

`force_of_backwash`: Force that will be exerted on the manifold pipes during backwash. It is assumed that this force will be equally distributed over each of the seven manifolds.

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

print('The total force that backwash will exert on the manifolds is ',force_of_backwash.to(u.N),'. The force exerted on each manifold is ',(force_of_backwash.to(u.N))/7,'.')
```
The total force that backwash will exert on the manifolds is 679.8 newtons. Assuming that this force will be equally distributed over each of the seven manifolds, the force exerted on each manifold is 97.11 newtons. This is the force that each manifold will have to withstand.

Written by Erica Marroquin (em628).
