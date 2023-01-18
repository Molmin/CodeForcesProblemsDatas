## Description

<div><p><span class="tex-font-style-it">And where the are the phone numbers?</span></p><p>You are given a string <span class="tex-span"><i>s</i></span> consisting of lowercase English letters and an integer <span class="tex-span"><i>k</i></span>. Find the lexicographically smallest string <span class="tex-span"><i>t</i></span> of length <span class="tex-span"><i>k</i></span>, such that its set of letters is a subset of the set of letters of <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>s</i></span> is lexicographically smaller than <span class="tex-span"><i>t</i></span>.</p><p>It's guaranteed that the answer exists.</p><p>Note that the set of letters is a set, not a multiset. For example, the set of letters of <span class="tex-font-style-tt">abadaba</span> is <span class="tex-span">{<i>a</i>, <i>b</i>, <i>d</i>}</span>.</p><p>String <span class="tex-span"><i>p</i></span> is lexicographically smaller than string <span class="tex-span"><i>q</i></span>, if <span class="tex-span"><i>p</i></span> is a prefix of <span class="tex-span"><i>q</i></span>, is not equal to <span class="tex-span"><i>q</i></span> or there exists <span class="tex-span"><i>i</i></span>, such that <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>q</i><sub class="lower-index"><i>i</i></sub></span> and for all <span class="tex-span"><i>j</i> &lt; <i>i</i></span> it is satisfied that <span class="tex-span"><i>p</i><sub class="lower-index"><i>j</i></sub> = <i>q</i><sub class="lower-index"><i>j</i></sub></span>. For example, <span class="tex-font-style-tt">abc</span> is lexicographically smaller than <span class="tex-font-style-tt">abcd</span> , <span class="tex-font-style-tt">abd</span> is lexicographically smaller than <span class="tex-font-style-tt">abec</span>, <span class="tex-font-style-tt">afa</span> <span class="tex-font-style-bf">is not</span> lexicographically smaller than <span class="tex-font-style-tt">ab</span> and <span class="tex-font-style-tt">a</span> <span class="tex-font-style-bf">is not</span> lexicographically smaller than <span class="tex-font-style-tt">a</span>.</p></div><div class="input-specification"><p>The first line of input contains two space separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100 000</span>)&nbsp;— the length of <span class="tex-span"><i>s</i></span> and the required length of <span class="tex-span"><i>t</i></span>.</p><p>The second line of input contains the string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase English letters.</p></div><div class="output-specification"><p>Output the string <span class="tex-span"><i>t</i></span> conforming to the requirements above.</p><p>It's guaranteed that the answer exists.</p></div>

## Input

<p>The first line of input contains two space separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 100 000</span>)&nbsp;— the length of <span class="tex-span"><i>s</i></span> and the required length of <span class="tex-span"><i>t</i></span>.</p><p>The second line of input contains the string <span class="tex-span"><i>s</i></span> consisting of <span class="tex-span"><i>n</i></span> lowercase English letters.</p>

## Output

<p>Output the string <span class="tex-span"><i>t</i></span> conforming to the requirements above.</p><p>It's guaranteed that the answer exists.</p>





```input1
3 3
abc

```




```input2
3 2
abc

```




```input3
3 3
ayy

```




```input4
2 3
ba

```




```output1
aca

```




```output2
ac

```




```output3
yaa

```




```output4
baa

```



## Note

<p>In the first example the list of strings <span class="tex-span"><i>t</i></span> of length 3, such that the set of letters of <span class="tex-span"><i>t</i></span> is a subset of letters of <span class="tex-span"><i>s</i></span> is as follows: <span class="tex-font-style-tt">aaa</span>, <span class="tex-font-style-tt">aab</span>, <span class="tex-font-style-tt">aac</span>, <span class="tex-font-style-tt">aba</span>, <span class="tex-font-style-tt">abb</span>, <span class="tex-font-style-tt">abc</span>, <span class="tex-font-style-tt">aca</span>, <span class="tex-font-style-tt">acb</span>, <span class="tex-span">...</span>. Among them, those are lexicographically greater than <span class="tex-font-style-tt">abc</span>: <span class="tex-font-style-tt">aca</span>, <span class="tex-font-style-tt">acb</span>, <span class="tex-span">...</span>. Out of those the lexicographically smallest is <span class="tex-font-style-tt">aca</span>.</p>
