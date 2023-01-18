## Description

<div><p>Mr Keks is a typical white-collar in Byteland.</p><p>He has a bookshelf in his office with some books on it, each book has an integer positive price.</p><p>Mr Keks defines the value of a shelf as the sum of books prices on it. </p><p>Miraculously, Mr Keks was promoted and now he is moving into a new office.</p><p>He learned that in the new office he will have not a single bookshelf, but exactly $k$ bookshelves. He decided that the beauty of the $k$ shelves is the <a href="https://en.wikipedia.org/wiki/Bitwise_operation#AND">bitwise AND</a> of the values of all the shelves.</p><p>He also decided that he won't spend time on reordering the books, so he will place several first books on the first shelf, several next books on the next shelf and so on. Of course, he will place at least one book on each shelf. This way he will put all his books on $k$ shelves in such a way that the beauty of the shelves is as large as possible. Compute this maximum possible beauty.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $k$ ($1 \leq k \leq n \leq 50$)&nbsp;— the number of books and the number of shelves in the new office.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots a_n$, ($0 &lt; a_i &lt; 2^{50}$)&nbsp;— the prices of the books in the order they stand on the old shelf.</p></div><div class="output-specification"><p>Print the maximum possible beauty of $k$ shelves in the new office.</p></div>

## Input

<p>The first line contains two integers $n$ and $k$ ($1 \leq k \leq n \leq 50$)&nbsp;— the number of books and the number of shelves in the new office.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots a_n$, ($0 &lt; a_i &lt; 2^{50}$)&nbsp;— the prices of the books in the order they stand on the old shelf.</p>

## Output

<p>Print the maximum possible beauty of $k$ shelves in the new office.</p>





```input1
10 4
9 14 28 1 7 13 15 29 2 31

```




```input2
7 3
3 14 15 92 65 35 89

```




```output1
24

```




```output2
64

```



## Note

<p>In the first example you can split the books as follows:</p><p>$$(9 + 14 + 28 + 1 + 7) \&amp; (13 + 15) \&amp; (29 + 2) \&amp; (31) = 24.$$</p><p>In the second example you can split the books as follows:</p><p>$$(3 + 14 + 15 + 92) \&amp; (65) \&amp; (35 + 89) = 64.$$</p>
