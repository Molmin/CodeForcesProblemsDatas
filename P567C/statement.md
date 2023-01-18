## Description

<div><p>Polycarp loves geometric progressions very much. Since he was only three years old, he loves only the progressions of length three. He also has a favorite integer <span class="tex-span"><i>k</i></span> and a sequence <span class="tex-span"><i>a</i></span>, consisting of <span class="tex-span"><i>n</i></span> integers.</p><p>He wants to know how many subsequences of length three can be selected from <span class="tex-span"><i>a</i></span>, so that they form a geometric progression with common ratio <span class="tex-span"><i>k</i></span>.</p><p>A subsequence of length three is a combination of three such indexes <span class="tex-span"><i>i</i><sub class="lower-index">1</sub>, <i>i</i><sub class="lower-index">2</sub>, <i>i</i><sub class="lower-index">3</sub></span>, that <span class="tex-span">1 ≤ <i>i</i><sub class="lower-index">1</sub> &lt; <i>i</i><sub class="lower-index">2</sub> &lt; <i>i</i><sub class="lower-index">3</sub> ≤ <i>n</i></span>. That is, a subsequence of length three are such groups of three elements that are not necessarily consecutive in the sequence, but their indexes are strictly increasing.</p><p>A geometric progression with common ratio <span class="tex-span"><i>k</i></span> is a sequence of numbers of the form <span class="tex-span"><i>b</i>·<i>k</i><sup class="upper-index">0</sup>, <i>b</i>·<i>k</i><sup class="upper-index">1</sup>, ..., <i>b</i>·<i>k</i><sup class="upper-index"><i>r</i> - 1</sup></span>.</p><p>Polycarp is only three years old, so he can not calculate this number himself. Help him to do it.</p></div><div class="input-specification"><p>The first line of the input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 2·10<sup class="upper-index">5</sup></span>), showing how many numbers Polycarp's sequence has and his favorite number.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — elements of the sequence.</p></div><div class="output-specification"><p>Output a single number — the number of ways to choose a subsequence of length three, such that it forms a geometric progression with a common ratio <span class="tex-span"><i>k</i></span>.</p></div>

## Input

<p>The first line of the input contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 2·10<sup class="upper-index">5</sup></span>), showing how many numbers Polycarp's sequence has and his favorite number.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — elements of the sequence.</p>

## Output

<p>Output a single number — the number of ways to choose a subsequence of length three, such that it forms a geometric progression with a common ratio <span class="tex-span"><i>k</i></span>.</p>





```input1
5 2
1 1 2 2 4

```




```input2
3 1
1 1 1

```




```input3
10 3
1 2 6 2 3 6 9 18 3 9

```




```output1
4
```




```output2
1
```




```output3
6
```



## Note

<p>In the first sample test the answer is four, as any of the two 1s can be chosen as the first element, the second element can be any of the 2s, and the third element of the subsequence must be equal to 4.</p>
