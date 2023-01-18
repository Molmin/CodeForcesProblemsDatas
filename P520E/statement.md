## Description

<div><p>Vasya is sitting on an extremely boring math class. To have fun, he took a piece of paper and wrote out <span class="tex-span"><i>n</i></span> numbers on a single line. After that, Vasya began to write out different ways to put pluses ("<span class="tex-font-style-tt">+</span>") in the line between certain digits in the line so that the result was a correct arithmetic expression; formally, no two pluses in such a partition can stand together (between any two adjacent pluses there must be at least one digit), and no plus can stand at the beginning or the end of a line. For example, in the string <span class="tex-font-style-tt">100500</span>, ways <span class="tex-font-style-tt">100500</span> (add no pluses), <span class="tex-font-style-tt">1+00+500</span> or <span class="tex-font-style-tt">10050+0</span> are correct, and ways <span class="tex-font-style-tt">100++500</span>, <span class="tex-font-style-tt">+1+0+0+5+0+0</span> or <span class="tex-font-style-tt">100500+</span> are incorrect.</p><p>The lesson was long, and Vasya has written all the correct ways to place exactly <span class="tex-span"><i>k</i></span> pluses in a string of digits. At this point, he got caught having fun by a teacher and he was given the task to calculate the sum of all the resulting arithmetic expressions by the end of the lesson (when calculating the value of an expression the leading zeros should be ignored). As the answer can be large, Vasya is allowed to get only its remainder modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. Help him!</p></div><div class="input-specification"><p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> &lt; <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains a string consisting of <span class="tex-span"><i>n</i></span> digits.</p></div><div class="output-specification"><p>Print the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains two integers, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> &lt; <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains a string consisting of <span class="tex-span"><i>n</i></span> digits.</p>

## Output

<p>Print the answer to the problem modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
3 1
108

```




```input2
3 2
108

```




```output1
27
```




```output2
9
```



## Note

<p>In the first sample the result equals <span class="tex-span">(1 + 08) + (10 + 8) = 27</span>.</p><p>In the second sample the result equals <span class="tex-span">1 + 0 + 8 = 9</span>.</p>
