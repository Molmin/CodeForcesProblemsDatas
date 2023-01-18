## Description

<div><p>The semester is already ending, so Danil made an effort and decided to visit a lesson on harmony analysis to know how does the professor look like, at least. Danil was very bored on this lesson until the teacher gave the group a simple task: find <span class="tex-span">4</span> vectors in <span class="tex-span">4</span>-dimensional space, such that every coordinate of every vector is <span class="tex-span">1</span> or <span class="tex-span"> - 1</span> and any two vectors are orthogonal. Just as a reminder, two vectors in <span class="tex-span"><i>n</i></span>-dimensional space are considered to be orthogonal if and only if their scalar product is equal to zero, that is: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://ARQUYLPp.png" style="max-width: 100.0%;max-height: 100.0%;"></center>.<p>Danil quickly managed to come up with the solution for this problem and the teacher noticed that the problem can be solved in a more general case for <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span> vectors in <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span>-dimensinoal space. When Danil came home, he quickly came up with the solution for this problem. Can you cope with it?</p></div><div class="input-specification"><p>The only line of the input contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 9</span>).</p></div><div class="output-specification"><p>Print <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span> lines consisting of <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span> characters each. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line must be equal to '<span class="tex-span"> * </span>' if the <span class="tex-span"><i>j</i></span>-th coordinate of the <span class="tex-span"><i>i</i></span>-th vector is equal to <span class="tex-span"> - 1</span>, and must be equal to '<span class="tex-span"> + </span>' if it's equal to <span class="tex-span"> + 1</span>. It's guaranteed that the answer always exists.</p><p>If there are many correct answers, print any.</p></div>

## Input

<p>The only line of the input contains a single integer <span class="tex-span"><i>k</i></span> (<span class="tex-span">0 ≤ <i>k</i> ≤ 9</span>).</p>

## Output

<p>Print <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span> lines consisting of <span class="tex-span">2<sup class="upper-index"><i>k</i></sup></span> characters each. The <span class="tex-span"><i>j</i></span>-th character of the <span class="tex-span"><i>i</i></span>-th line must be equal to '<span class="tex-span"> * </span>' if the <span class="tex-span"><i>j</i></span>-th coordinate of the <span class="tex-span"><i>i</i></span>-th vector is equal to <span class="tex-span"> - 1</span>, and must be equal to '<span class="tex-span"> + </span>' if it's equal to <span class="tex-span"> + 1</span>. It's guaranteed that the answer always exists.</p><p>If there are many correct answers, print any.</p>





```input1
2

```




```output1
++**
+*+*
++++
+**+
```



## Note

<p>Consider all scalar products in example:</p><ul> <li> Vectors <span class="tex-span">1</span> and <span class="tex-span">2</span>: <span class="tex-span">( + 1)·( + 1) + ( + 1)·( - 1) + ( - 1)·( + 1) + ( - 1)·( - 1) = 0</span> </li><li> Vectors <span class="tex-span">1</span> and <span class="tex-span">3</span>: <span class="tex-span">( + 1)·( + 1) + ( + 1)·( + 1) + ( - 1)·( + 1) + ( - 1)·( + 1) = 0</span> </li><li> Vectors <span class="tex-span">1</span> and <span class="tex-span">4</span>: <span class="tex-span">( + 1)·( + 1) + ( + 1)·( - 1) + ( - 1)·( - 1) + ( - 1)·( + 1) = 0</span> </li><li> Vectors <span class="tex-span">2</span> and <span class="tex-span">3</span>: <span class="tex-span">( + 1)·( + 1) + ( - 1)·( + 1) + ( + 1)·( + 1) + ( - 1)·( + 1) = 0</span> </li><li> Vectors <span class="tex-span">2</span> and <span class="tex-span">4</span>: <span class="tex-span">( + 1)·( + 1) + ( - 1)·( - 1) + ( + 1)·( - 1) + ( - 1)·( + 1) = 0</span> </li><li> Vectors <span class="tex-span">3</span> and <span class="tex-span">4</span>: <span class="tex-span">( + 1)·( + 1) + ( + 1)·( - 1) + ( + 1)·( - 1) + ( + 1)·( + 1) = 0</span> </li></ul>
