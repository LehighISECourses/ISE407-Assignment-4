<p>Assignment 4 <br>
Due: October 29, 2020 <br>

Note: A full HTML version of this document can be viewed [here](https://htmlpreview.github.io/?https://github.com/LehighISECourses/ISE407-Assignment-4/blob/main/README.html).

</p><ol class="enumerate" type=1><li class="li-enumerate">Consider the following algorithm for multiplying 2 &#XD7; 2
matrices. To compute the product
<table class="display dcenter"><tr style="vertical-align:middle"><td class="dcell">
</td><td class="dcell">&#X23A1;<br>
&#X23A2;<br>
&#X23A3;</td><td class="dcell"><table style="border-spacing:6px;border-collapse:separate;" class="cellpading0"><tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">c</span><sub>11</sub></td><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">c</span><sub>12</sub> </td></tr>
<tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">c</span><sub>21</sub></td><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">c</span><sub>22</sub> </td></tr>
</table></td><td class="dcell">&#XA0;</td><td class="dcell">&#X23A4;<br>
&#X23A5;<br>
&#X23A6;</td><td class="dcell">
=&#XA0;
</td><td class="dcell">&#X23A1;<br>
&#X23A2;<br>
&#X23A3;</td><td class="dcell"><table style="border-spacing:6px;border-collapse:separate;" class="cellpading0"><tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">a</span><sub>11</sub></td><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">a</span><sub>12</sub> </td></tr>
<tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">a</span><sub>21</sub></td><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">a</span><sub>22</sub> </td></tr>
</table></td><td class="dcell">&#XA0;</td><td class="dcell">&#X23A4;<br>
&#X23A5;<br>
&#X23A6;</td><td class="dcell">
</td><td class="dcell">&#X23A1;<br>
&#X23A2;<br>
&#X23A3;</td><td class="dcell"><table style="border-spacing:6px;border-collapse:separate;" class="cellpading0"><tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">b</span><sub>11</sub></td><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">b</span><sub>12</sub> </td></tr>
<tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">b</span><sub>21</sub></td><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">b</span><sub>22</sub> </td></tr>
</table></td><td class="dcell">&#XA0;</td><td class="dcell">&#X23A4;<br>
&#X23A5;<br>
&#X23A6;</td><td class="dcell">,
&#XA0;&#XA0;&#XA0;&#XA0;(1)</td></tr>
</table>
we first compute the following products:
<table class="display dcenter"><tr style="vertical-align:middle"><td class="dcell">
&#XA0;&#XA0;&#XA0;&#XA0;&#XA0;

</td><td class="dcell"><table style="border-spacing:6px;border-collapse:separate;" class="cellpading0"><tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">m</span><sub>1</sub></td><td style="text-align:left;white-space:nowrap" >&#XA0;=&#XA0;(<span style="font-style:italic">a</span><sub>12</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">a</span><sub>22</sub>)(<span style="font-style:italic">b</span><sub>21</sub>&#XA0;+&#XA0;<span style="font-style:italic">b</span><sub>22</sub>)&#XA0;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(2)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" >
<span style="font-style:italic">m</span><sub>2</sub></td><td style="text-align:left;white-space:nowrap" >&#XA0;=&#XA0;(<span style="font-style:italic">a</span><sub>11</sub>&#XA0;+&#XA0;<span style="font-style:italic">a</span><sub>22</sub>)(<span style="font-style:italic">b</span><sub>11</sub>&#XA0;+&#XA0;<span style="font-style:italic">b</span><sub>22</sub>)&#XA0;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(3)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" >
<span style="font-style:italic">m</span><sub>3</sub></td><td style="text-align:left;white-space:nowrap" >&#XA0;=&#XA0;(<span style="font-style:italic">a</span><sub>11</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">a</span><sub>21</sub>)(<span style="font-style:italic">b</span><sub>11</sub>&#XA0;+&#XA0;<span style="font-style:italic">b</span><sub>12</sub>)&#XA0;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(4)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" >
<span style="font-style:italic">m</span><sub>4</sub></td><td style="text-align:left;white-space:nowrap" >&#XA0;=&#XA0;(<span style="font-style:italic">a</span><sub>11</sub>&#XA0;+&#XA0;<span style="font-style:italic">a</span><sub>12</sub>)&#XA0;<span style="font-style:italic">b</span><sub>22</sub>&#XA0;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(5)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" >
<span style="font-style:italic">m</span><sub>5</sub></td><td style="text-align:left;white-space:nowrap" >&#XA0;=&#XA0;<span style="font-style:italic">a</span><sub>11</sub>(<span style="font-style:italic">b</span><sub>12</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">b</span><sub>22</sub>)&#XA0;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(6)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" >
<span style="font-style:italic">m</span><sub>6</sub></td><td style="text-align:left;white-space:nowrap" >&#XA0;=&#XA0;<span style="font-style:italic">a</span><sub>22</sub>(<span style="font-style:italic">b</span><sub>21</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">b</span><sub>11</sub>)&#XA0;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(7)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" >
<span style="font-style:italic">m</span><sub>7</sub></td><td style="text-align:left;white-space:nowrap" >&#XA0;=&#XA0;(<span style="font-style:italic">a</span><sub>21</sub>&#XA0;+&#XA0;<span style="font-style:italic">a</span><sub>22</sub>)&#XA0;<span style="font-style:italic">b</span><sub>11</sub>.
</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(8)</td></tr>
</table></td></tr>
</table>
Then compute the entries in the product matrix with 
<table class="display dcenter"><tr style="vertical-align:middle"><td class="dcell">
&#XA0;&#XA0;&#XA0;&#XA0;&#XA0;

</td><td class="dcell"><table style="border-spacing:6px;border-collapse:separate;" class="cellpading0"><tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">c</span><sub>11</sub></td><td style="text-align:left;white-space:nowrap" >&#XA0;=&#XA0;<span style="font-style:italic">m</span><sub>1</sub>&#XA0;+&#XA0;<span style="font-style:italic">m</span><sub>2</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">m</span><sub>4</sub>&#XA0;+&#XA0;<span style="font-style:italic">m</span><sub>6</sub>&#XA0;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(9)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" >
<span style="font-style:italic">c</span><sub>12</sub></td><td style="text-align:left;white-space:nowrap" >&#XA0;=&#XA0;<span style="font-style:italic">m</span><sub>4</sub>&#XA0;+&#XA0;<span style="font-style:italic">m</span><sub>5</sub>&#XA0;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(10)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" >
<span style="font-style:italic">c</span><sub>21</sub></td><td style="text-align:left;white-space:nowrap" >&#XA0;=&#XA0;<span style="font-style:italic">m</span><sub>6</sub>&#XA0;+&#XA0;<span style="font-style:italic">m</span><sub>7</sub>&#XA0;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(11)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" >
<span style="font-style:italic">c</span><sub>22</sub></td><td style="text-align:left;white-space:nowrap" >&#XA0;=&#XA0;<span style="font-style:italic">m</span><sub>2</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">m</span><sub>3</sub>&#XA0;+&#XA0;<span style="font-style:italic">m</span><sub>5</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">m</span><sub>7</sub>.
</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&nbsp;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(12)</td></tr>
</table></td></tr>
</table>
With this technique, we compute the product with seven
multiplications and 18 additions rather than the usual eight
multiplications and four additions. Although this does not result in a
savings for the case of 2 &#XD7; 2 matrices, the technique can be
generalized to improve up the asymptotic running time of the naive
algorithm, which requires <span style="font-style:italic">O</span>(<span style="font-style:italic">n</span><sup>3</sup>) operations.<ol class="enumerate" type=a><li class="li-enumerate">Generalize the above method to derive a recursive method for
multiplying two <span style="font-style:italic">n</span> &#XD7; <span style="font-style:italic">n</span> matrices. You may assume <span style="font-style:italic">n</span> is a power
of 2. </li><li class="li-enumerate">Write the recursion for the running time of your method, solve
it, and show that the running time of this method is asymptotically
better than that of the naive algorithm. </li><li class="li-enumerate">Propose a parallel version of this algorithm and analyze its
running time using the PRAM model of computation. Can the number of
processors be chosen so as to make this algorithm cost-optimal?
Would the running time be affected if the underlying architecture
had more restricted communication, such as with a mesh?</li></ol></li><li class="li-enumerate">Propose a method of parallelizing the naive algorithm for matrix
multiplication under the PRAM model and analyze it both
theoretically and empirically using a standard strong scalability analysis in
Julia. Use the department&#X2019;s compute cluster to test with up to 16 cores
(bonus points for testing a distributed version on more than one node!).</li><li class="li-enumerate">Solve each of the following recurrences, assuming
that <span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>) is constant for sufficiently small values of
<span style="font-style:italic">n</span>. Explain how you got your answer.<ol class="enumerate" type=a><li class="li-enumerate"><span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>) = 2<span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>/2) + <span style="font-style:italic">n</span><sup>3</sup></li><li class="li-enumerate"><span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>) = 2<span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>/4) + &#X221A;<span style="text-decoration:overline"><span style="font-style:italic">n</span></span></li><li class="li-enumerate"><span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>) = <span style="font-style:italic">T</span>(&#X221A;<span style="text-decoration:overline"><span style="font-style:italic">n</span></span>) + 1</li><li class="li-enumerate"><span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>) = 4<span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>/2) + <span style="font-style:italic">n</span><sup>2</sup> &#X221A;<span style="text-decoration:overline"><span style="font-style:italic">n</span></span></li></ol></li><li class="li-enumerate">Suppose you have one machine and a set of <span style="font-style:italic">n</span> tasks. Task <span style="font-style:italic">j</span> has a processing time <span style="font-style:italic">w</span><sub><span style="font-style:italic">j</span></sub>, a profit
<span style="font-style:italic">p</span><sub><span style="font-style:italic">j</span></sub>, and a deadline <span style="font-style:italic">d</span><sub><span style="font-style:italic">j</span></sub>. If you complete a task <span style="font-style:italic">j</span> by
deadline <span style="font-style:italic">d</span><sub><span style="font-style:italic">j</span></sub>, you receive a profit <span style="font-style:italic">p</span><sub><span style="font-style:italic">j</span></sub> (otherwise, you receive
no profit). You wish to find a schedule that completes all the tasks
and derives the maximum profit. <ol class="enumerate" type=a><li class="li-enumerate">State the decision version of this problem.</li><li class="li-enumerate">show that it is NP-complete by reducing the knapsack problem to
it.</li><li class="li-enumerate">Give a polynomial-time algorithm for the decision problem,
assuming that all processing times are integers from 1 to <span style="font-style:italic">n</span>. </li></ol></li></ol>
