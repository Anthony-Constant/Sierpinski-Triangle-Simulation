# Sierpinski Triangle Simulation

## What is it?

Sierpinski Triangle is a simulation that shows an initial green cell with a nucleus (a small white circle) that in the next generation produces two similar daughter cells, one at its left, the other at its right. The daughter cells repeat this for another 20 or so generations, leading in the end to the structure of a Sierpinski triangle.

## How it works

The simulation starts with an initial patch in the middle of the top-row of the canvas, which has been colored green by a single turtle, who itself was created in a "tosetup" procedure. Besides marking the initial patch, the parent turtle also replicates by hatching a "child" on that patch. The hatched child itself also leaves a "copy" of itself behind (a grand-child, so to speak).

The "to go" procedure asks the "child" to run a "to move" procedure. The "to move" instructs the child to go to a patch below and at the left of the original cell, followed by going to a patch below and at the right of the original cell. Before it makes that second move, it calls the "tomark-and-breed" procedure. It does so again after completing the second move.

The "to go" runs for a defined number of generations. To do this, a counter called "generationstep" has been set at 1 in the setup and is increased by 1 every time the simulation goes through a next round of "to go". The "to go" stops after it has been checked if generationstep = #generations. Note: that each cell contains just one "copy". This means that the parent turtle and the "children", but not the "copies", must have "died".

## How to use it

- First, click the "setup" button to set up the initial agent.
- Then, click the "go" button to run the program.
- Move the #generations slider to specify the number of generations outputted.
- Note: The "to go" stops after it has been checked if generationstep = #generations.

## Things to try

- Experiment with changing the number of generations and observe the output.

## License

This project is licensed under the [MIT License](https://opensource.org/licenses/MIT).

## Acknowledgements

This script was developed by [Anthony Constant](https://anthonyconstant.co.uk/).
