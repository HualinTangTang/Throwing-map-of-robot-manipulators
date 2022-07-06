# Throwing-map-of-robot-manipulators

In manufacturing, objects are typically transported by robots via pick and place.
Especially when using serial robots, the speed for this task is limited. Significantly
higher speeds and ranges can be achieved if the robot throws objects. In this thesis,
the so-called throwing map, i.e., the space where the robot can throw objects, is
introduced and elaborated. The throwing map has multiple applications:
a) Path planning of mobile manipulators
For mobile manipulators moving between workstations, the throwing map can
be used to optimize paths. Question: What is the shortest path to be followed
by a robot that throws objects into boxes?
b) Optimizing robot kinematics for throwing.
How can kinematics (e.g., link lengths) be optimized to allow a robot to throw
as far as possible?
c) Comparison of different types of robots in terms of throwing distance
Typically, fixed-base serial manipulators are used in industry. Higher throwing
distances can be achieved by adding a mobile base or by using a robot with
intrinsically elastic joints. In this regard, it is possible to compare the
performance of different robots.
d) Computation and execution of throwing trajectories
One could compute (optimal) throwing trajectories and execute them on the
robot. It would be possible to compute trajectories using an existing planner.
One could then use the resulting trajectories to determine the throwing map,
i.e., determine the throwing map for the robot in combination with a concrete
planner.
e) Throwing distance for different throwing modes (underhand vs. overhand
throwing).
Work plan proposal
a) Definition throwing map
a. What is the throwing map?
b. Difference between throwing map for point object and real objects (map
becomes larger, use sphere as approximation, for example)
c. How can it be determined?
i. Via reachability map
ii. By throwing trajectory with maximum range
d. How can it be calculated/represented in a simplified way? (e.g., 2D vs.
3D)
b) Computation throwing map for Franka Emika robot
a. Calculation and visualization of velocity polytope (results already
available).
b. Determination of the reachability map (results already available)
c. Determine the Cartesian velocity for each reachable pose (polytope,
results already available)
d. For each reachable pose, determine the throwing trajectory in all
directions (45 degree angle)
e. Determine the envelope of all throwing trajectories (alternative:
trajectory with maximum range)
f. Visualize result
g. Repeat and visualize calculation for restricted work space (e.g., 0-40 cm
above table surface)
h. Extension to mobile manipulator and robot with elastic joints (results
available)
