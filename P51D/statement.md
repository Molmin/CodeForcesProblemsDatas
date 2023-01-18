## Description

<div><p>Polycarp loves geometric progressions — he collects them. However, as such progressions occur very rarely, he also loves the sequences of numbers where it is enough to delete a single element to get a geometric progression.</p><p>In this task we shall define geometric progressions as finite sequences of numbers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = <i>c</i>·<i>b</i><sup class="upper-index"><i>i</i> - 1</sup></span> for some real numbers <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>b</i></span>. For example, the sequences [2, -4, 8], [0, 0, 0, 0], [199] are geometric progressions and [0, 1, 2, 3] is not.</p><p>Recently Polycarp has found a sequence and he can't classify it. Help him to do it. Determine whether it is a geometric progression. If it is not, check if it can become a geometric progression if an element is deleted from it.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of elements in the given sequence. The second line contains the given sequence. The numbers are space-separated. All the elements of the given sequence are integers and their absolute value does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">0</span>, if the given sequence is a geometric progression. Otherwise, check if it is possible to make the sequence a geometric progression by deleting a single element. If it is possible, print <span class="tex-font-style-tt">1</span>. If it is impossible, print <span class="tex-font-style-tt">2</span>.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of elements in the given sequence. The second line contains the given sequence. The numbers are space-separated. All the elements of the given sequence are integers and their absolute value does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span>.</p>

## Output

<p>Print <span class="tex-font-style-tt">0</span>, if the given sequence is a geometric progression. Otherwise, check if it is possible to make the sequence a geometric progression by deleting a single element. If it is possible, print <span class="tex-font-style-tt">1</span>. If it is impossible, print <span class="tex-font-style-tt">2</span>.</p>





```input1
4
3 6 12 24

```




```input2
4
-8 -16 24 -32

```




```input3
4
0 1 2 3

```




```output1
0

```




```output2
1

```




```output3
2

```


