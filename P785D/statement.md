## Description

<div><p>As you probably know, Anton goes to school. One of the school subjects that Anton studies is Bracketology. On the Bracketology lessons students usually learn different sequences that consist of round brackets (characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" (without quotes)).</p><p>On the last lesson Anton learned about the regular simple bracket sequences (RSBS). A bracket sequence <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> is an RSBS if the following conditions are met:</p><ul> <li> It is not empty (that is <span class="tex-span"><i>n</i> ≠ 0</span>). </li><li> The length of the sequence is even. </li><li> First <img align="middle" class="tex-formula" src="file://agnLpY21.png" style="max-width: 100.0%;max-height: 100.0%;"> charactes of the sequence are equal to "<span class="tex-font-style-tt">(</span>". </li><li> Last <img align="middle" class="tex-formula" src="file://DtyzaPd8.png" style="max-width: 100.0%;max-height: 100.0%;"> charactes of the sequence are equal to "<span class="tex-font-style-tt">)</span>". </li></ul><p>For example, the sequence "<span class="tex-font-style-tt">((()))</span>" is an RSBS but the sequences "<span class="tex-font-style-tt">((())</span>" and "<span class="tex-font-style-tt">(()())</span>" are not RSBS.</p><p>Elena Ivanovna, Anton's teacher, gave him the following task as a homework. Given a bracket sequence <span class="tex-span"><i>s</i></span>. Find the number of its distinct subsequences such that they are RSBS. Note that a subsequence of <span class="tex-span"><i>s</i></span> is a string that can be obtained from <span class="tex-span"><i>s</i></span> by deleting some of its elements. Two subsequences are considered distinct if distinct sets of positions are deleted.</p><p>Because the answer can be very big and Anton's teacher doesn't like big numbers, she asks Anton to find the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p><p>Anton thought of this task for a very long time, but he still doesn't know how to solve it. Help Anton to solve this task and write a program that finds the answer for it!</p></div><div class="input-specification"><p>The only line of the input contains a string <span class="tex-span"><i>s</i></span>&nbsp;— the bracket sequence given in Anton's homework. The string consists only of characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" (without quotes). It's guaranteed that the string is not empty and its length doesn't exceed <span class="tex-span">200 000</span>.</p></div><div class="output-specification"><p>Output one number&nbsp;— the answer for the task modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The only line of the input contains a string <span class="tex-span"><i>s</i></span>&nbsp;— the bracket sequence given in Anton's homework. The string consists only of characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>" (without quotes). It's guaranteed that the string is not empty and its length doesn't exceed <span class="tex-span">200 000</span>.</p>

## Output

<p>Output one number&nbsp;— the answer for the task modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
)(()()

```




```input2
()()()

```




```input3
)))

```




```output1
6

```




```output2
7

```




```output3
0

```



## Note

<p>In the first sample the following subsequences are possible:</p><ul> <li> If we delete characters at the positions <span class="tex-span">1</span> and <span class="tex-span">5</span> (numbering starts with one), we will get the subsequence "<span class="tex-font-style-tt">(())</span>". </li><li> If we delete characters at the positions <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">3</span> and <span class="tex-span">4</span>, we will get the subsequence "<span class="tex-font-style-tt">()</span>". </li><li> If we delete characters at the positions <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">4</span> and <span class="tex-span">5</span>, we will get the subsequence "<span class="tex-font-style-tt">()</span>". </li><li> If we delete characters at the positions <span class="tex-span">1</span>, <span class="tex-span">2</span>, <span class="tex-span">5</span> and <span class="tex-span">6</span>, we will get the subsequence "<span class="tex-font-style-tt">()</span>". </li><li> If we delete characters at the positions <span class="tex-span">1</span>, <span class="tex-span">3</span>, <span class="tex-span">4</span> and <span class="tex-span">5</span>, we will get the subsequence "<span class="tex-font-style-tt">()</span>". </li><li> If we delete characters at the positions <span class="tex-span">1</span>, <span class="tex-span">3</span>, <span class="tex-span">5</span> and <span class="tex-span">6</span>, we will get the subsequence "<span class="tex-font-style-tt">()</span>". </li></ul><p>The rest of the subsequnces are not RSBS. So we got <span class="tex-span">6</span> distinct subsequences that are RSBS, so the answer is <span class="tex-span">6</span>.</p>
