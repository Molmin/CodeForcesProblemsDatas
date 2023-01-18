## Description

<div><p>Arkady likes to walk around his kitchen. His labyrinthine kitchen consists of several important places connected with passages. Unfortunately it happens that these passages are flooded with milk so that it's impossible to pass through them. Namely, it's possible to pass through each passage in any direction only during some time interval.</p><p>The lengths of all passages are equal and Arkady makes through them in one second. For security reasons, Arkady can never stop, also, he can't change direction while going through a passage. In other words, if he starts walking in some passage, he should reach its end and immediately leave the end.</p><p>Today Arkady needs to quickly reach important place <span class="tex-span"><i>n</i></span> from place <span class="tex-span">1</span>. He plans to exit the place <span class="tex-span">1</span> at time moment <span class="tex-span">0</span> and reach the place <span class="tex-span"><i>n</i></span> as early as he can. Please find the minimum time he should spend on his way.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of important places and the number of passages, respectively.</p><p>After that, <span class="tex-span"><i>m</i></span> lines follow, each of them describe one passage. Each line contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>, <span class="tex-span">0 ≤ <i>l</i> &lt; <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the places the passage connects and the time segment during which it's possible to use this passage.</p></div><div class="output-specification"><p>Print one integer&nbsp;— minimum time Arkady should spend to reach the destination. If he can't reach the place <span class="tex-span"><i>n</i></span>, print <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5·10<sup class="upper-index">5</sup></span>, <span class="tex-span">0 ≤ <i>m</i> ≤ 5·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of important places and the number of passages, respectively.</p><p>After that, <span class="tex-span"><i>m</i></span> lines follow, each of them describe one passage. Each line contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>, <span class="tex-span">0 ≤ <i>l</i> &lt; <i>r</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the places the passage connects and the time segment during which it's possible to use this passage.</p>

## Output

<p>Print one integer&nbsp;— minimum time Arkady should spend to reach the destination. If he can't reach the place <span class="tex-span"><i>n</i></span>, print <span class="tex-font-style-tt">-1</span>.</p>





```input1
5 6
1 2 0 1
2 5 2 3
2 5 0 1
1 3 0 1
3 4 1 2
4 5 2 3

```




```input2
2 1
1 2 1 100

```




```output1
3

```




```output2
-1

```



## Note

<p>In the first example Arkady should go through important places <span class="tex-span">1 → 3 → 4 → 5</span>.</p><p>In the second example Arkady can't start his walk because at time moment <span class="tex-span">0</span> it's impossible to use the only passage.</p>
