## Description

<div><p>Katya studies in a fifth grade. Recently her class studied right triangles and the Pythagorean theorem. It appeared, that there are triples of positive integers such that you can construct a right triangle with segments of lengths corresponding to triple. Such triples are called <span class="tex-font-style-it">Pythagorean triples</span>.</p><p>For example, triples <span class="tex-span">(3, 4, 5)</span>, <span class="tex-span">(5, 12, 13)</span> and <span class="tex-span">(6, 8, 10)</span> are Pythagorean triples.</p><p>Here Katya wondered if she can specify the length of some side of right triangle and find any Pythagorean triple corresponding to such length? Note that the side which length is specified can be a cathetus as well as hypotenuse.</p><p>Katya had no problems with completing this task. Will you do the same?</p></div><div class="input-specification"><p>The only line of the input contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the length of some side of a right triangle.</p></div><div class="output-specification"><p>Print two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>), such that <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> form a Pythagorean triple, in the only line.</p><p>In case if there is no any Pythagorean triple containing integer <span class="tex-span"><i>n</i></span>, print <span class="tex-span"> - 1</span> in the only line. If there are many answers, print any of them.</p></div>

## Input

<p>The only line of the input contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the length of some side of a right triangle.</p>

## Output

<p>Print two integers <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>m</i>, <i>k</i> ≤ 10<sup class="upper-index">18</sup></span>), such that <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>k</i></span> form a Pythagorean triple, in the only line.</p><p>In case if there is no any Pythagorean triple containing integer <span class="tex-span"><i>n</i></span>, print <span class="tex-span"> - 1</span> in the only line. If there are many answers, print any of them.</p>





```input1
3

```




```input2
6

```




```input3
1

```




```input4
17

```




```input5
67

```




```output1
4 5
```




```output2
8 10
```




```output3
-1
```




```output4
144 145
```




```output5
2244 2245
```



## Note

<center><img class="tex-graphics" src="file://Pq13FInu.png" style="max-width: 100.0%;max-height: 100.0%;"><p>Illustration for the first sample.</p></center>
