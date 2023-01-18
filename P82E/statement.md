## Description

<div><p>Consider a house plan. </p><p>Let the house be represented by an infinite horizontal strip defined by the inequality <span class="tex-span"> - <i>h</i> ≤ <i>y</i> ≤ <i>h</i></span>. Strictly outside the house there are two light sources at the points <span class="tex-span">(0, <i>f</i>)</span> and <span class="tex-span">(0,  - <i>f</i>)</span>. Windows are located in the walls, the windows are represented by segments on the lines <span class="tex-span"><i>y</i> = <i>h</i></span> and <span class="tex-span"><i>y</i> =  - <i>h</i></span>. Also, the windows are arranged symmetrically about the line <span class="tex-span"><i>y</i> = 0</span>.</p><p>Your task is to find the area of the floor at the home, which will be lighted by the sources of light. </p><center> <img class="tex-graphics" src="file://baiAlPzO.png" style="max-width: 100.0%;max-height: 100.0%;"> </center></div><div class="input-specification"><p>The first line of the input file contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>f</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">1 ≤ <i>h</i> ≤ 10</span>, <span class="tex-span"><i>h</i> &lt; <i>f</i> ≤ 1000</span>). Next, <span class="tex-span"><i>n</i></span> lines contain two integers each <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 5000 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>), each entry indicates two segments. Endpoints of the first segment are <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>h</i>)</span>-<span class="tex-span">(<i>r</i><sub class="lower-index"><i>i</i></sub>, <i>h</i>)</span>, and endpoints of the second segment are <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>,  - <i>h</i>)</span>-<span class="tex-span">(<i>r</i><sub class="lower-index"><i>i</i></sub>,  - <i>h</i>)</span>. These segments describe location of windows. Numbers in the lines are space-separated. It is guaranteed that no two distinct segments have common points. </p></div><div class="output-specification"><p>Print the single real number — the area of the illuminated part of the floor with an absolute or relative error of no more than <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p></div>

## Input

<p>The first line of the input file contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>h</i></span> and <span class="tex-span"><i>f</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500</span>, <span class="tex-span">1 ≤ <i>h</i> ≤ 10</span>, <span class="tex-span"><i>h</i> &lt; <i>f</i> ≤ 1000</span>). Next, <span class="tex-span"><i>n</i></span> lines contain two integers each <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 5000 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> &lt; <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 5000</span>), each entry indicates two segments. Endpoints of the first segment are <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>h</i>)</span>-<span class="tex-span">(<i>r</i><sub class="lower-index"><i>i</i></sub>, <i>h</i>)</span>, and endpoints of the second segment are <span class="tex-span">(<i>l</i><sub class="lower-index"><i>i</i></sub>,  - <i>h</i>)</span>-<span class="tex-span">(<i>r</i><sub class="lower-index"><i>i</i></sub>,  - <i>h</i>)</span>. These segments describe location of windows. Numbers in the lines are space-separated. It is guaranteed that no two distinct segments have common points. </p>

## Output

<p>Print the single real number — the area of the illuminated part of the floor with an absolute or relative error of no more than <span class="tex-span">10<sup class="upper-index"> - 4</sup></span>.</p>





```input1
1 1 2
-1 1

```




```input2
2 2 4
-1 0
1 2

```




```output1
10.0000000000

```




```output2
23.3333333333

```



## Note

<p>The second sample test is shown on the figure. Green area is the desired area of the illuminated part of the floor. Violet segments indicate windows.</p>
