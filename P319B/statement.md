## Description

<div><p>There are <span class="tex-span"><i>n</i></span> psychos standing in a line. Each psycho is assigned a unique integer from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. At each step every psycho who has an id greater than the psycho to his right (if exists) kills his right neighbor in the line. Note that a psycho might kill and get killed at the same step. </p><p>You're given the initial arrangement of the psychos in the line. Calculate how many steps are needed to the moment of time such, that nobody kills his neighbor after that moment. Look notes to understand the statement more precise.</p></div><div class="input-specification"><p>The first line of input contains integer <span class="tex-span"><i>n</i></span> denoting the number of psychos, <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. In the second line there will be a list of <span class="tex-span"><i>n</i></span> space separated distinct integers each in range <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive — ids of the psychos in the line from left to right.</p></div><div class="output-specification"><p>Print the number of steps, so that the line remains the same afterward.</p></div>

## Input

<p>The first line of input contains integer <span class="tex-span"><i>n</i></span> denoting the number of psychos, <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>. In the second line there will be a list of <span class="tex-span"><i>n</i></span> space separated distinct integers each in range <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, inclusive — ids of the psychos in the line from left to right.</p>

## Output

<p>Print the number of steps, so that the line remains the same afterward.</p>





```input1
10
10 9 7 8 6 5 3 4 2 1

```




```input2
6
1 2 3 4 5 6

```




```output1
2

```




```output2
0

```



## Note

<p>In the first sample line of the psychos transforms as follows: [10 9 7 8 6 5 3 4 2 1] <span class="tex-span"> → </span> <span class="tex-font-style-bf">[10 8 4]</span> <span class="tex-span"> → </span> [10]. So, there are two steps.</p>
