## Description

<div><p>Ralph has a magic field which is divided into <span class="tex-span"><i>n</i> × <i>m</i></span> blocks. That is to say, there are <span class="tex-span"><i>n</i></span> rows and <span class="tex-span"><i>m</i></span> columns on the field. Ralph can put an integer in each block. However, the magic field doesn't always work properly. It works only if the product of integers in each row and each column equals to <span class="tex-span"><i>k</i></span>, where <span class="tex-span"><i>k</i></span> is either <span class="tex-font-style-tt">1</span> or <span class="tex-font-style-tt">-1</span>.</p><p>Now Ralph wants you to figure out the number of ways to put numbers in each block in such a way that the magic field works properly. Two ways are considered different if and only if there exists at least one block where the numbers in the first way and in the second way are different. You are asked to output the answer modulo <span class="tex-span">1000000007 = 10<sup class="upper-index">9</sup> + 7</span>.</p><p>Note that there is no range of the numbers to put in the blocks, but we can prove that the answer is not infinity.</p></div><div class="input-specification"><p>The only line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"><i>k</i></span> is either <span class="tex-font-style-tt">1</span> or <span class="tex-font-style-tt">-1</span>).</p></div><div class="output-specification"><p>Print a single number denoting the answer modulo <span class="tex-span">1000000007</span>.</p></div>

## Input

<p>The only line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">18</sup></span>, <span class="tex-span"><i>k</i></span> is either <span class="tex-font-style-tt">1</span> or <span class="tex-font-style-tt">-1</span>).</p>

## Output

<p>Print a single number denoting the answer modulo <span class="tex-span">1000000007</span>.</p>





```input1
1 1 -1

```




```input2
1 3 1

```




```input3
3 3 -1

```




```output1
1

```




```output2
1

```




```output3
16

```



## Note

<p>In the first example the only way is to put <span class="tex-font-style-tt">-1</span> into the only block.</p><p>In the second example the only way is to put <span class="tex-font-style-tt">1</span> into every block.</p>
