## Description

<div><p>After returning from the army Makes received a gift — an array <span class="tex-span"><i>a</i></span> consisting of <span class="tex-span"><i>n</i></span> positive integer numbers. He hadn't been solving problems for a long time, so he became interested to answer a particular question: how many triples of indices <span class="tex-span">(<i>i</i>, &nbsp;<i>j</i>, &nbsp;<i>k</i>)</span> (<span class="tex-span"><i>i</i> &lt; <i>j</i> &lt; <i>k</i></span>), such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>·<i>a</i><sub class="lower-index"><i>j</i></sub>·<i>a</i><sub class="lower-index"><i>k</i></sub></span> is minimum possible, are there in the array? Help him with it!</p></div><div class="input-specification"><p>The first line of input contains a positive integer number <span class="tex-span"><i>n</i>&nbsp;(3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of elements in array <span class="tex-span"><i>a</i></span>. The second line contains <span class="tex-span"><i>n</i></span> positive integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the elements of a given array.</p></div><div class="output-specification"><p>Print one number — the quantity of triples <span class="tex-span">(<i>i</i>, &nbsp;<i>j</i>, &nbsp;<i>k</i>)</span> such that <span class="tex-span"><i>i</i>, &nbsp;<i>j</i></span> and <span class="tex-span"><i>k</i></span> are pairwise distinct and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>·<i>a</i><sub class="lower-index"><i>j</i></sub>·<i>a</i><sub class="lower-index"><i>k</i></sub></span> is minimum possible.</p></div>

## Input

<p>The first line of input contains a positive integer number <span class="tex-span"><i>n</i>&nbsp;(3 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of elements in array <span class="tex-span"><i>a</i></span>. The second line contains <span class="tex-span"><i>n</i></span> positive integer numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>&nbsp;(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span> — the elements of a given array.</p>

## Output

<p>Print one number — the quantity of triples <span class="tex-span">(<i>i</i>, &nbsp;<i>j</i>, &nbsp;<i>k</i>)</span> such that <span class="tex-span"><i>i</i>, &nbsp;<i>j</i></span> and <span class="tex-span"><i>k</i></span> are pairwise distinct and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub>·<i>a</i><sub class="lower-index"><i>j</i></sub>·<i>a</i><sub class="lower-index"><i>k</i></sub></span> is minimum possible.</p>





```input1
4
1 1 1 1

```




```input2
5
1 3 2 3 4

```




```input3
6
1 3 3 1 3 2

```




```output1
4

```




```output2
2

```




```output3
1

```



## Note

<p>In the first example Makes always chooses three ones out of four, and the number of ways to choose them is <span class="tex-span">4</span>.</p><p>In the second example a triple of numbers <span class="tex-span">(1, 2, 3)</span> is chosen (numbers, not indices). Since there are two ways to choose an element <span class="tex-span">3</span>, then the answer is <span class="tex-span">2</span>.</p><p>In the third example a triple of numbers <span class="tex-span">(1, 1, 2)</span> is chosen, and there's only one way to choose indices.</p>
