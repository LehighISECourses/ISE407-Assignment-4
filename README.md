<!DOCTYPE html>
<html >
<head>
<meta http-equiv="Content-Type" content="text/html; charset=US-ASCII">
<meta name="generator" content="hevea 2.30">
<style type="text/css">
.li-itemize{margin:1ex 0ex;}
.li-enumerate{margin:1ex 0ex;}
.dd-description{margin:0ex 0ex 1ex 4ex;}
.dt-description{margin:0ex;}
.toc{list-style:none;}
.footnotetext{margin:0ex; padding:0ex;}
div.footnotetext P{margin:0px; text-indent:1em;}
.thefootnotes{text-align:left;margin:0ex;}
.dt-thefootnotes{margin:0em;}
.dd-thefootnotes{margin:0em 0em 0em 2em;}
.footnoterule{margin:1em auto 1em 0px;width:50%;}
.caption{padding-left:2ex; padding-right:2ex; margin-left:auto; margin-right:auto}
.title{margin:2ex auto;text-align:center}
.titlemain{margin:1ex 2ex 2ex 1ex;}
.titlerest{margin:0ex 2ex;}
.center{text-align:center;margin-left:auto;margin-right:auto;}
.flushleft{text-align:left;margin-left:0ex;margin-right:auto;}
.flushright{text-align:right;margin-left:auto;margin-right:0ex;}
div table{margin-left:inherit;margin-right:inherit;margin-bottom:2px;margin-top:2px}
td table{margin:auto;}
table{border-collapse:collapse;}
td{padding:0;}
.cellpadding0 tr td{padding:0;}
.cellpadding1 tr td{padding:1px;}
pre{text-align:left;margin-left:0ex;margin-right:auto;}
blockquote{margin-left:4ex;margin-right:4ex;text-align:left;}
td p{margin:0px;}
.boxed{border:1px solid black}
.textboxed{border:1px solid black}
.vbar{border:none;width:2px;background-color:black;}
.hbar{border:none;height:2px;width:100%;background-color:black;}
.hfill{border:none;height:1px;width:200%;background-color:black;}
.vdisplay{border-collapse:separate;border-spacing:2px;width:auto; empty-cells:show; border:2px solid red;}
.vdcell{white-space:nowrap;padding:0px; border:2px solid green;}
.display{border-collapse:separate;border-spacing:2px;width:auto; border:none;}
.dcell{white-space:nowrap;padding:0px; border:none;}
.dcenter{margin:0ex auto;}
.vdcenter{border:solid #FF8000 2px; margin:0ex auto;}
.minipage{text-align:left; margin-left:0em; margin-right:auto;}
.marginpar{border:solid thin black; width:20%; text-align:left;}
.marginparleft{float:left; margin-left:0ex; margin-right:1ex;}
.marginparright{float:right; margin-left:1ex; margin-right:0ex;}
.theorem{text-align:left;margin:1ex auto 1ex 0ex;}
.part{margin:2ex auto;text-align:center}
</style>
<title>ps4</title>
</head>
<body >
<!--HEVEA command line is: /usr/bin/hevea ps4.tex -->
<!--CUT STYLE article--><!--CUT DEF section 1 --><p><span style="font-size:x-large"><span style="font-weight:bold">Problem Set 4 <br>
ISE 407 &#X2013; Computational Methods in Optimization <br>
Due: November 1, 2019 <br>
Dr. Ralphs</span></span> <br>

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

</td><td class="dcell"><table style="border-spacing:6px;border-collapse:separate;" class="cellpading0"><tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">m</span><sub>1</sub></td><td style="text-align:center;white-space:nowrap" >&#XA0;=&#XA0;(<span style="font-style:italic">a</span><sub>12</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">a</span><sub>22</sub>)(<span style="font-style:italic">b</span><sub>21</sub>&#XA0;+&#XA0;<span style="font-style:italic">b</span><sub>22</sub>)&#XA0;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(2)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">m</span><sub>2</sub></td><td style="text-align:center;white-space:nowrap" >&#XA0;=&#XA0;(<span style="font-style:italic">a</span><sub>11</sub>&#XA0;+&#XA0;<span style="font-style:italic">a</span><sub>22</sub>)(<span style="font-style:italic">b</span><sub>11</sub>&#XA0;+&#XA0;<span style="font-style:italic">b</span><sub>22</sub>)&#XA0;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(3)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">m</span><sub>3</sub></td><td style="text-align:center;white-space:nowrap" >&#XA0;=&#XA0;(<span style="font-style:italic">a</span><sub>11</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">a</span><sub>21</sub>)(<span style="font-style:italic">b</span><sub>11</sub>&#XA0;+&#XA0;<span style="font-style:italic">b</span><sub>12</sub>)&#XA0;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(4)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">m</span><sub>4</sub></td><td style="text-align:center;white-space:nowrap" >&#XA0;=&#XA0;(<span style="font-style:italic">a</span><sub>11</sub>&#XA0;+&#XA0;<span style="font-style:italic">a</span><sub>12</sub>)&#XA0;<span style="font-style:italic">b</span><sub>22</sub>&#XA0;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(5)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">m</span><sub>5</sub></td><td style="text-align:center;white-space:nowrap" >&#XA0;=&#XA0;<span style="font-style:italic">a</span><sub>11</sub>(<span style="font-style:italic">b</span><sub>12</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">b</span><sub>22</sub>)&#XA0;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(6)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">m</span><sub>6</sub></td><td style="text-align:center;white-space:nowrap" >&#XA0;=&#XA0;<span style="font-style:italic">a</span><sub>22</sub>(<span style="font-style:italic">b</span><sub>21</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">b</span><sub>11</sub>)&#XA0;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(7)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">m</span><sub>7</sub></td><td style="text-align:center;white-space:nowrap" >&#XA0;=&#XA0;(<span style="font-style:italic">a</span><sub>21</sub>&#XA0;+&#XA0;<span style="font-style:italic">a</span><sub>22</sub>)&#XA0;<span style="font-style:italic">b</span><sub>11</sub>.
</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(8)</td></tr>
</table></td></tr>
</table>
Then compute the entries in the product matrix with 
<table class="display dcenter"><tr style="vertical-align:middle"><td class="dcell">


&#XA0;&#XA0;&#XA0;&#XA0;&#XA0;

</td><td class="dcell"><table style="border-spacing:6px;border-collapse:separate;" class="cellpading0"><tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">c</span><sub>11</sub></td><td style="text-align:center;white-space:nowrap" >&#XA0;=&#XA0;<span style="font-style:italic">m</span><sub>1</sub>&#XA0;+&#XA0;<span style="font-style:italic">m</span><sub>2</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">m</span><sub>4</sub>&#XA0;+&#XA0;<span style="font-style:italic">m</span><sub>6</sub>&#XA0;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(9)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">c</span><sub>12</sub></td><td style="text-align:center;white-space:nowrap" >&#XA0;=&#XA0;<span style="font-style:italic">m</span><sub>4</sub>&#XA0;+&#XA0;<span style="font-style:italic">m</span><sub>5</sub>&#XA0;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(10)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">c</span><sub>21</sub></td><td style="text-align:center;white-space:nowrap" >&#XA0;=&#XA0;<span style="font-style:italic">m</span><sub>6</sub>&#XA0;+&#XA0;<span style="font-style:italic">m</span><sub>7</sub>&#XA0;</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(11)</td></tr>
<tr><td style="text-align:right;white-space:nowrap" ><span style="font-style:italic">c</span><sub>22</sub></td><td style="text-align:center;white-space:nowrap" >&#XA0;=&#XA0;<span style="font-style:italic">m</span><sub>2</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">m</span><sub>3</sub>&#XA0;+&#XA0;<span style="font-style:italic">m</span><sub>5</sub>&#XA0;&#X2212;&#XA0;<span style="font-style:italic">m</span><sub>7</sub>.
</td><td style="text-align:left;white-space:nowrap" >&nbsp;</td><td style="text-align:right;white-space:nowrap" >&#XA0;&#XA0;&#XA0;&#XA0;(12)</td></tr>
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
multiplication under the PRAM model and analyze it theoretically. </li><li class="li-enumerate">Solve each of the following recurrences, assuming
that <span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>) is constant for sufficiently small values of
<span style="font-style:italic">n</span>. Explain how you got your answer.<ol class="enumerate" type=a><li class="li-enumerate"><span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>) = 2<span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>/2) + <span style="font-style:italic">n</span><sup>3</sup></li><li class="li-enumerate"><span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>) = 2<span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>/4) + &#X221A;<span style="text-decoration:overline"><span style="font-style:italic">n</span></span></li><li class="li-enumerate"><span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>) = <span style="font-style:italic">T</span>(&#X221A;<span style="text-decoration:overline"><span style="font-style:italic">n</span></span>) + 1</li><li class="li-enumerate"><span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>) = 4<span style="font-style:italic">T</span>(<span style="font-style:italic">n</span>/2) + <span style="font-style:italic">n</span><sup>2</sup> &#X221A;<span style="text-decoration:overline"><span style="font-style:italic">n</span></span></li></ol></li><li class="li-enumerate">Suppose you have one machine and a set of <span style="font-style:italic">n</span> tasks <span style="font-style:italic">a</span><sub>1</sub>, <span style="font-style:italic">a</span><sub>2</sub>,
&#X2026;, <span style="font-style:italic">a</span><sub><span style="font-style:italic">n</span></sub>. Each task <span style="font-style:italic">a</span><sub><span style="font-style:italic">j</span></sub> has a processing time <span style="font-style:italic">p</span><sub><span style="font-style:italic">j</span></sub>, a profit
<span style="font-style:italic">p</span><sub><span style="font-style:italic">j</span></sub>, and a deadline <span style="font-style:italic">d</span><sub><span style="font-style:italic">j</span></sub>. If you complete a task <span style="font-style:italic">a</span><sub><span style="font-style:italic">j</span></sub> by
deadline <span style="font-style:italic">d</span><sub><span style="font-style:italic">j</span></sub>, you receive a profit <span style="font-style:italic">p</span><sub><span style="font-style:italic">j</span></sub> (otherwise, you receive
no profit). You wish to find a schedule that completes all the tasks
and derives the maximum profit. <ol class="enumerate" type=a><li class="li-enumerate">State the decision version of this problem.</li><li class="li-enumerate">show that it is NP-complete by reducing the knapsack problem to
it.</li><li class="li-enumerate">Give a polynomial-time algorithm for the decision problem,
assuming that all processing times are integers from 1 to <span style="font-style:italic">n</span>. </li></ol></li><li class="li-enumerate">This problem considers algorithms for sorting. You are to choose any two
(or more) optimal sorting algorithm and implement them in C++ according the
following guidelines.
<ul class="itemize"><li class="li-itemize">
Your implementation should be
object-oriented and should consist of a base class to contain the list, with
two derived classes containing the implementations of the two sorting methods.
</li><li class="li-itemize">You should provide a single <span style="font-family:monospace">main()</span> function that can be
compiled to produce a sorting program that reads the data from the stadard
input and then uses one of the two implementations to sort the data and
write it to the standard output, with the choice being a compile-time
option specified by defining certain symbols.
</li><li class="li-itemize">You should provide a simple Makefile, with one target for each sorting
algorithm, that specifies the proper symbol and builds a binary using the
chosen sorting method. Please give your binaries different names and
supply a target &#X201C;all&#X201D; that builds all binaries.
</li><li class="li-itemize">You should write a script that produces a graph of the empirical
running times functions of all sorting methods in a single figure by
generating random data and feeding it into your programs. The script can
be written in bash or Python.
</li></ul>
Do an empirical analysis of your two methods according to the following
guidelines. 
<ul class="itemize"><li class="li-itemize">
Plot the empirical running time functions for your initial implementations of
the two methods. 
</li><li class="li-itemize">Plot similar graphs based on operation counts. You can do this by
separating out the operations into functions and then using a profiler to
count the operations. Discuss how these compare to the empirical running
time functions. 
</li><li class="li-itemize">Use <span style="font-family:monospace">cache_grind</span> to do an analysis of cache usage. Do you
notice anything interesting?
</li><li class="li-itemize">Compare the methods using a performance profile for a fixed input
size. Does one method completely dominate the other or does it depend on
the input? If the latter, try to determine what kinds of inputs favor one
implementation or the other. 
</li><li class="li-itemize">See if there is any way to optimize your favorite implementation
by expliting cache effects or otherwise. Report on any optimizations you
find. 
</li></ul></li></ol><!--CUT END -->
<!--HTMLFOOT-->
<!--ENDHTML-->
<!--FOOTER-->
<hr style="height:2"><blockquote class="quote"><em>This document was translated from L<sup>A</sup>T<sub>E</sub>X by
</em><a href="http://hevea.inria.fr/index.html"><em>H</em><em><span style="font-size:small"><sup>E</sup></span></em><em>V</em><em><span style="font-size:small"><sup>E</sup></span></em><em>A</em></a><em>.</em></blockquote></body>
</html>
