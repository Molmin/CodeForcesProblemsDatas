## Description

<div><p>Polycarp is currently developing a project in Vaja language and using a popular dependency management system called Vamen. From Vamen's point of view both Vaja project and libraries are treated projects for simplicity.</p><p>A project in Vaja has its own uniqie non-empty name consisting of lowercase latin letters with length not exceeding <span class="tex-span">10</span> and version — positive integer from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">6</sup></span>. Each project (keep in mind that it is determined by both its name and version) might depend on other projects. For sure, there are no cyclic dependencies.</p><p>You're given a list of project descriptions. <span class="tex-font-style-bf">The first</span> of the given projects is the one being developed by Polycarp at this moment. Help Polycarp determine all projects that his project depends on (directly or via a certain chain). </p><p>It's possible that Polycarp's project depends on two different versions of some project. In this case collision resolving is applied, i.e. for each such project the system chooses the version that minimizes the distance from it to Polycarp's project. If there are several options, the newer (with the maximum version) is preferred. This version is considered actual; <span class="tex-font-style-bf">other versions and their dependencies are ignored.</span></p><p>More formal, choose such a set of projects of minimum possible size that the following conditions hold: </p><ul> <li> Polycarp's project is chosen; </li><li> Polycarp's project depends (directly or indirectly) on all other projects in the set; </li><li> no two projects share the name; </li><li> for each project <span class="tex-span"><i>x</i></span> that some other project in the set depends on we have either <span class="tex-span"><i>x</i></span> or some <span class="tex-span"><i>y</i></span> with other version and shorter chain to Polycarp's project chosen. In case of ties the newer one is chosen. </li></ul><p>Output all Polycarp's project's dependencies (Polycarp's project itself should't be printed) in lexicographical order.</p></div><div class="input-specification"><p>The first line contains an only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>) — the number of projects in Vaja.</p><p>The following lines contain the project descriptions. Each project is described by a line consisting of its name and version separated by space. The next line gives the number of direct dependencies (from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>) and the dependencies themselves (one in a line) in arbitrary order. Each dependency is specified by its name and version. The projects are also given in arbitrary order, but the first of them is always Polycarp's. Project descriptions are separated by one empty line. Refer to samples for better understanding.</p><p>It's guaranteed that there are no cyclic dependencies. </p></div><div class="output-specification"><p>Output all Polycarp's project's dependencies in lexicographical order.</p></div>

## Input

<p>The first line contains an only integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1 000</span>) — the number of projects in Vaja.</p><p>The following lines contain the project descriptions. Each project is described by a line consisting of its name and version separated by space. The next line gives the number of direct dependencies (from <span class="tex-span">0</span> to <span class="tex-span"><i>n</i> - 1</span>) and the dependencies themselves (one in a line) in arbitrary order. Each dependency is specified by its name and version. The projects are also given in arbitrary order, but the first of them is always Polycarp's. Project descriptions are separated by one empty line. Refer to samples for better understanding.</p><p>It's guaranteed that there are no cyclic dependencies. </p>

## Output

<p>Output all Polycarp's project's dependencies in lexicographical order.</p>





```input1
4
a 3
2
b 1
c 1
&nbsp;
b 2
0
&nbsp;
b 1
1
b 2
&nbsp;
c 1
1
b 2

```




```input2
9
codehorses 5
3
webfrmk 6
mashadb 1
mashadb 2
&nbsp;
commons 2
0
&nbsp;
mashadb 3
0
&nbsp;
webfrmk 6
2
mashadb 3
commons 2
&nbsp;
extra 4
1
extra 3
&nbsp;
extra 3
0
&nbsp;
extra 1
0
&nbsp;
mashadb 1
1
extra 3
&nbsp;
mashadb 2
1
extra 1

```




```input3
3
abc 1
2
abc 3
cba 2

abc 3
0

cba 2
0

```




```output1
2
b 1
c 1

```




```output2
4
commons 2
extra 1
mashadb 2
webfrmk 6

```




```output3
1
cba 2

```



## Note

<p>The first sample is given in the pic below. Arrow from <span class="tex-span"><i>A</i></span> to <span class="tex-span"><i>B</i></span> means that <span class="tex-span"><i>B</i></span> directly depends on <span class="tex-span"><i>A</i></span>. Projects that Polycarp's project «<span class="tex-font-style-tt">a</span>» (version <span class="tex-span">3</span>) depends on are painted black.</p><center> <img class="tex-graphics" src="file://0eym0WZH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The second sample is again given in the pic below. Arrow from <span class="tex-span"><i>A</i></span> to <span class="tex-span"><i>B</i></span> means that <span class="tex-span"><i>B</i></span> directly depends on <span class="tex-span"><i>A</i></span>. Projects that Polycarp's project «<span class="tex-font-style-tt">codehorses</span>» (version <span class="tex-span">5</span>) depends on are paint it black. Note that «<span class="tex-font-style-tt">extra 1</span>» is chosen instead of «<span class="tex-font-style-tt">extra 3</span>» since «<span class="tex-font-style-tt">mashadb 1</span>» and all of its dependencies are ignored due to «<span class="tex-font-style-tt">mashadb 2</span>».</p><center> <img class="tex-graphics" src="file://uPvu0cX3.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
