## Description

<div><p>The Berland University is preparing to celebrate the 256-th anniversary of its founding! A specially appointed Vice Rector for the celebration prepares to decorate the campus. In the center of the campus <span class="tex-span"><i>n</i></span> ice sculptures were erected. The sculptures are arranged in a circle at equal distances from each other, so they form a regular <span class="tex-span"><i>n</i></span>-gon. They are numbered in clockwise order with numbers from 1 to <span class="tex-span"><i>n</i></span>.</p><p>The site of the University has already conducted a voting that estimated each sculpture's characteristic of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the degree of the sculpture's attractiveness. The values of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> can be positive, negative or zero.</p><p>When the university rector came to evaluate the work, he said that this might be not the perfect arrangement. He suggested to melt some of the sculptures so that: </p><ul> <li> the remaining sculptures form a regular polygon (the number of vertices should be between 3 and <span class="tex-span"><i>n</i></span>), </li><li> the sum of the <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> values of the remaining sculptures is maximized. </li></ul><p>Help the Vice Rector to analyze the criticism — find the maximum value of <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> sum which can be obtained in this way. It is allowed not to melt any sculptures at all. The sculptures can not be moved.</p></div><div class="input-specification"><p>The first input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 20000</span>) — the initial number of sculptures. The second line contains a sequence of integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the degree of the <span class="tex-span"><i>i</i></span>-th sculpture's attractiveness (<span class="tex-span"> - 1000 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>). The numbers on the line are separated by spaces.</p></div><div class="output-specification"><p>Print the required maximum sum of the sculptures' attractiveness.</p></div>

## Input

<p>The first input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 20000</span>) — the initial number of sculptures. The second line contains a sequence of integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> — the degree of the <span class="tex-span"><i>i</i></span>-th sculpture's attractiveness (<span class="tex-span"> - 1000 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>). The numbers on the line are separated by spaces.</p>

## Output

<p>Print the required maximum sum of the sculptures' attractiveness.</p>





```input1
8
1 2 -3 4 -5 5 2 3

```




```input2
6
1 -2 3 -4 5 -6

```




```input3
6
1 2 3 4 5 6

```




```output1
14

```




```output2
9

```




```output3
21

```



## Note

<p>In the first sample it is best to leave every second sculpture, that is, leave sculptures with attractivenesses: 2, 4, 5 и 3.</p>
