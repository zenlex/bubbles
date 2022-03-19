# Bubbles!
### A Generative 3D Bubble Nebula in ThreeJS

Developed as part of a creative coding meetup at Recurse Center

*Initial concept developed in collaboration with Ingrid Chung and Kawayan de Guzman.*

## Demo
Currently deployed on replit [here](https://bubbles.zenlex.repl.co/)


## Setup
Script is self contained within `index.html`.
The core Three.JS library file is included locally as well. No other setup required. 


### The Algorithm
Bubbles spawn with randomized colors, positions, and growth rates
Each time a bubble doubles in size it 'pops' and spawns two new random children

To limit the exponential growth consequences, there is a constant cap of actively growing bubbles
Each time this cap is exceeded, half of the existing active bubbles get frozen in time allowing density to grow over time

While actively monitored and manipulated bubbles are capped at a constant max, 
be aware that as density grows GPU demand will increase as there are translucency and shadow calculations happening on the bubbles
