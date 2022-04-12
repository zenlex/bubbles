# Bubbles!
![Threejs](https://img.shields.io/badge/threejs-black?style=for-the-badge&logo=three.js&logoColor=white)
### A Generative 3D Bubble Nebula

Developed as part of a creative coding meetup at Recurse Center
*Initial concept developed in collaboration with Ingrid Chung and Kawayan de Guzman.*

## Demo
Currently deployed on replit [here](https://bubbles.zenlex.repl.co/)

### Install
Download the html file (the JavaScript is all embedded) and the three.js library file to the same folder. 
Launch the html file in a browser. 

### Usage
- Scroll to zoom in/out
- Click and drag to rotate camera

The bubbles will build up over time. 

Bubbles spawn with randomized colors, positions, and growth rates
Each time a bubble doubles in size it 'pops' and spawns two new random children

To limit the exponential growth consequences, there is a constant limit on actively growing bubbles `MAX_BUBBLES`
You may adjust the value of `MAX_BUBBLES` based on your system hardware (default = 500). 
Each time this cap is exceeded, half of the existing active bubbles get frozen allowing density to grow over time

### License
[GNU General Public License](https://opensource.org/licenses/GPL-3.0)
