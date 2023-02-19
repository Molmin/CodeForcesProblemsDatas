## Description

<div><p>A robot is standing at the origin of the infinite two-dimensional plane. Each second the robot moves exactly $1$ meter in one of the four cardinal directions: north, south, west, and east. For the first step the robot <span class="tex-font-style-bf">can choose any of the four directions</span>, but then at the end of every second it <span class="tex-font-style-bf">has to turn</span> 90 degrees left or right with respect to the direction it just moved in. For example, if the robot has just moved north or south, the next step it takes has to be either west or east, and vice versa.</p><p>The robot makes <span class="tex-font-style-bf">exactly</span> $n$ steps from its starting position according to the rules above. How many different points can the robot arrive to at the end? The final orientation of the robot can be ignored.</p></div><div class="input-specification"><p>The only line contains a single integer $n$ ($1 \leq n \leq 1000$)&nbsp;— the number of steps the robot makes.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of different possible locations after <span class="tex-font-style-bf">exactly</span> $n$ steps.</p></div>

## Input

<p>The only line contains a single integer $n$ ($1 \leq n \leq 1000$)&nbsp;— the number of steps the robot makes.</p>

## Output

<p>Print a single integer&nbsp;— the number of different possible locations after <span class="tex-font-style-bf">exactly</span> $n$ steps.</p>





```input1
1
```




```input2
2
```




```input3
3
```




```output1
4
```




```output2
4
```




```output3
12
```



## Note

<p>In the first sample case, the robot will end up 1 meter north, south, west, or east depending on its initial direction.</p><p>In the second sample case, the robot will always end up $\sqrt{2}$ meters north-west, north-east, south-west, or south-east.</p>
