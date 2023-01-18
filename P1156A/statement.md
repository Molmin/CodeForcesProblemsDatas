## Description

<div><p>The math faculty of Berland State University has suffered the sudden drop in the math skills of enrolling students. This year the highest grade on the entrance math test was 8. Out of 100! Thus, the decision was made to make the test easier.</p><p>Future students will be asked just a single question. They are given a sequence of integer numbers $a_1, a_2, \dots, a_n$, each number is from $1$ to $3$ and $a_i \ne a_{i + 1}$ for each valid $i$. The $i$-th number represents a type of the $i$-th figure:</p><ol> <li> circle; </li><li> isosceles triangle with the length of height equal to the length of base; </li><li> square. </li></ol><p>The figures of the given sequence are placed somewhere on a Cartesian plane in such a way that:</p><ul> <li> $(i + 1)$-th figure is inscribed into the $i$-th one; </li><li> each triangle base is parallel to OX; </li><li> the triangle is oriented in such a way that the vertex opposite to its base is at the top; </li><li> each square sides are parallel to the axes; </li><li> for each $i$ from $2$ to $n$ figure $i$ has the maximum possible length of side for triangle and square and maximum radius for circle. </li></ul><p><span class="tex-font-style-it">Note that the construction is unique for some fixed position and size of just the first figure.</span></p><p>The task is to calculate the number of <span class="tex-font-style-bf">distinct</span> points (not necessarily with integer coordinates) where figures touch. The trick is, however, that the number is sometimes infinite. But that won't make the task difficult for you, will it?</p><p>So can you pass the math test and enroll into Berland State University?</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 100$) — the number of figures.</p><p>The second line contains $n$ integer numbers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 3$, $a_i \ne a_{i + 1}$) — types of the figures.</p></div><div class="output-specification"><p>The first line should contain either the word "<span class="tex-font-style-tt">Infinite</span>" if the number of distinct points where figures touch is infinite or "<span class="tex-font-style-tt">Finite</span>" otherwise.</p><p>If the number is finite than print it in the second line. It's guaranteed that the number fits into 32-bit integer type.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 100$) — the number of figures.</p><p>The second line contains $n$ integer numbers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 3$, $a_i \ne a_{i + 1}$) — types of the figures.</p>

## Output

<p>The first line should contain either the word "<span class="tex-font-style-tt">Infinite</span>" if the number of distinct points where figures touch is infinite or "<span class="tex-font-style-tt">Finite</span>" otherwise.</p><p>If the number is finite than print it in the second line. It's guaranteed that the number fits into 32-bit integer type.</p>





```input1
3
2 1 3
```




```input2
3
1 2 3
```




```output1
Finite
7
```




```output2
Infinite
```



## Note

<p>Here are the glorious pictures for the examples. Note that the triangle is not equilateral but just isosceles with the length of height equal to the length of base. Thus it fits into a square in a unique way.</p><p>The distinct points where figures touch are marked red.</p><p>In the second example the triangle and the square touch each other for the whole segment, it contains infinite number of points.</p><center> <img class="tex-graphics" src="file://LG9BSjGo.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
