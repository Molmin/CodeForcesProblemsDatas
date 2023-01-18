## Description

<div><p>One day Petya was solving a very interesting problem. But although he used many optimization techniques, his solution still got Time limit exceeded verdict. Petya conducted a thorough analysis of his program and found out that his function for finding maximum element in an array of <span class="tex-span"><i>n</i></span> positive integers was too slow. Desperate, Petya decided to use a somewhat unexpected optimization using parameter <span class="tex-span"><i>k</i></span>, so now his function contains the following code:</p><pre class="verbatim"><br>int fast_max(int n, int a[]) { <br>    int ans = 0;<br>    int offset = 0;<br>    for (int i = 0; i &lt; n; ++i)<br>        if (ans &lt; a[i]) {<br>            ans = a[i];<br>            offset = 0;<br>        } else {<br>            offset = offset + 1;<br>            if (offset == k)<br>                return ans;<br>        }<br>    return ans;<br>}<br></pre><p>That way the function iteratively checks array elements, storing the intermediate maximum, and if after <span class="tex-span"><i>k</i></span> consecutive iterations that maximum has not changed, it is returned as the answer.</p><p>Now Petya is interested in fault rate of his function. He asked you to find the number of permutations of integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> such that the return value of his function on those permutations is not equal to <span class="tex-span"><i>n</i></span>. Since this number could be very big, output the answer modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The only line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>), separated by a space&nbsp;— the length of the permutations and the parameter <span class="tex-span"><i>k</i></span>.</p></div><div class="output-specification"><p>Output the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The only line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">6</sup></span>), separated by a space&nbsp;— the length of the permutations and the parameter <span class="tex-span"><i>k</i></span>.</p>

## Output

<p>Output the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
5 2

```




```input2
5 3

```




```input3
6 3

```




```output1
22

```




```output2
6

```




```output3
84

```



## Note

<p>Permutations from second example: </p><p><span class="tex-span">[4, 1, 2, 3, 5]</span>, <span class="tex-span">[4, 1, 3, 2, 5]</span>, <span class="tex-span">[4, 2, 1, 3, 5]</span>, <span class="tex-span">[4, 2, 3, 1, 5]</span>, <span class="tex-span">[4, 3, 1, 2, 5]</span>, <span class="tex-span">[4, 3, 2, 1, 5]</span>.</p>
