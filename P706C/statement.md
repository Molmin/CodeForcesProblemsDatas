## Description

<div><p>Vasiliy is fond of solving different tasks. Today he found one he wasn't able to solve himself, so he asks you to help.</p><p>Vasiliy is given <span class="tex-span"><i>n</i></span> strings consisting of lowercase English letters. He wants them to be sorted in lexicographical order (as in the dictionary), but he is not allowed to swap any of them. The only operation he is allowed to do is to reverse any of them (first character becomes last, second becomes one before last and so on).</p><p>To reverse the <span class="tex-span"><i>i</i></span>-th string Vasiliy has to spent <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> units of energy. He is interested in the minimum amount of energy he has to spent in order to have strings sorted in lexicographical order.</p><p>String <span class="tex-span"><i>A</i></span> is lexicographically smaller than string <span class="tex-span"><i>B</i></span> if it is shorter than <span class="tex-span"><i>B</i></span> (<span class="tex-span">|<i>A</i>| &lt; |<i>B</i>|</span>) and is its prefix, or if none of them is a prefix of the other and at the first position where they differ character in <span class="tex-span"><i>A</i></span> is smaller than the character in <span class="tex-span"><i>B</i></span>.</p><p>For the purpose of this problem, two equal strings nearby do not break the condition of sequence being sorted lexicographically.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of strings.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the <span class="tex-span"><i>i</i></span>-th of them is equal to the amount of energy Vasiliy has to spent in order to reverse the <span class="tex-span"><i>i</i></span>-th string. </p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each containing a string consisting of lowercase English letters. The total length of these strings doesn't exceed <span class="tex-span">100 000</span>.</p></div><div class="output-specification"><p>If it is impossible to reverse some of the strings such that they will be located in lexicographical order, print <span class="tex-span"> - 1</span>. Otherwise, print the minimum total amount of energy Vasiliy has to spent.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of strings.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the <span class="tex-span"><i>i</i></span>-th of them is equal to the amount of energy Vasiliy has to spent in order to reverse the <span class="tex-span"><i>i</i></span>-th string. </p><p>Then follow <span class="tex-span"><i>n</i></span> lines, each containing a string consisting of lowercase English letters. The total length of these strings doesn't exceed <span class="tex-span">100 000</span>.</p>

## Output

<p>If it is impossible to reverse some of the strings such that they will be located in lexicographical order, print <span class="tex-span"> - 1</span>. Otherwise, print the minimum total amount of energy Vasiliy has to spent.</p>





```input1
2
1 2
ba
ac

```




```input2
3
1 3 1
aa
ba
ac

```




```input3
2
5 5
bbb
aaa

```




```input4
2
3 3
aaa
aa

```




```output1
1

```




```output2
1

```




```output3
-1

```




```output4
-1

```



## Note

<p>In the second sample one has to reverse string <span class="tex-span">2</span> or string <span class="tex-span">3</span>. To amount of energy required to reverse the string <span class="tex-span">3</span> is smaller.</p><p>In the third sample, both strings do not change after reverse and they go in the wrong order, so the answer is <span class="tex-span"> - 1</span>.</p><p>In the fourth sample, both strings consists of characters '<span class="tex-font-style-tt">a</span>' only, but in the sorted order string "<span class="tex-font-style-tt">aa</span>" should go before string "<span class="tex-font-style-tt">aaa</span>", thus the answer is <span class="tex-span"> - 1</span>.</p>
