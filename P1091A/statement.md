## Description

<div><p>Alice and Bob are decorating a Christmas Tree. </p><p>Alice wants only $3$ types of ornaments to be used on the Christmas Tree: yellow, blue and red. They have $y$ yellow ornaments, $b$ blue ornaments and $r$ red ornaments.</p><p>In Bob's opinion, a Christmas Tree will be beautiful if:</p><ul> <li> the number of blue ornaments used is greater by <span class="tex-font-style-bf">exactly</span> $1$ than the number of yellow ornaments, and </li><li> the number of red ornaments used is greater by <span class="tex-font-style-bf">exactly</span> $1$ than the number of blue ornaments. </li></ul><p>That is, if they have $8$ yellow ornaments, $13$ blue ornaments and $9$ red ornaments, we can choose $4$ yellow, $5$ blue and $6$ red ornaments ($5=4+1$ and $6=5+1$).</p><p>Alice wants to choose as many ornaments as possible, but she also wants the Christmas Tree to be beautiful according to Bob's opinion.</p><p>In the example two paragraphs above, we would choose $7$ yellow, $8$ blue and $9$ red ornaments. If we do it, we will use $7+8+9=24$ ornaments. That is the maximum number.</p><p>Since Alice and Bob are busy with preparing food to the New Year's Eve, they are asking you to find out the maximum number of ornaments that can be used in their <span class="tex-font-style-bf">beautiful</span> Christmas Tree! </p><p>It is guaranteed that it is possible to choose at least $6$ ($1+2+3=6$) ornaments.</p></div><div class="input-specification"><p>The only line contains three integers $y$, $b$, $r$ ($1 \leq y \leq 100$, $2 \leq b \leq 100$, $3 \leq r \leq 100$)&nbsp;— the number of yellow, blue and red ornaments. </p><p>It is guaranteed that it is possible to choose at least $6$ ($1+2+3=6$) ornaments.</p></div><div class="output-specification"><p>Print one number&nbsp;— the maximum number of ornaments that can be used. </p></div>

## Input

<p>The only line contains three integers $y$, $b$, $r$ ($1 \leq y \leq 100$, $2 \leq b \leq 100$, $3 \leq r \leq 100$)&nbsp;— the number of yellow, blue and red ornaments. </p><p>It is guaranteed that it is possible to choose at least $6$ ($1+2+3=6$) ornaments.</p>

## Output

<p>Print one number&nbsp;— the maximum number of ornaments that can be used. </p>





```input1
8 13 9
```




```input2
13 3 6
```




```output1
24
```




```output2
9
```



## Note

<p>In the first example, the answer is $7+8+9=24$.</p><p>In the second example, the answer is $2+3+4=9$.</p>
