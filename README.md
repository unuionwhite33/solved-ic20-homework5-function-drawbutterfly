Download Link: https://assignmentchef.com/product/solved-ic20-homework5-function-drawbutterfly
<br>
<h1>Exercise 1</h1>

Write the <strong>function</strong> <strong>drawButterfly</strong> that:

<ul>

 <li>takes the value n for expressing the size N=2<sup>n</sup> of the Butterfly network – draw the Butterfly network</li>

</ul>

Write the <strong>function</strong> <strong>self-routing-Butterfly</strong> that:

<ul>

 <li>takes a permutation in input</li>

 <li>calculates the routing on the Butterfly using the self-routing algorithm – gives as <strong>output</strong>: o the matrix P of size N x 2n, where each column represents the element of the permutation, in particular <em>odd</em> columns represent the sequence <em>before</em> traversing nodes in a stage and <em>even</em> columns represent the sequence <em>after</em> traversing nodes in a stage. In the case a conflict occurs, the program stops after completing the computation for all the nodes in the current stage and writes the number of the first stage where the conflict occurs (assuming all inputs traverse the network in parallel)</li>

</ul>

o the matrix S of size (N/2) x n, representing the switch setting of the Butterfly, where 0 represents the state <em>straight</em>, 1 represents the state <em>cross</em>, and a value at your choice (any value different from 0 and

1, or NaN) for switches not set yet

Write the <strong>script</strong> that:

<ul>

 <li>takes the value n for expressing the size N=2<sup>n</sup> of the Butterfly network as a parameter</li>

 <li>chooses a random permutation of N elements</li>

 <li>calls the function <strong>self-routing-Butterfly</strong></li>

 <li>draws the picture of the Butterfly calling the function <strong>drawButterfly</strong> using different colors for straight and cross state of nodes (or drawing the node setting with lines inside the switch), and using the color gray for nodes of stages not traversed (or leaving the switch empty), furthermore, in case of conflict the nodes involved must be highlighted</li>

</ul>




<strong>Remark </strong>The following definition of the Butterfly stage and Butterfly network can be useful:

<em>An edge stage is a </em>Butterfly edge stage<em> of size l, l= 1, 2, ···, n−1, if any node, with (n−1)-bit binary label v, in the first node stage is connected to node v′ in the second stage if and only if v = v′ (straight edge) or v and v′ differ only in the l-th bit (cross edge). A </em>Butterfly<em> is a log N stage network consisting of an ordered sequence of Butterfly edge stages of increasing size from 1 to n−1. </em>




<h1>Exercise 2 – Interconnection Networks – CLOS</h1>

Write a script (for the design of a Clos network) that :

<ul>

 <li>takes as input: N, number of inputs/outputs, and n, size of the crossbar module used for building switches – in the first stage, n is also the number of inputs per module allowed</li>

 <li>calculates the number of modules in each of the three stages of a Clos network, and the number of inputs and outputs of modules in both cases, <em>strictly non-blocking</em> and <em>rearrangeable</em> network</li>

 <li>writes in output the number and size of modules, for each of the three stages, in the two cases</li>

 <li>calculates the gain when using the Clos network, with respect to the Crossbar N x N, comparing their costs, in both cases strictly non-blocking and rearrangeable non-blocking,</li>

</ul>

<h1>Reference: Exercise discussed in lecture given on 11 May 2020</h1>