## Description

<div><p>Imagine that you are in a building that has exactly <span class="tex-span"><i>n</i></span> floors. You can move between the floors in a lift. Let's number the floors from bottom to top with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Now you're on the floor number <span class="tex-span"><i>a</i></span>. You are very bored, so you want to take the lift. Floor number <span class="tex-span"><i>b</i></span> has a secret lab, the entry is forbidden. However, you already are in the mood and decide to make <span class="tex-span"><i>k</i></span> consecutive trips in the lift.</p><p>Let us suppose that at the moment you are on the floor number <span class="tex-span"><i>x</i></span> (initially, you were on floor <span class="tex-span"><i>a</i></span>). For another trip between floors you choose some floor with number <span class="tex-span"><i>y</i></span> (<span class="tex-span"><i>y</i> ≠ <i>x</i></span>) and the lift travels to this floor. As you cannot visit floor <span class="tex-span"><i>b</i></span> with the secret lab, you decided that the distance from the current floor <span class="tex-span"><i>x</i></span> to the chosen <span class="tex-span"><i>y</i></span> must be strictly less than the distance from the current floor <span class="tex-span"><i>x</i></span> to floor <span class="tex-span"><i>b</i></span> with the secret lab. Formally, it means that the following inequation must fulfill: <span class="tex-span">|<i>x</i> - <i>y</i>| &lt; |<i>x</i> - <i>b</i>|</span>. After the lift successfully transports you to floor <span class="tex-span"><i>y</i></span>, you write down number <span class="tex-span"><i>y</i></span> in your notepad.</p><p>Your task is to find the number of distinct number sequences that you could have written in the notebook as the result of <span class="tex-span"><i>k</i></span> trips in the lift. As the sought number of trips can be rather large, find the remainder after dividing the number by <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div><div class="input-specification"><p>The first line of the input contains four space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>).</p></div><div class="output-specification"><p>Print a single integer — the remainder after dividing the sought number of sequences by <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p></div>

## Input

<p>The first line of the input contains four space-separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>, <span class="tex-span"><i>a</i> ≠ <i>b</i></span>).</p>

## Output

<p>Print a single integer — the remainder after dividing the sought number of sequences by <span class="tex-span">1000000007</span> (<span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>).</p>





```input1
5 2 4 1

```




```input2
5 2 4 2

```




```input3
5 3 4 1

```




```output1
2

```




```output2
2

```




```output3
0

```



## Note

<p>Two sequences <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>, <i>p</i><sub class="lower-index">2</sub>, ..., <i>p</i><sub class="lower-index"><i>k</i></sub></span> and <span class="tex-span"><i>q</i><sub class="lower-index">1</sub>, <i>q</i><sub class="lower-index">2</sub>, ..., <i>q</i><sub class="lower-index"><i>k</i></sub></span> are <span class="tex-font-style-it">distinct</span>, if there is such integer <span class="tex-span"><i>j</i></span> (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>k</i></span>), that <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub> ≠ <i>q</i><sub class="lower-index"><i>j</i></sub></span>.</p><p><span class="tex-font-style-bf">Notes to the samples</span>:</p><ol> <li> In the first sample after the first trip you are either on floor <span class="tex-span">1</span>, or on floor <span class="tex-span">3</span>, because <span class="tex-span">|1 - 2| &lt; |2 - 4|</span> and <span class="tex-span">|3 - 2| &lt; |2 - 4|</span>. </li><li> In the second sample there are two possible sequences: <span class="tex-span">(1, 2)</span>; <span class="tex-span">(1, 3)</span>. You cannot choose floor <span class="tex-span">3</span> for the first trip because in this case no floor can be the floor for the second trip. </li><li> In the third sample there are no sought sequences, because you cannot choose the floor for the first trip. </li></ol>
