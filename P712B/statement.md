## Description

<div><p>Memory is performing a walk on the two-dimensional plane, starting at the origin. He is given a string <span class="tex-span"><i>s</i></span> with his directions for motion:</p><ul><li> An '<span class="tex-font-style-tt">L</span>' indicates he should move one unit left. </li><li> An '<span class="tex-font-style-tt">R</span>' indicates he should move one unit right. </li><li> A '<span class="tex-font-style-tt">U</span>' indicates he should move one unit up. </li><li> A '<span class="tex-font-style-tt">D</span>' indicates he should move one unit down.</li></ul><p>But now Memory wants to end at the origin. To do this, he has a special trident. This trident can replace any character in <span class="tex-span"><i>s</i></span> with any of '<span class="tex-font-style-tt">L</span>', '<span class="tex-font-style-tt">R</span>', '<span class="tex-font-style-tt">U</span>', or '<span class="tex-font-style-tt">D</span>'. However, because he doesn't want to wear out the trident, he wants to make the minimum number of edits possible. Please tell Memory what is the minimum number of changes he needs to make to produce a string that, when walked, will end at the origin, or if there is no such string.</p></div><div class="input-specification"><p>The first and only line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100 000</span>)&nbsp;— the instructions Memory is given.</p></div><div class="output-specification"><p>If there is a string satisfying the conditions, output a single integer&nbsp;— the minimum number of edits required. In case it's not possible to change the sequence in such a way that it will bring Memory to to the origin, output <span class="tex-font-style-tt">-1</span>.</p></div>

## Input

<p>The first and only line contains the string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 100 000</span>)&nbsp;— the instructions Memory is given.</p>

## Output

<p>If there is a string satisfying the conditions, output a single integer&nbsp;— the minimum number of edits required. In case it's not possible to change the sequence in such a way that it will bring Memory to to the origin, output <span class="tex-font-style-tt">-1</span>.</p>





```input1
RRU

```




```input2
UDUR

```




```input3
RUUR

```




```output1
-1

```




```output2
1

```




```output3
2

```



## Note

<p>In the first sample test, Memory is told to walk right, then right, then up. It is easy to see that it is impossible to edit these instructions to form a valid walk.</p><p>In the second sample test, Memory is told to walk up, then down, then up, then right. One possible solution is to change <span class="tex-span"><i>s</i></span> to "<span class="tex-font-style-tt">LDUR</span>". This string uses 1 edit, which is the minimum possible. It also ends at the origin.</p>
