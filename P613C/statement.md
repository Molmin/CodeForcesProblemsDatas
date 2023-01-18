## Description

<div><p>Ivan wants to make a necklace as a present to his beloved girl. A <span class="tex-font-style-it">necklace</span> is a cyclic sequence of beads of different colors. Ivan says that necklace is <span class="tex-font-style-it">beautiful</span> relative to the cut point between two adjacent beads, if the chain of beads remaining after this cut is a palindrome (reads the same forward and backward).</p><center> <img class="tex-graphics" src="file://NIkKCSfn.png" style="max-width: 100.0%;max-height: 100.0%;" width="227px"> </center><p>Ivan has beads of <span class="tex-span"><i>n</i></span> colors. He wants to make a necklace, such that it's beautiful relative to as many cuts as possible. He certainly wants to use all the beads. Help him to make the most beautiful necklace.</p></div><div class="input-specification"><p>The first line of the input contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 26</span>) — the number of colors of beads. The second line contains after <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> &nbsp; — the quantity of beads of <span class="tex-span"><i>i</i></span>-th color. It is guaranteed that the sum of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is at least 2 and does not exceed <span class="tex-span">100 000</span>.</p></div><div class="output-specification"><p>In the first line print a single number&nbsp;— the maximum number of beautiful cuts that a necklace composed from given beads may have. In the second line print any example of such necklace.</p><p>Each color of the beads should be represented by the corresponding lowercase English letter (starting with <span class="tex-font-style-tt">a</span>). As the necklace is cyclic, print it starting from any point.</p></div>

## Input

<p>The first line of the input contains a single number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 26</span>) — the number of colors of beads. The second line contains after <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> &nbsp; — the quantity of beads of <span class="tex-span"><i>i</i></span>-th color. It is guaranteed that the sum of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is at least 2 and does not exceed <span class="tex-span">100 000</span>.</p>

## Output

<p>In the first line print a single number&nbsp;— the maximum number of beautiful cuts that a necklace composed from given beads may have. In the second line print any example of such necklace.</p><p>Each color of the beads should be represented by the corresponding lowercase English letter (starting with <span class="tex-font-style-tt">a</span>). As the necklace is cyclic, print it starting from any point.</p>





```input1
3
4 2 1

```




```input2
1
4

```




```input3
2
1 1

```




```output1
1
abacaba
```




```output2
4
aaaa

```




```output3
0
ab

```



## Note

<p>In the first sample a necklace can have at most one beautiful cut. The example of such a necklace is shown on the picture.</p><p>In the second sample there is only one way to compose a necklace.</p>
