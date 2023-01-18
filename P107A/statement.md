## Description

<div><p>The German University in Cairo (GUC) dorm houses are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Underground water pipes connect these houses together. Each pipe has certain direction (water can flow only in this direction and not vice versa), and diameter (which characterizes the maximal amount of water it can handle).</p><p>For each house, there is at most one pipe going into it and at most one pipe going out of it. With the new semester starting, GUC student and dorm resident, Lulu, wants to install tanks and taps at the dorms. For every house with an outgoing water pipe and without an incoming water pipe, Lulu should install a water tank at that house. For every house with an incoming water pipe and without an outgoing water pipe, Lulu should install a water tap at that house. Each tank house will convey water to all houses that have a sequence of pipes from the tank to it. Accordingly, each tap house will receive water originating from some tank house.</p><p>In order to avoid pipes from bursting one week later (like what happened last semester), Lulu also has to consider the diameter of the pipes. The amount of water each tank conveys should not exceed the diameter of the pipes connecting a tank to its corresponding tap. Lulu wants to find the maximal amount of water that can be safely conveyed from each tank to its corresponding tap.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000, 0 ≤ <i>p</i> ≤ <i>n</i>)</span> — the number of houses and the number of pipes correspondingly. </p><p>Then <span class="tex-span"><i>p</i></span> lines follow — the description of <span class="tex-span"><i>p</i></span> pipes. The <span class="tex-span"><i>i</i></span>-th line contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, indicating a pipe of diameter <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> going from house <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to house <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>It is guaranteed that for each house there is at most one pipe going into it and at most one pipe going out of it.</p></div><div class="output-specification"><p>Print integer <span class="tex-span"><i>t</i></span> in the first line — the number of tank-tap pairs of houses.</p><p>For the next <span class="tex-span"><i>t</i></span> lines, print 3 integers per line, separated by spaces: <span class="tex-span"><i>tank</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>tap</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>diameter</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>tank</i><sub class="lower-index"><i>i</i></sub> ≠ <i>tap</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>t</i></span>). Here <span class="tex-span"><i>tank</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>tap</i><sub class="lower-index"><i>i</i></sub></span> are indexes of tank and tap houses respectively, and <span class="tex-span"><i>diameter</i><sub class="lower-index"><i>i</i></sub></span> is the maximum amount of water that can be conveyed. All the <span class="tex-span"><i>t</i></span> lines should be ordered (increasingly) by <span class="tex-span"><i>tank</i><sub class="lower-index"><i>i</i></sub></span>.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 1000, 0 ≤ <i>p</i> ≤ <i>n</i>)</span> — the number of houses and the number of pipes correspondingly. </p><p>Then <span class="tex-span"><i>p</i></span> lines follow — the description of <span class="tex-span"><i>p</i></span> pipes. The <span class="tex-span"><i>i</i></span>-th line contains three integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, indicating a pipe of diameter <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> going from house <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to house <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>, <i>a</i><sub class="lower-index"><i>i</i></sub> ≠ <i>b</i><sub class="lower-index"><i>i</i></sub>, 1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>It is guaranteed that for each house there is at most one pipe going into it and at most one pipe going out of it.</p>

## Output

<p>Print integer <span class="tex-span"><i>t</i></span> in the first line — the number of tank-tap pairs of houses.</p><p>For the next <span class="tex-span"><i>t</i></span> lines, print 3 integers per line, separated by spaces: <span class="tex-span"><i>tank</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>tap</i><sub class="lower-index"><i>i</i></sub></span>, and <span class="tex-span"><i>diameter</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>tank</i><sub class="lower-index"><i>i</i></sub> ≠ <i>tap</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>t</i></span>). Here <span class="tex-span"><i>tank</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>tap</i><sub class="lower-index"><i>i</i></sub></span> are indexes of tank and tap houses respectively, and <span class="tex-span"><i>diameter</i><sub class="lower-index"><i>i</i></sub></span> is the maximum amount of water that can be conveyed. All the <span class="tex-span"><i>t</i></span> lines should be ordered (increasingly) by <span class="tex-span"><i>tank</i><sub class="lower-index"><i>i</i></sub></span>.</p>





```input1
3 2
1 2 10
2 3 20

```




```input2
3 3
1 2 20
2 3 10
3 1 5

```




```input3
4 2
1 2 60
3 4 50

```




```output1
1
1 3 10

```




```output2
0

```




```output3
2
1 2 60
3 4 50

```


