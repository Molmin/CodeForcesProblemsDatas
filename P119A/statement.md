## Description

<div><p>Simon and Antisimon play a game. Initially each player receives one fixed positive integer that doesn't change throughout the game. Simon receives number <span class="tex-span"><i>a</i></span> and Antisimon receives number <span class="tex-span"><i>b</i></span>. They also have a heap of <span class="tex-span"><i>n</i></span> stones. The players take turns to make a move and Simon starts. During a move a player should take from the heap the number of stones equal to the greatest common divisor of the fixed number he has received and the number of stones left in the heap. A player loses when he cannot take the required number of stones (i. e. the heap has <span class="tex-font-style-underline">strictly</span> less stones left than one needs to take). </p><p>Your task is to determine by the given <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>n</i></span> who wins the game.</p></div><div class="input-specification"><p>The only string contains space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>n</i> ≤ 100</span>) — the fixed numbers Simon and Antisimon have received correspondingly and the initial number of stones in the pile.</p></div><div class="output-specification"><p>If Simon wins, print "<span class="tex-font-style-tt">0</span>" (without the quotes), otherwise print "<span class="tex-font-style-tt">1</span>" (without the quotes).</p></div>

## Input

<p>The only string contains space-separated integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>n</i> ≤ 100</span>) — the fixed numbers Simon and Antisimon have received correspondingly and the initial number of stones in the pile.</p>

## Output

<p>If Simon wins, print "<span class="tex-font-style-tt">0</span>" (without the quotes), otherwise print "<span class="tex-font-style-tt">1</span>" (without the quotes).</p>





```input1
3 5 9

```




```input2
1 1 100

```




```output1
0
```




```output2
1
```



## Note

<p>The greatest common divisor of two non-negative integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> is such maximum positive integer <span class="tex-span"><i>k</i></span>, that <span class="tex-span"><i>a</i></span> is divisible by <span class="tex-span"><i>k</i></span> without remainder and similarly, <span class="tex-span"><i>b</i></span> is divisible by <span class="tex-span"><i>k</i></span> without remainder. Let <span class="tex-span"><i>gcd</i>(<i>a</i>, <i>b</i>)</span> represent the operation of calculating the greatest common divisor of numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. Specifically, <span class="tex-span"><i>gcd</i>(<i>x</i>, 0) = <i>gcd</i>(0, <i>x</i>) = <i>x</i></span>.</p><p>In the first sample the game will go like that:</p><ul><li> Simon should take <span class="tex-span"><i>gcd</i>(3, 9) = 3</span> stones from the heap. After his move the heap has <span class="tex-span">6</span> stones left.</li><li> Antisimon should take <span class="tex-span"><i>gcd</i>(5, 6) = 1</span> stone from the heap. After his move the heap has <span class="tex-span">5</span> stones left.</li><li> Simon should take <span class="tex-span"><i>gcd</i>(3, 5) = 1</span> stone from the heap. After his move the heap has <span class="tex-span">4</span> stones left.</li><li> Antisimon should take <span class="tex-span"><i>gcd</i>(5, 4) = 1</span> stone from the heap. After his move the heap has <span class="tex-span">3</span> stones left.</li><li> Simon should take <span class="tex-span"><i>gcd</i>(3, 3) = 3</span> stones from the heap. After his move the heap has <span class="tex-span">0</span> stones left.</li><li> Antisimon should take <span class="tex-span"><i>gcd</i>(5, 0) = 5</span> stones from the heap. As <span class="tex-span">0 &lt; 5</span>, it is impossible and Antisimon loses.</li></ul><p>In the second sample each player during each move takes one stone from the heap. As <span class="tex-span"><i>n</i></span> is even, Antisimon takes the last stone and Simon can't make a move after that.</p>
