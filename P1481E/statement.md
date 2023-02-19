## Description

<div><p>One day you wanted to read something, so you went to your bookshelf to grab some book. But when you saw how messy the bookshelf was you decided to clean it up first.</p><center> <img class="tex-graphics" src="file://WKtUXVSD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>There are $n$ books standing in a row on the shelf, the $i$-th book has color $a_i$.</p><p>You'd like to rearrange the books to make the shelf look beautiful. The shelf is considered <span class="tex-font-style-it">beautiful</span> if all books of the same color are next to each other.</p><p>In one operation you can take one book from any position on the shelf and move it to the right end of the shelf.</p><p>What is the minimum number of operations you need to make the shelf beautiful?</p></div><div class="input-specification"><p>The first line contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$)&nbsp;— the number of books.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$)&nbsp;— the book colors.</p></div><div class="output-specification"><p>Output the minimum number of operations to make the shelf beautiful.</p></div>

## Input

<p>The first line contains one integer $n$ ($1 \le n \le 5 \cdot 10^5$)&nbsp;— the number of books.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$)&nbsp;— the book colors.</p>

## Output

<p>Output the minimum number of operations to make the shelf beautiful.</p>





```input1
5
1 2 2 1 3
```




```input2
5
1 2 2 1 1
```




```output1
2
```




```output2
1
```



## Note

<p>In the first example, we have the bookshelf $[1, 2, 2, 1, 3]$ and can, for example: </p><ol> <li> take a book on position $4$ and move to the right end: we'll get $[1, 2, 2, 3, 1]$; </li><li> take a book on position $1$ and move to the right end: we'll get $[2, 2, 3, 1, 1]$. </li></ol><p>In the second example, we can move the first book to the end of the bookshelf and get $[2,2,1,1,1]$.</p>
