Download Link: https://assignmentchef.com/product/solved-cse-4082-project-1
<br>
Diagonal 15-Puzzle is a modified version of the 15-Puzzle in which the blank square may slide about a diagonal axis in addition to horizontal and vertical axes. However, the cost of each diagonal slide is 3 whereas the cost of each horizontal or vertical slide is 1. The final state of the Diagonal 15-Puzzle is as follows:

<table width="145">

 <tbody>

  <tr>

   <td width="37">1</td>

   <td width="36">2</td>

   <td width="36">3</td>

   <td width="36">4</td>

  </tr>

  <tr>

   <td width="37">12</td>

   <td width="36">13</td>

   <td width="36">14</td>

   <td width="36">5</td>

  </tr>

  <tr>

   <td width="37">11</td>

   <td width="36"> </td>

   <td width="36">15</td>

   <td width="36">6</td>

  </tr>

  <tr>

   <td width="37">10</td>

   <td width="36">9</td>

   <td width="36">8</td>

   <td width="36">7</td>

  </tr>

 </tbody>

</table>




In this project, you are required to implement the following search methods for solving the Diagonal 15-Puzzle:

<ol>

 <li>Uniform Cost Search</li>

 <li>Iterative Lengthening Search</li>

 <li>A* Heuristic Search with the admissible heuristic h1 discussed in class (h1(n) = The number of misplaced tiles at node n)</li>

 <li>A* Heuristic Search with the admissible heuristic h2 discussed in class (h2(n) = The sum of the city-block distances of each misplaced tile from its current location to its goal location)</li>

 <li>(Bonus – 10 points) A* Heuristic Search with the admissible heuristic h3 which provides better solutions than h2.</li>

</ol>

In order to compare performances of these methods, your program should be able to generate random puzzle instances such that the optimum solution is at the depth d of the tree. In order to generate random puzzle instances, you may start from the final state and randomly go backwards.  Note that you should prevent cycles when generating random instances.

You have to provide the following outputs:

<table width="566">

 <tbody>

  <tr>

   <td width="112"> </td>

   <td colspan="3" width="343">The total number of expanded nodes</td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">d: depth of the solution</td>

   <td width="119">UCS</td>

   <td width="112">ILS</td>

   <td width="112">A*-H1</td>

   <td width="112">A*-H2</td>

  </tr>

  <tr>

   <td width="112">2</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">4</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">6</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">8</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">10</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">12</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">16</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">20</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">24</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">28</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

 </tbody>

</table>




<table width="566">

 <tbody>

  <tr>

   <td width="112"> </td>

   <td colspan="3" width="343">The maximum number of nodes stored in memory</td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">d: depth of the solution</td>

   <td width="119">UCS</td>

   <td width="112">ILS</td>

   <td width="112">A*-H1</td>

   <td width="112">A*-H2</td>

  </tr>

  <tr>

   <td width="112">2</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">4</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">6</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">8</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">10</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">12</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">16</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">20</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">24</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

  <tr>

   <td width="112">28</td>

   <td width="119"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

   <td width="112"> </td>

  </tr>

 </tbody>

</table>




For each entry in the above tables, <u>you have to generate 10 random instances</u> and report the arithmetic average. <u>You may not be able to fill every entry in the table since it may take too long</u>. In this case leave the corresponding entries empty.

In addition to the tables above, <u>for each of the three instances provided below and for each algorithm</u>, you should submit:

<ol>

 <li>The cost of the solution found.</li>

 <li>The solution path itself (from the given initial state to the final state). iii. The number of expanded nodes. a.</li>

</ol>

<table width="145">

 <tbody>

  <tr>

   <td width="37"> </td>

   <td width="36">1</td>

   <td width="36">3</td>

   <td width="36">4</td>

  </tr>

  <tr>

   <td width="37">12</td>

   <td width="36">13</td>

   <td width="36">2</td>

   <td width="36">5</td>

  </tr>

  <tr>

   <td width="37">11</td>

   <td width="36">14</td>

   <td width="36">15</td>

   <td width="36">6</td>

  </tr>

  <tr>

   <td width="37">10</td>

   <td width="36">9</td>

   <td width="36">8</td>

   <td width="36">7</td>

  </tr>

 </tbody>

</table>

b.

<table width="145">

 <tbody>

  <tr>

   <td width="37">1</td>

   <td width="36">3</td>

   <td width="36">5</td>

   <td width="36">4</td>

  </tr>

  <tr>

   <td width="37">2</td>

   <td width="36">13</td>

   <td width="36">14</td>

   <td width="36">15</td>

  </tr>

  <tr>

   <td width="37">11</td>

   <td width="36">12</td>

   <td width="36">9</td>

   <td width="36">6</td>

  </tr>

  <tr>

   <td width="37"> </td>

   <td width="36">10</td>

   <td width="36">8</td>

   <td width="36">7</td>

  </tr>

 </tbody>

</table>







c.

<table width="145">

 <tbody>

  <tr>

   <td width="37">1</td>

   <td width="36">13</td>

   <td width="36">3</td>

   <td width="36">4</td>

  </tr>

  <tr>

   <td width="37">12</td>

   <td width="36">11</td>

   <td width="36">2</td>

   <td width="36">5</td>

  </tr>

  <tr>

   <td width="37">9</td>

   <td width="36">8</td>

   <td width="36">15</td>

   <td width="36">7</td>

  </tr>

  <tr>

   <td width="37">10</td>

   <td width="36">6</td>

   <td width="36">14</td>

   <td width="36"> </td>

  </tr>

 </tbody>

</table>




Notes:




<ol>

 <li>The project should be done in groups of two! If you want to work in groups of three, then you have to implement the following algorithms additionally:

  <ol>

   <li>Depth First Search</li>

   <li>Breadth First Search</li>

  </ol></li>

</ol>

<ul>

 <li>Iterative Deepening Search</li>

</ul>

and report the results.




<ol>

 <li>Using source code (even partially) found from internet or any other resources is not allowed!</li>

</ol>




<ol>

 <li><u>You should also submit a design document</u> describing the classes (fields and methods) used in the project. This document should also contain the required tables and the other outputs.</li>

</ol>




<ol>

 <li><u>Your code will not be executed if you do not submit the required outputs!</u> Thus, if you do not present your outputs (two tables and outputs for the given three instances) in the document, you will get the minimum grade!</li>

</ol>




<ol>

 <li>Do not submit separate output file, embed the outputs in the design document!</li>

</ol>




<ol>

 <li>Do not submit any executable file (your e-mail may return back!) Submit only source code and design document (with outputs).</li>

</ol>





