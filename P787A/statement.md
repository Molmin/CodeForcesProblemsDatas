## Description

<div><p>A monster is chasing after Rick and Morty on another planet. They're so frightened that sometimes they scream. More accurately, Rick screams at times <span class="tex-span"><i>b</i>, <i>b</i> + <i>a</i>, <i>b</i> + 2<i>a</i>, <i>b</i> + 3<i>a</i>, ...</span> and Morty screams at times <span class="tex-span"><i>d</i>, <i>d</i> + <i>c</i>, <i>d</i> + 2<i>c</i>, <i>d</i> + 3<i>c</i>, ...</span>. </p><center> <img class="tex-graphics" src="file://qSSX6MuO.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The Monster will catch them if at any point they scream at the same time, so it wants to know when it will catch them (the first time they scream at the same time) or that they will never scream at the same time.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 100</span>). </p><p>The second line contains two integers <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>c</i>, <i>d</i> ≤ 100</span>).</p></div><div class="output-specification"><p>Print the first time Rick and Morty will scream at the same time, or <span class="tex-span"> - 1</span> if they will never scream at the same time.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ 100</span>). </p><p>The second line contains two integers <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">1 ≤ <i>c</i>, <i>d</i> ≤ 100</span>).</p>

## Output

<p>Print the first time Rick and Morty will scream at the same time, or <span class="tex-span"> - 1</span> if they will never scream at the same time.</p>





```input1
20 2
9 19

```




```input2
2 1
16 12

```




```output1
82

```




```output2
-1

```



## Note

<p>In the first sample testcase, Rick's <span class="tex-span">5</span>th scream and Morty's <span class="tex-span">8</span>th time are at time <span class="tex-span">82</span>. </p><p>In the second sample testcase, all Rick's screams will be at odd times and Morty's will be at even times, so they will never scream at the same time.</p>
