### GPU-Flock-Simulation
Untiy3D Implementation of flock simulation, GPU Powered.

**Implementation Details:**

Computation happens on the GPU using _ComputeShaders_, then the buffer with data is set in another _SurfaceShader_ that calculates the view matrix for each boid -flock handled as a big mesh-, they're then rendered on the screen, thus eliminating the overhead of recieving the data from the GPU buffer to the CPU and drawing them again.

**How to Run:**

Start the sample scene ***Scenes/BasicFlocking*** and hit play.

Tweak the parameters of ***BasicFlockController*** to control the general behaviour of boids.

**Unity Version:**

- 2018.3.9f1

**ToDo Features:**

- [x] Add Predation Behaviour (_Some boids will act as a predator, seek to hunt other boids_)
- [x] Add Flee Behaviour (_Boids will run away from predators_)
- [x] Add different ranges for each behaviour.
- [x] Add Boid Specific Skinned Animation.
- [x] ~Add Collision Avoidance (_Boids will avoid collisions around the scene, __will probably be baked static colliders___)~ Collision Avoidance won't be feasible for the general purpose of the whole system!

**Inspired by:**

* [Shinao](https://github.com/Shinao).
* [Nature Of Code](https://natureofcode.com/).
* [Keijiro](https://github.com/keijiro).
