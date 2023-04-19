<h1>Sierpinski Triangle Simulation</h1>
<h2>What is it?</h2>
<p>Sierpinski Triangle is a simulation that shows an initial green cell with a nucleus (a small white circle) that in the next generation produces two similar daughter cells, one at its left, the other at its right. The daughter cells repeat this for another 20 or so generations, leading in the end to the structure of a Sierpinski triangle.</p>
<h2>How it works</h2>
<p>The simulation starts with an initial patch in the middle of the top-row of the canvas, which has been colored green by a single turtle, who itself was created in a "tosetup" procedure. Besides marking the initial patch, the parent turtle also replicates by hatching a "child" on that patch. The hatched child itself also leaves a "copy" of itself behind (a grand-child, so to speak).</p>
<p>The "to go" procedure asks the "child" to run a "to move" procedure. The "to move" instructs the child to go to a patch below and at the left of the original cell, followed by going to a patch below and at the right of the original cell. Before it makes that second move, it calls the "tomark-and-breed" procedure. It does so again after completing the second move.</p>
<p>The "to go" runs for a defined number of generations. To do this, a counter called "generationstep" has been set at 1 in the setup and is increased by 1 every time the simulation goes through a next round of "to go". The "to go" stops after it has been checked if generationstep = #generations. Note: that each cell contains just one "copy". This means that the parent turtle and the "children", but not the "copies", must have "died".</p>
<h2>How to use it</h2>
<ul>
  <li>First, click the "setup" button to set up the initial agent.</li>
  <li>Then, click the "go" button to run the program.</li>
  <li>Move the #generations slider to specify the number of generations outputted.</li>
  <li>Note: The "to go" stops after it has been checked if generationstep = #generations.</li>
</ul>
<h2>Things to try</h2>
<ul>
  <li>Experiment with changing the number of generations and observe the output.</li>
</ul>
<h2>Credits</h2>
<p>This script was created by Anthony Constant (AC). If you have any questions or suggestions, you can contact him at https://anthonyconstant.co.uk/</p>
<h2>License</h2>
<p>This script is released under the MIT License. See the LICENSE file for more details.</p>
