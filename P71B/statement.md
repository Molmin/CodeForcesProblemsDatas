## Description

<div><p>A progress bar is an element of graphical interface that displays the progress of a process for this very moment before it is completed. Let's take a look at the following form of such a bar.</p><p>A bar is represented as <span class="tex-span"><i>n</i></span> squares, located in line. To add clarity, let's number them with positive integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from the left to the right. Each square has saturation (<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> for the <span class="tex-span"><i>i</i></span>-th square), which is measured by an integer from <span class="tex-span">0</span> to <span class="tex-span"><i>k</i></span>. When the bar for some <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) is displayed, squares <span class="tex-span">1, 2, ... , <i>i</i> - 1</span> has the saturation <span class="tex-span"><i>k</i></span>, squares <span class="tex-span"><i>i</i> + 1, <i>i</i> + 2, ... , <i>n</i></span> has the saturation <span class="tex-span">0</span>, and the saturation of the square <span class="tex-span"><i>i</i></span> can have any value from <span class="tex-span">0</span> to <span class="tex-span"><i>k</i></span>.</p><p>So some first squares of the progress bar always have the saturation <span class="tex-span"><i>k</i></span>. Some last squares always have the saturation <span class="tex-span">0</span>. And there is no more than one square that has the saturation different from <span class="tex-span">0</span> and <span class="tex-span"><i>k</i></span>.</p><p>The degree of the process's completion is measured in percents. Let the process be <span class="tex-span"><i>t</i></span>% completed. Then the following inequation is fulfilled: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://6FqTiWBw.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>An example of such a bar can be seen on the picture.</p><center> <img class="tex-graphics" src="file://i8SEDRdF.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>For the given <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>t</i></span> determine the measures of saturation for all the squares <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> of the progress bar.</p></div><div class="input-specification"><p>We are given 3 space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>t</i> ≤ 100</span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> numbers. The <span class="tex-span"><i>i</i></span>-th of them should be equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p></div>

## Input

<p>We are given 3 space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100</span>, <span class="tex-span">0 ≤ <i>t</i> ≤ 100</span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> numbers. The <span class="tex-span"><i>i</i></span>-th of them should be equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p>





```input1
10 10 54

```




```input2
11 13 37

```




```output1
10 10 10 10 10 4 0 0 0 0
```




```output2
13 13 13 13 0 0 0 0 0 0 0
```


