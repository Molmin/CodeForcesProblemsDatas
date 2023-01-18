## Description

<div><p>Winter is here at the North and the White Walkers are close. John Snow has an army consisting of <span class="tex-span"><i>n</i></span> soldiers. While the rest of the world is fighting for the Iron Throne, he is going to get ready for the attack of the White Walkers.</p><p>He has created a method to know how strong his army is. Let the <span class="tex-span"><i>i</i></span>-th soldier’s strength be <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. For some <span class="tex-span"><i>k</i></span> he calls <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, ..., <i>i</i><sub class="lower-index"><i>k</i></sub></span> a clan if <span class="tex-span"><i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; <i>i</i><sub class="lower-index">3</sub> &lt; ... &lt; <i>i</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>gcd</i>(<i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub>, <i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">2</sub></sub>, ..., <i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>k</i></sub></sub>) &gt; 1</span> . He calls the strength of that clan <span class="tex-span"><i>k</i>·<i>gcd</i>(<i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">1</sub></sub>, <i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index">2</sub></sub>, ..., <i>a</i><sub class="lower-index"><i>i</i><sub class="lower-index"><i>k</i></sub></sub>)</span>. Then he defines the strength of his army by the sum of strengths of all possible clans.</p><p>Your task is to find the strength of his army. As the number may be very large, you have to print it modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p><p>Greatest common divisor (gcd) of a sequence of integers is the maximum possible integer so that each element of the sequence is divisible by it.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>)&nbsp;— the size of the army.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000000</span>)&nbsp;— denoting the strengths of his soldiers.</p></div><div class="output-specification"><p>Print one integer&nbsp;— the strength of John Snow's army modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200000</span>)&nbsp;— the size of the army.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 1000000</span>)&nbsp;— denoting the strengths of his soldiers.</p>

## Output

<p>Print one integer&nbsp;— the strength of John Snow's army modulo <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
3
3 3 1

```




```input2
4
2 3 4 6

```




```output1
12

```




```output2
39

```



## Note

<p>In the first sample the clans are <span class="tex-span">{1}, {2}, {1, 2}</span> so the answer will be <span class="tex-span">1·3 + 1·3 + 2·3 = 12</span></p>
