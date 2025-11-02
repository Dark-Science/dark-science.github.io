# Initiation Trial 0

This trial, serving as an excellent beginning program for learning GNU Octave, was intended to obtain a quick first glimpse of how the trajectory would appear. The update loop for the program resulted in producing one graph and the spatiotemporal coordinates for every captured position which would occur with each regular time increment or "tick". Initializing parameters and constants at the beginning of the program, which is good coding practice anyway, makes the setup for reiteration trials 0A, 0B, and 0C effortless while trial 0 can be thought of as the task for ensuring the program is written in a usable manner, though such items are not needed on the WBS.

## Program Initialization

GNU Octave, like many other languages, requires variables (and constants) to at least be assigned 'dummy values' before they can be employed in many functions, even ones that are needed to determine its proper initial value in the first place. For writing this simple program, only introductory kinematics and object properties are needed for simulation. Kinematic differential equations solved by hand can be done through various mathematical means and compared with the results of computer programs, like the one written in GNU Octave for this purpose. Programming the mathematics easily takes advantage of automating loops, plots, and if statements when doing so on paper would consume dozens of pages and even more so in hours and unnecessary frustration from eraser marks and penmanship.

<div class="joplin-table-wrapper"><table border="1" style="border-collapse: collapse; width: 100%;" class="jop-noMdConv"><colgroup class="jop-noMdConv"><col style="width: 25%;" class="jop-noMdConv"><col style="width: 25%;" class="jop-noMdConv"><col style="width: 25%;" class="jop-noMdConv"><col style="width: 25%;" class="jop-noMdConv"></colgroup><thead class="jop-noMdConv"><tr class="jop-noMdConv"><th scope="col" class="jop-noMdConv"><h3 class="jop-noMdConv">Initial Dimensions</h3></th><th scope="col" class="jop-noMdConv">Initial Kinematics</th><th scope="col" class="jop-noMdConv">Object Properties</th><th scope="col" class="jop-noMdConv">Program Properties</th></tr></thead><tbody class="jop-noMdConv"><tr class="jop-noMdConv"><td class="jop-noMdConv"><ul class="jop-noMdConv"><li class="jop-noMdConv">x<sub class="jop-noMdConv">0</sub> = 0 (m)</li><li class="jop-noMdConv">y<sub class="jop-noMdConv">0</sub> = 0 (m)</li><li class="jop-noMdConv">t = 0 (s)</li><li class="jop-noMdConv">θ<sub class="jop-noMdConv">0</sub> = 85 (deg)</li><li class="jop-noMdConv">θ = θ<sub class="jop-noMdConv">0</sub></li></ul></td><td class="jop-noMdConv"><ul class="jop-noMdConv"><li class="jop-noMdConv">v<sub class="jop-noMdConv">0</sub> = 100 (m/s)</li></ul></td><td class="jop-noMdConv"><ul class="jop-noMdConv"><li class="jop-noMdConv">m = 1 (kg)</li><li class="jop-noMdConv">g = 9.81 (m/s<sup class="jop-noMdConv">2</sup>)</li></ul></td><td class="jop-noMdConv"><ul class="jop-noMdConv"><li class="jop-noMdConv">dt = 0.8</li><li class="jop-noMdConv">flag = 8/dt</li></ul></td></tr></tbody></table></div>

## Kinematic Formulas

The below vector formulas define the trajectory for the given object:

1.  $\vec{a} = 0\hat{i} - g\hat{j}$
2.  $\vec{v} = (v_0\cos{\theta_0})\hat{i} - (v_0\sin{\theta_0}-gt)\hat{j}$
3.  $\vec{r} = x_0\hat{i} - y_0\hat{j}$

## Graph Plotting per Loop

The program functions by plotting the position (x, y) for each time increment (dt), and updating t, r, and v using the formulas below:

1.  $t = t + dt$
2.  $\vec{r} = (x + \dot{x} dt)\hat{i} + (y + \dot{y} dt)\hat{j}$
3.  $\vec{v} = \dot{x}\hat{i} + (\dot{y} - gt)\hat{j}$

# Results: Trials A-C

<div class="joplin-table-wrapper"><table class="jop-noMdConv"><thead class="jop-noMdConv"><tr class="jop-noMdConv"><th class="jop-noMdConv"><h3 class="jop-noMdConv"><strong class="jop-noMdConv">Trial 0A</strong></h3></th><th class="jop-noMdConv"><img src="../../_resources/935bf7e4227669708b3703c2abdb0bf1.png" alt="935bf7e4227669708b3703c2abdb0bf1.png" class="jop-noMdConv"></th></tr></thead><tbody class="jop-noMdConv"><tr class="jop-noMdConv"><td class="jop-noMdConv"><h3 class="jop-noMdConv"><strong class="jop-noMdConv"><strong class="jop-noMdConv">Trial 0B</strong></strong></h3></td><td class="jop-noMdConv"><img src="../../_resources/fe63da43b214846d5ab2e42d6ad04b5d.png" alt="fe63da43b214846d5ab2e42d6ad04b5d.png" class="jop-noMdConv"></td></tr><tr class="jop-noMdConv"><td class="jop-noMdConv"><h3 class="jop-noMdConv"><strong class="jop-noMdConv"><strong class="jop-noMdConv">Trial 0C</strong></strong></h3></td><td class="jop-noMdConv"><img src="../../_resources/6d9f46b743bcfd33c330a622cab24bc5.png" alt="6d9f46b743bcfd33c330a622cab24bc5.png" class="jop-noMdConv"></td></tr><tr class="jop-noMdConv"><td class="jop-noMdConv"><h3 class="jop-noMdConv"><strong class="jop-noMdConv"><strong class="jop-noMdConv"><ins class="jop-noMdConv">Trial 0 Plot</ins><br class="jop-noMdConv"></strong></strong></h3></td><td class="jop-noMdConv"><img src="../../_resources/6e60213a8ecc41b8293b91b80edfb95b.png" alt="6e60213a8ecc41b8293b91b80edfb95b.png" class="jop-noMdConv"></td></tr></tbody></table></div>

## Testing Kinematics
