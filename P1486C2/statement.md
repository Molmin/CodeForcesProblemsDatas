## Description

<div><p><span class="tex-font-style-bf">The only difference between the easy and the hard version is the limit to the number of queries</span>.</p><p><span class="tex-font-style-bf">This is an interactive problem.</span></p><p>There is an array $a$ of $n$ <span class="tex-font-style-bf">different</span> numbers. In one query you can ask the position of the second maximum element in a subsegment $a[l..r]$. Find the position of the maximum element in the array in no more than <span class="tex-font-style-bf">20</span> queries.</p><p>A subsegment $a[l..r]$ is all the elements $a_l, a_{l + 1}, ..., a_r$. After asking this subsegment you will be given the position of the second maximum from this subsegment <span class="tex-font-style-bf">in the whole</span> array.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ $(2 \leq n \leq 10^5)$ — the number of elements in the array.</p></div><div><h2>Interaction</h2><p>You can ask queries by printing "<span class="tex-font-style-tt">? $l$ $r$</span>" $(1 \leq l &lt; r \leq n)$. The answer is the index of the second maximum of all elements $a_l, a_{l + 1}, ..., a_r$. Array $a$ is fixed beforehand and can't be changed in time of interaction.</p><p>You can output the answer by printing "<span class="tex-font-style-tt">! $p$</span>", where <span class="tex-font-style-tt">$p$</span> is the index of the maximum element in the array.</p><p>You can ask no more than <span class="tex-font-style-bf">20</span> queries. <span class="tex-font-style-bf">Printing the answer doesn't count as a query</span>.</p><p>After printing a query do not forget to output end of line and flush the output. Otherwise, you will get <span class="tex-font-style-tt">Idleness limit exceeded</span>. To do this, use:</p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> or <span class="tex-font-style-tt">cout.flush()</span> in C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> <span class="tex-font-style-tt">stdout.flush()</span> in Python; </li><li> see documentation for other languages </li></ul><p><span class="tex-font-style-bf"><span class="tex-font-style-section">Hacks</span></span></p><p>To make a hack, use the following test format.</p><p>In the first line output a single integer $n$ $(2 \leq n \leq 10^5)$. In the second line output a permutation of $n$ integers $1$ to $n$. The position of $n$ in the permutation is the position of the maximum</p></div>

## Input

<p>The first line contains a single integer $n$ $(2 \leq n \leq 10^5)$ — the number of elements in the array.</p>





```input1
5

3

4
```




```output1
? 1 5

? 4 5

! 1
```



## Note

<p>In the sample suppose $a$ is $[5, 1, 4, 2, 3]$. So after asking the $[1..5]$ subsegment $4$ is second to max value, and it's position is $3$. After asking the $[4..5]$ subsegment $2$ is second to max value and it's position in the whole array is $4$.</p><p>Note that there are other arrays $a$ that would produce the same interaction, and the answer for them might be different. Example output is given in purpose of understanding the interaction.</p>
