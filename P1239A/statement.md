## Description

<div><p>Recently Ivan the Fool decided to become smarter and study the probability theory. He thinks that he understands the subject fairly well, and so he began to behave like he already got PhD in that area.</p><p>To prove his skills, Ivan decided to demonstrate his friends a concept of random picture. A picture is a field of $n$ rows and $m$ columns, where each cell is either black or white. Ivan calls the picture random if for every cell it has <span class="tex-font-style-bf">at most</span> one adjacent cell of the same color. Two cells are considered adjacent if they share a side.</p><p>Ivan's brothers spent some time trying to explain that it's not how the randomness usually works. Trying to convince Ivan, they want to count the number of different random (according to Ivan) pictures. Two pictures are considered different if at least one cell on those two picture is colored differently. Since the number of such pictures may be quite large, print it modulo $10^9 + 7$.</p></div><div class="input-specification"><p>The only line contains two integers $n$ and $m$ ($1 \le n, m \le 100\,000$), the number of rows and the number of columns of the field.</p></div><div class="output-specification"><p>Print one integer, the number of random pictures modulo $10^9 + 7$.</p></div>

## Input

<p>The only line contains two integers $n$ and $m$ ($1 \le n, m \le 100\,000$), the number of rows and the number of columns of the field.</p>

## Output

<p>Print one integer, the number of random pictures modulo $10^9 + 7$.</p>





```input1
2 3
```




```output1
8
```



## Note

<p>The picture below shows all possible random pictures of size $2$ by $3$. </p><center> <img class="tex-graphics" src="file://RavGJdmv.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
