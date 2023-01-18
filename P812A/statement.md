## Description

<div><p>Sagheer is walking in the street when he comes to an intersection of two roads. Each road can be represented as two parts where each part has <span class="tex-span">3</span> lanes getting into the intersection (one for each direction) and <span class="tex-span">3</span> lanes getting out of the intersection, so we have <span class="tex-span">4</span> parts in total. Each part has <span class="tex-span">4</span> lights, one for each lane getting into the intersection (<span class="tex-span"><i>l</i></span> — left, <span class="tex-span"><i>s</i></span> — straight, <span class="tex-span"><i>r</i></span> — right) and a light <span class="tex-span"><i>p</i></span> for a pedestrian crossing. </p><center> <img class="tex-graphics" src="file://yjBlI6y5.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>An accident is possible if a car can hit a pedestrian. This can happen if the light of a pedestrian crossing of some part and the light of a lane that can get to or from that same part are green at the same time.</p><p>Now, Sagheer is monitoring the configuration of the traffic lights. Your task is to help him detect whether an accident is possible.</p></div><div class="input-specification"><p>The input consists of four lines with each line describing a road part given in a counter-clockwise order.</p><p>Each line contains four integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>p</i></span> — for the left, straight, right and pedestrian lights, respectively. The possible values are <span class="tex-span">0</span> for red light and <span class="tex-span">1</span> for green light.</p></div><div class="output-specification"><p>On a single line, print "<span class="tex-font-style-tt">YES</span>" if an accident is possible, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p></div>

## Input

<p>The input consists of four lines with each line describing a road part given in a counter-clockwise order.</p><p>Each line contains four integers <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>r</i></span>, <span class="tex-span"><i>p</i></span> — for the left, straight, right and pedestrian lights, respectively. The possible values are <span class="tex-span">0</span> for red light and <span class="tex-span">1</span> for green light.</p>

## Output

<p>On a single line, print "<span class="tex-font-style-tt">YES</span>" if an accident is possible, and "<span class="tex-font-style-tt">NO</span>" otherwise.</p>





```input1
1 0 0 1
0 1 0 0
0 0 1 0
0 0 0 1

```




```input2
0 1 1 0
1 0 1 0
1 1 0 0
0 0 0 1

```




```input3
1 0 0 0
0 0 0 1
0 0 0 0
1 0 1 0

```




```output1
YES

```




```output2
NO

```




```output3
NO

```



## Note

<p>In the first example, some accidents are possible because cars of part <span class="tex-span">1</span> can hit pedestrians of parts <span class="tex-span">1</span> and <span class="tex-span">4</span>. Also, cars of parts <span class="tex-span">2</span> and <span class="tex-span">3</span> can hit pedestrians of part <span class="tex-span">4</span>.</p><p>In the second example, no car can pass the pedestrian crossing of part <span class="tex-span">4</span> which is the only green pedestrian light. So, no accident can occur.</p>
