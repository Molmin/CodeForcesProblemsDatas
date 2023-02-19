## Description

<div><p>Dasha logged into the system and began to solve problems. One of them is as follows:</p><p>Given two sequences <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> of length <span class="tex-span"><i>n</i></span> each you need to write a sequence <span class="tex-span"><i>c</i></span> of length <span class="tex-span"><i>n</i></span>, the <span class="tex-span"><i>i</i></span>-th element of which is calculated as follows: <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i></sub> - <i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>About sequences <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> we know that their elements are in the range from <span class="tex-span"><i>l</i></span> to <span class="tex-span"><i>r</i></span>. More formally, elements satisfy the following conditions: <span class="tex-span"><i>l</i> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i></span> and <span class="tex-span"><i>l</i> ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i></span>. About sequence <span class="tex-span"><i>c</i></span> we know that all its elements are distinct.</p><center> <img class="tex-graphics" src="file://TXsUjvXL.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Dasha wrote a solution to that problem quickly, but checking her work on the standard test was not so easy. Due to an error in the test system only the sequence <span class="tex-span"><i>a</i></span> and the <span class="tex-font-style-it">compressed sequence</span> of the sequence <span class="tex-span"><i>c</i></span> were known from that test.</p><p>Let's give the definition to a <span class="tex-font-style-it">compressed sequence</span>. A <span class="tex-font-style-it">compressed sequence</span> of sequence <span class="tex-span"><i>c</i></span> of length <span class="tex-span"><i>n</i></span> is a sequence <span class="tex-span"><i>p</i></span> of length <span class="tex-span"><i>n</i></span>, so that <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> equals to the number of integers which are less than or equal to <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> in the sequence <span class="tex-span"><i>c</i></span>. For example, for the sequence <span class="tex-span"><i>c</i> = [250, 200, 300, 100, 50]</span> the compressed sequence will be <span class="tex-span"><i>p</i> = [4, 3, 5, 2, 1]</span>. Pay attention that in <span class="tex-span"><i>c</i></span> all integers are distinct. Consequently, the <span class="tex-font-style-it">compressed sequence</span> contains all integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> inclusively.</p><p>Help Dasha to find any sequence <span class="tex-span"><i>b</i></span> for which the calculated <span class="tex-font-style-it">compressed sequence</span> of sequence <span class="tex-span"><i>c</i></span> is correct.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the length of the sequence and boundaries of the segment where the elements of sequences <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>,  <i>a</i><sub class="lower-index">2</sub>,  ...,  <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(<i>l</i> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i>)</span> — the elements of the sequence <span class="tex-span"><i>a</i></span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,  <i>p</i><sub class="lower-index">2</sub>,  ...,  <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the <span class="tex-font-style-it">compressed sequence</span> of the sequence <span class="tex-span"><i>c</i></span>.</p></div><div class="output-specification"><p>If there is no the suitable sequence <span class="tex-span"><i>b</i></span>, then in the only line print "<span class="tex-font-style-tt">-1</span>".</p><p>Otherwise, in the only line print <span class="tex-span"><i>n</i></span> integers — the elements of any suitable sequence <span class="tex-span"><i>b</i></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>r</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>, 1 ≤ <i>l</i> ≤ <i>r</i> ≤ 10<sup class="upper-index">9</sup>)</span> — the length of the sequence and boundaries of the segment where the elements of sequences <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are.</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>,  <i>a</i><sub class="lower-index">2</sub>,  ...,  <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(<i>l</i> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i>)</span> — the elements of the sequence <span class="tex-span"><i>a</i></span>.</p><p>The next line contains <span class="tex-span"><i>n</i></span> distinct integers <span class="tex-span"><i>p</i><sub class="lower-index">1</sub>,  <i>p</i><sub class="lower-index">2</sub>,  ...,  <i>p</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i>)</span> — the <span class="tex-font-style-it">compressed sequence</span> of the sequence <span class="tex-span"><i>c</i></span>.</p>

## Output

<p>If there is no the suitable sequence <span class="tex-span"><i>b</i></span>, then in the only line print "<span class="tex-font-style-tt">-1</span>".</p><p>Otherwise, in the only line print <span class="tex-span"><i>n</i></span> integers — the elements of any suitable sequence <span class="tex-span"><i>b</i></span>.</p>





```input1
5 1 5
1 1 1 1 1
3 1 5 4 2

```




```input2
4 2 9
3 4 8 9
3 2 1 4

```




```input3
6 1 5
1 1 1 1 1 1
2 3 5 4 1 6

```




```output1
3 1 5 4 2
```




```output2
2 2 2 9
```




```output3
-1

```



## Note

<p>Sequence <span class="tex-span"><i>b</i></span> which was found in the second sample is suitable, because calculated sequence <span class="tex-span"><i>c</i> = [2 - 3, 2 - 4, 2 - 8, 9 - 9] = [ - 1,  - 2,  - 6, 0]</span> (note that <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub> = <i>b</i><sub class="lower-index"><i>i</i></sub> - <i>a</i><sub class="lower-index"><i>i</i></sub></span>) has compressed sequence equals to <span class="tex-span"><i>p</i> = [3, 2, 1, 4]</span>.</p>
