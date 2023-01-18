## Description

<div><p>Valera considers a number <span class="tex-font-style-it">beautiful</span>, if it equals <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span> or -<span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span> for some integer <span class="tex-span"><i>k</i></span> <span class="tex-span">(<i>k</i> ≥ 0)</span>. Recently, the math teacher asked Valera to represent number <span class="tex-span"><i>n</i></span> as the sum of beautiful numbers. As Valera is really greedy, he wants to complete the task using as few beautiful numbers as possible. </p><p>Help Valera and find, how many numbers he is going to need. In other words, if you look at all decompositions of the number <span class="tex-span"><i>n</i></span> into beautiful summands, you need to find the size of the decomposition which has the fewest summands.</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup>)</span>, that is the binary representation of number <span class="tex-span"><i>n</i></span> without leading zeroes <span class="tex-span">(<i>n</i> &gt; 0)</span>.</p></div><div class="output-specification"><p>Print a single integer — the minimum amount of beautiful numbers that give a total of <span class="tex-span"><i>n</i></span>.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span> <span class="tex-span">(1 ≤ |<i>s</i>| ≤ 10<sup class="upper-index">6</sup>)</span>, that is the binary representation of number <span class="tex-span"><i>n</i></span> without leading zeroes <span class="tex-span">(<i>n</i> &gt; 0)</span>.</p>

## Output

<p>Print a single integer — the minimum amount of beautiful numbers that give a total of <span class="tex-span"><i>n</i></span>.</p>





```input1
10

```




```input2
111

```




```input3
1101101

```




```output1
1

```




```output2
2

```




```output3
4

```



## Note

<p>In the first sample <span class="tex-span"><i>n</i> = 2</span> is a beautiful number.</p><p>In the second sample <span class="tex-span"><i>n</i> = 7</span> and Valera can decompose it into sum <span class="tex-span">2<sup class="upper-index">3</sup> + ( - 2<sup class="upper-index">0</sup>)</span>.</p><p>In the third sample <span class="tex-span"><i>n</i> = 109</span> can be decomposed into the sum of four summands as follows: <span class="tex-span">2<sup class="upper-index">7</sup> + ( - 2<sup class="upper-index">4</sup>) + ( - 2<sup class="upper-index">2</sup>) + 2<sup class="upper-index">0</sup></span>.</p>
