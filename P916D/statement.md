## Description

<div><p><span class="tex-font-style-it">Why I have to finish so many assignments???</span></p><p>Jamie is getting very busy with his school life. He starts to forget the assignments that he has to do. He decided to write the things down on a to-do list. He assigns a value <span class="tex-font-style-tt">priority</span> for each of his assignment <span class="tex-font-style-bf">(lower value means more important)</span> so he can decide which he needs to spend more time on.</p><p>After a few days, Jamie finds out the list is too large that he can't even manage the list by himself! As you are a good friend of Jamie, help him write a program to support the following operations on the to-do list:</p><ul> <li> <span class="tex-span"><i>set</i> <i>a</i><sub class="lower-index"><i>i</i></sub> <i>x</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— Add assignment <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> to the to-do list if it is not present, and set its <span class="tex-font-style-tt">priority</span> to <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. If assignment <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is already in the to-do list, its <span class="tex-font-style-tt">priority</span> <span class="tex-font-style-bf">is changed</span> to <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> <span class="tex-span"><i>remove</i> <i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— Remove assignment <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> from the to-do list if it is present in it. </li><li> <span class="tex-span"><i>query</i> <i>a</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— Output the number of assignments that are more important (have a <span class="tex-font-style-bf">smaller</span> <span class="tex-font-style-tt">priority</span> value) than assignment <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, so Jamie can decide a better schedule. Output <span class="tex-span"> - 1</span> if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is not in the to-do list. </li><li> <span class="tex-span"><i>undo</i> <i>d</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— Undo all changes that have been made in the previous <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> days (not including the day of this operation) </li></ul><p>At day <span class="tex-span">0</span>, the to-do list is empty. In each of the following <span class="tex-span"><i>q</i></span> days, Jamie will do <span class="tex-font-style-bf">exactly one</span> out of the four operations. If the operation is a <span class="tex-span"><i>query</i></span>, you should <span class="tex-font-style-bf">output the result of the query before proceeding to the next day</span>, or poor Jamie cannot make appropriate decisions.</p></div><div class="input-specification"><p>The first line consists of a single integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span>&nbsp;— the number of operations.</p><p>The following <span class="tex-span"><i>q</i></span> lines consists of the description of the operations. The <span class="tex-span"><i>i</i></span>-th line consists of the operation that Jamie has done in the <span class="tex-span"><i>i</i></span>-th day. The query has the following format:</p><p>The first word in the line indicates the type of operation. It must be one of the following four: <span class="tex-font-style-tt">set</span>, <span class="tex-font-style-tt">remove</span>, <span class="tex-font-style-tt">query</span>, <span class="tex-font-style-tt">undo</span>.</p><ul> <li> If it is a <span class="tex-font-style-tt">set</span> operation, a string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> follows <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the assignment that need to be set to <span class="tex-font-style-tt">priority</span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> If it is a <span class="tex-font-style-tt">remove</span> operation, a string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> follows. <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the assignment that need to be removed. </li><li> If it is a <span class="tex-font-style-tt">query</span> operation, a string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> follows. <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the assignment that needs to be queried. </li><li> If it is a <span class="tex-font-style-tt">undo</span> operation, an integer <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> follows <span class="tex-span">(0 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i>)</span>. <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the number of days that changes needed to be undone. </li></ul><p>All assignment names <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> only consists of lowercase English letters and have a length <span class="tex-span">1 ≤ |<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 15</span>.</p><p>It is guaranteed that the last operation is a <span class="tex-font-style-tt">query</span> operation.</p></div><div class="output-specification"><p>For each <span class="tex-font-style-tt">query</span> operation, output a single integer&nbsp;— the number of assignments that have a priority lower than assignment <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, or <span class="tex-span"> - 1</span> if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is not in the to-do list.</p></div><div><h2>Interaction</h2><p>If the operation is a <span class="tex-span"><i>query</i></span>, you <span class="tex-font-style-bf">should</span> output the result of the query and flush the output stream before proceeding to the next operation. Otherwise, you may get the verdict <span class="tex-font-style-tt">Idleness Limit Exceed</span>.</p><p>For flushing the output stream, please refer to the documentation of your chosen programming language. The flush functions of some common programming languages are listed below:</p><ul> <li> C: <span class="tex-font-style-tt">fflush(stdout);</span> </li><li> C++: <span class="tex-font-style-tt">cout « flush;</span> </li><li> Java: <span class="tex-font-style-tt">System.out.flush();</span> </li></ul></div>

## Input

<p>The first line consists of a single integer <span class="tex-span"><i>q</i></span> <span class="tex-span">(1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup>)</span>&nbsp;— the number of operations.</p><p>The following <span class="tex-span"><i>q</i></span> lines consists of the description of the operations. The <span class="tex-span"><i>i</i></span>-th line consists of the operation that Jamie has done in the <span class="tex-span"><i>i</i></span>-th day. The query has the following format:</p><p>The first word in the line indicates the type of operation. It must be one of the following four: <span class="tex-font-style-tt">set</span>, <span class="tex-font-style-tt">remove</span>, <span class="tex-font-style-tt">query</span>, <span class="tex-font-style-tt">undo</span>.</p><ul> <li> If it is a <span class="tex-font-style-tt">set</span> operation, a string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and an integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> follows <span class="tex-span">(1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>. <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the assignment that need to be set to <span class="tex-font-style-tt">priority</span> <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span>. </li><li> If it is a <span class="tex-font-style-tt">remove</span> operation, a string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> follows. <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the assignment that need to be removed. </li><li> If it is a <span class="tex-font-style-tt">query</span> operation, a string <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> follows. <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the assignment that needs to be queried. </li><li> If it is a <span class="tex-font-style-tt">undo</span> operation, an integer <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> follows <span class="tex-span">(0 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i>)</span>. <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span> is the number of days that changes needed to be undone. </li></ul><p>All assignment names <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> only consists of lowercase English letters and have a length <span class="tex-span">1 ≤ |<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 15</span>.</p><p>It is guaranteed that the last operation is a <span class="tex-font-style-tt">query</span> operation.</p>

## Output

<p>For each <span class="tex-font-style-tt">query</span> operation, output a single integer&nbsp;— the number of assignments that have a priority lower than assignment <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, or <span class="tex-span"> - 1</span> if <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is not in the to-do list.</p>





```input1
8
set chemlabreport 1
set physicsexercise 2
set chinesemockexam 3
query physicsexercise
query chinesemockexam
remove physicsexercise
query physicsexercise
query chinesemockexam

```




```input2
8
set physicsexercise 2
set chinesemockexam 3
set physicsexercise 1
query physicsexercise
query chinesemockexam
undo 4
query physicsexercise
query chinesemockexam

```




```input3
5
query economicsessay
remove economicsessay
query economicsessay
undo 2
query economicsessay

```




```input4
5
set economicsessay 1
remove economicsessay
undo 1
undo 1
query economicsessay

```




```output1
1
2
-1
1

```




```output2
0
1
0
-1

```




```output3
-1
-1
-1

```




```output4
-1

```


