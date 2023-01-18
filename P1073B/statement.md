## Description

<div><p>Vasya has got $n$ books, numbered from $1$ to $n$, arranged in a stack. The topmost book has number $a_1$, the next one — $a_2$, and so on. The book at the bottom of the stack has number $a_n$. <span class="tex-font-style-bf">All numbers are distinct</span>.</p><p>Vasya wants to move all the books to his backpack in $n$ steps. During $i$-th step he wants to move the book number $b_i$ into his backpack. If the book with number $b_i$ is in the stack, he takes this book and all the books <span class="tex-font-style-bf">above</span> the book $b_i$, and puts them into the backpack; otherwise he does nothing and begins the next step. For example, if books are arranged in the order $[1, 2, 3]$ (book $1$ is the topmost), and Vasya moves the books in the order $[2, 1, 3]$, then during the first step he will move two books ($1$ and $2$), during the second step he will do nothing (since book $1$ is already in the backpack), and during the third step — one book (the book number $3$). <span class="tex-font-style-bf">Note that $b_1, b_2, \dots, b_n$ are distinct.</span></p><p>Help Vasya! Tell him the number of books he will put into his backpack during each step.</p></div><div class="input-specification"><p>The first line contains one integer $n~(1 \le n \le 2 \cdot 10^5)$ — the number of books in the stack.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n~(1 \le a_i \le n)$ denoting the stack of books.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n~(1 \le b_i \le n)$ denoting the steps Vasya is going to perform.</p><p>All numbers $a_1 \dots a_n$ are distinct, the same goes for $b_1 \dots b_n$.</p></div><div class="output-specification"><p>Print $n$ integers. The $i$-th of them should be equal to the number of books Vasya moves to his backpack during the $i$-th step.</p></div>

## Input

<p>The first line contains one integer $n~(1 \le n \le 2 \cdot 10^5)$ — the number of books in the stack.</p><p>The second line contains $n$ integers $a_1, a_2, \dots, a_n~(1 \le a_i \le n)$ denoting the stack of books.</p><p>The third line contains $n$ integers $b_1, b_2, \dots, b_n~(1 \le b_i \le n)$ denoting the steps Vasya is going to perform.</p><p>All numbers $a_1 \dots a_n$ are distinct, the same goes for $b_1 \dots b_n$.</p>

## Output

<p>Print $n$ integers. The $i$-th of them should be equal to the number of books Vasya moves to his backpack during the $i$-th step.</p>





```input1
3
1 2 3
2 1 3

```




```input2
5
3 1 4 2 5
4 5 1 3 2

```




```input3
6
6 5 4 3 2 1
6 5 3 4 2 1

```




```output1
2 0 1 

```




```output2
3 2 0 0 0 

```




```output3
1 1 2 0 1 1 

```



## Note

<p>The first example is described in the statement.</p><p>In the second example, during the first step Vasya will move the books $[3, 1, 4]$. After that only books $2$ and $5$ remain in the stack ($2$ is above $5$). During the second step Vasya will take the books $2$ and $5$. After that the stack becomes empty, so during next steps Vasya won't move any books.</p>
