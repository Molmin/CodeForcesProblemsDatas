## Description

<div><p>Today Sonya learned about long integers and invited all her friends to share the fun. Sonya has an initially empty multiset with integers. Friends give her <span class="tex-span"><i>t</i></span> queries, each of one of the following type:</p><ol> <li> <span class="tex-span"> + </span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— add non-negative integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to the multiset. Note, that she has a multiset, thus there may be many occurrences of the same integer. </li><li> <span class="tex-span"> - </span> <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— delete a single occurrence of non-negative integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> from the multiset. It's guaranteed, that there is at least one <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> in the multiset. </li><li> <span class="tex-span">?</span> <span class="tex-span"><i>s</i></span>&nbsp;— count the number of integers in the multiset (with repetitions) that match some pattern <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span">0</span> and <span class="tex-span">1</span>. In the pattern, <span class="tex-span">0</span> stands for the even digits, while <span class="tex-span">1</span> stands for the odd. Integer <span class="tex-span"><i>x</i></span> matches the pattern <span class="tex-span"><i>s</i></span>, if the parity of the <span class="tex-span"><i>i</i></span>-th from the right digit in decimal notation matches the <span class="tex-span"><i>i</i></span>-th from the right digit of the pattern. If the pattern is shorter than this integer, it's supplemented with <span class="tex-span">0</span>-s from the left. Similarly, if the integer is shorter than the pattern its decimal notation is supplemented with the <span class="tex-span">0</span>-s from the left. </li></ol><p>For example, if the pattern is <span class="tex-span"><i>s</i> = 010</span>, than integers <span class="tex-span">92</span>, <span class="tex-span">2212</span>, <span class="tex-span">50</span> and <span class="tex-span">414</span> match the pattern, while integers <span class="tex-span">3</span>, <span class="tex-span">110</span>, <span class="tex-span">25</span> and <span class="tex-span">1030</span> do not.</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100 000</span>)&nbsp;— the number of operation Sonya has to perform.</p><p>Next <span class="tex-span"><i>t</i></span> lines provide the descriptions of the queries in order they appear in the input file. The <span class="tex-span"><i>i</i></span>-th row starts with a character <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the type of the corresponding operation. If <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is equal to '<span class="tex-font-style-tt">+</span>' or '<span class="tex-font-style-tt">-</span>' then it's followed by a space and an integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">18</sup></span>) given without leading zeroes (unless it's <span class="tex-font-style-tt">0</span>). If <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals '<span class="tex-font-style-tt">?</span>' then it's followed by a space and a sequence of zeroes and onse, giving the pattern of length no more than <span class="tex-span">18</span>.</p><p>It's guaranteed that there will be at least one query of type '<span class="tex-font-style-tt">?</span>'.</p><p>It's guaranteed that any time some integer is removed from the multiset, there will be at least one occurrence of this integer in it.</p></div><div class="output-specification"><p>For each query of the third type print the number of integers matching the given pattern. Each integer is counted as many times, as it appears in the multiset at this moment of time.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 100 000</span>)&nbsp;— the number of operation Sonya has to perform.</p><p>Next <span class="tex-span"><i>t</i></span> lines provide the descriptions of the queries in order they appear in the input file. The <span class="tex-span"><i>i</i></span>-th row starts with a character <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— the type of the corresponding operation. If <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is equal to '<span class="tex-font-style-tt">+</span>' or '<span class="tex-font-style-tt">-</span>' then it's followed by a space and an integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; 10<sup class="upper-index">18</sup></span>) given without leading zeroes (unless it's <span class="tex-font-style-tt">0</span>). If <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> equals '<span class="tex-font-style-tt">?</span>' then it's followed by a space and a sequence of zeroes and onse, giving the pattern of length no more than <span class="tex-span">18</span>.</p><p>It's guaranteed that there will be at least one query of type '<span class="tex-font-style-tt">?</span>'.</p><p>It's guaranteed that any time some integer is removed from the multiset, there will be at least one occurrence of this integer in it.</p>

## Output

<p>For each query of the third type print the number of integers matching the given pattern. Each integer is counted as many times, as it appears in the multiset at this moment of time.</p>





```input1
12
+ 1
+ 241
? 1
+ 361
- 241
? 0101
+ 101
? 101
- 101
? 101
+ 4000
? 0

```




```input2
4
+ 200
+ 200
- 200
? 0

```




```output1
2
1
2
1
1

```




```output2
1

```



## Note

<p>Consider the integers matching the patterns from the queries of the third type. Queries are numbered in the order they appear in the input. </p><ol> <li> <span class="tex-span">1</span> and <span class="tex-span">241</span>. </li><li> <span class="tex-span">361</span>. </li><li> <span class="tex-span">101</span> and <span class="tex-span">361</span>. </li><li> <span class="tex-span">361</span>. </li><li> <span class="tex-span">4000</span>. </li></ol>
