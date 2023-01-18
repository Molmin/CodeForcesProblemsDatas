## Description

<div><p>Vasya collects coins: he has exactly one coin for every year from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. Naturally, Vasya keeps all the coins in his collection in the order in which they were released. Once Vasya's younger brother made a change — he took all the coins whose release year dated from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span> inclusively and put them in the reverse order. That is, he took a certain segment <span class="tex-span">[<i>l</i>, <i>r</i>]</span> and reversed it. At that the segment's endpoints did not coincide. For example, if <span class="tex-span"><i>n</i> = 8</span>, then initially Vasya's coins were kept in the order <span class="tex-font-style-tt">1 2 3 4 5 6 7 8</span>. If Vasya's younger brother chose the segment <span class="tex-span">[2, 6]</span>, then after the reversal the coin order will change to <span class="tex-font-style-tt">1 6 5 4 3 2 7 8</span>. Vasya suspects that someone else could have spoilt the permutation after his brother. Help him to find that out. Check if the given permutation can be obtained from the permutation <span class="tex-font-style-tt">1 2 ... <span class="tex-span"><i>n</i></span></span> using exactly one segment reversal. If it is possible, find the segment itself.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) which is the number of coins in Vasya's collection. The second line contains space-separated <span class="tex-span"><i>n</i></span> integers which are the spoilt sequence of coins. It is guaranteed that the given sequence is a permutation, i.e. it contains only integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and every number is used exactly 1 time.</p></div><div class="output-specification"><p>If it is impossible to obtain the given permutation from the original one in exactly one action, print <span class="tex-font-style-tt">0 0</span>. Otherwise, print two numbers <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> &lt; <i>r</i> ≤ <i>n</i></span>) which are the endpoints of the segment that needs to be reversed to obtain from permutation <span class="tex-font-style-tt">1 2 ... <span class="tex-span"><i>n</i></span></span> the given one.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) which is the number of coins in Vasya's collection. The second line contains space-separated <span class="tex-span"><i>n</i></span> integers which are the spoilt sequence of coins. It is guaranteed that the given sequence is a permutation, i.e. it contains only integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, and every number is used exactly 1 time.</p>

## Output

<p>If it is impossible to obtain the given permutation from the original one in exactly one action, print <span class="tex-font-style-tt">0 0</span>. Otherwise, print two numbers <span class="tex-span"><i>l</i></span> <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>l</i> &lt; <i>r</i> ≤ <i>n</i></span>) which are the endpoints of the segment that needs to be reversed to obtain from permutation <span class="tex-font-style-tt">1 2 ... <span class="tex-span"><i>n</i></span></span> the given one.</p>





```input1
8
1 6 5 4 3 2 7 8

```




```input2
4
2 3 4 1

```




```input3
4
1 2 3 4

```




```output1
2 6

```




```output2
0 0

```




```output3
0 0

```


