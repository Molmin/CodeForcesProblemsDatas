## Description

<div><p>There are <span class="tex-span"><i>n</i></span> pearls in a row. Let's enumerate them with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from the left to the right. The pearl number <span class="tex-span"><i>i</i></span> has the type <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Let's call a sequence of consecutive pearls a <span class="tex-font-style-tt">segment</span>. Let's call a segment <span class="tex-font-style-tt">good</span> if it contains two pearls of the same type.</p><p>Split the row of the pearls to the maximal number of good segments. Note that each pearl should appear in exactly one segment of the partition.</p><p>As input/output can reach huge size it is recommended to use fast input/output methods: for example, prefer to use <span class="tex-font-style-tt">scanf/printf</span> instead of <span class="tex-font-style-tt">cin/cout</span> in C++, prefer to use <span class="tex-font-style-tt">BufferedReader/PrintWriter</span> instead of <span class="tex-font-style-tt">Scanner/System.out</span> in <span class="tex-font-style-tt">Java</span>.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of pearls in a row.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) – the type of the <span class="tex-span"><i>i</i></span>-th pearl.</p></div><div class="output-specification"><p>On the first line print integer <span class="tex-span"><i>k</i></span> — the maximal number of segments in a partition of the row.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines should contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the number of the leftmost and the rightmost pearls in the <span class="tex-span"><i>j</i></span>-th segment.</p><p>Note you should print the correct partition of the row of the pearls, so each pearl should be in exactly one segment and all segments should contain two pearls of the same type.</p><p>If there are several optimal solutions print any of them. You can print the segments in any order.</p><p>If there are no correct partitions of the row print the number "<span class="tex-font-style-tt">-1</span>".</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) — the number of pearls in a row.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) – the type of the <span class="tex-span"><i>i</i></span>-th pearl.</p>

## Output

<p>On the first line print integer <span class="tex-span"><i>k</i></span> — the maximal number of segments in a partition of the row.</p><p>Each of the next <span class="tex-span"><i>k</i></span> lines should contain two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>j</i></sub>, <i>r</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>j</i></sub> ≤ <i>r</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the number of the leftmost and the rightmost pearls in the <span class="tex-span"><i>j</i></span>-th segment.</p><p>Note you should print the correct partition of the row of the pearls, so each pearl should be in exactly one segment and all segments should contain two pearls of the same type.</p><p>If there are several optimal solutions print any of them. You can print the segments in any order.</p><p>If there are no correct partitions of the row print the number "<span class="tex-font-style-tt">-1</span>".</p>





```input1
5
1 2 3 4 1

```




```input2
5
1 2 3 4 5

```




```input3
7
1 2 1 3 1 2 1

```




```output1
1
1 5

```




```output2
-1

```




```output3
2
1 3
4 7

```


