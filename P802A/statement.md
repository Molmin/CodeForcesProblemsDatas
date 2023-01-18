## Description

<div><p>Your search for Heidi is over – you finally found her at a library, dressed up as a human. In fact, she has spent so much time there that she now runs the place! Her job is to buy books and keep them at the library so that people can borrow and read them. There are <span class="tex-span"><i>n</i></span> different books, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>.</p><p>We will look at the library's operation during <span class="tex-span"><i>n</i></span> consecutive days. Heidi knows in advance that on the <span class="tex-span"><i>i</i></span>-th day (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) precisely one person will come to the library, request to borrow the book <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, read it in a few hours, and return the book later on the same day.</p><p>Heidi desperately wants to please all her guests, so she will make sure to always have the book <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> available in the library on the <span class="tex-span"><i>i</i></span>-th day. During the night before the <span class="tex-span"><i>i</i></span>-th day, she has the option of going to the bookstore (which operates at nights to avoid competition with the library) and buying any book for the price of 1 CHF. Of course, if she already has a book at the library, she does not need to buy it again. Initially, the library contains no books.</p><p>There is a problem, though. The capacity of the library is <span class="tex-span"><i>k</i></span> – this means that at any time, there can be at most <span class="tex-span"><i>k</i></span> books at the library. If buying a new book would cause Heidi to have more than <span class="tex-span"><i>k</i></span> books, she must first get rid of some book that she already has, in order to make room for the new book. If she later needs a book that she got rid of, she will need to buy that book again.</p><p>You are given <span class="tex-span"><i>k</i></span> and the sequence of requests for books <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. What is the minimum cost (in CHF) of buying new books to satisfy all the requests?</p></div><div class="input-specification"><p>The first line of input will contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 80</span>). The second line will contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) – the sequence of book requests.</p></div><div class="output-specification"><p>On a single line print the minimum cost of buying books at the store so as to satisfy all requests.</p></div>

## Input

<p>The first line of input will contain two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 80</span>). The second line will contain <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>) – the sequence of book requests.</p>

## Output

<p>On a single line print the minimum cost of buying books at the store so as to satisfy all requests.</p>





```input1
4 80
1 2 2 1

```




```input2
4 1
1 2 2 1

```




```input3
4 2
1 2 3 1

```




```output1
2

```




```output2
3

```




```output3
3

```



## Note

<p>In the first test case, Heidi is able to keep all books forever. Therefore, she only needs to buy the book <span class="tex-span">1</span> before the first day and the book <span class="tex-span">2</span> before the second day.</p><p>In the second test case, she can only keep one book at a time. Therefore she will need to buy new books on the first, second and fourth day.</p><p>In the third test case, before buying book <span class="tex-span">3</span> on the third day, she must decide which of the books <span class="tex-span">1</span> and <span class="tex-span">2</span> she should get rid of. Of course, she should keep the book <span class="tex-span">1</span>, which will be requested on the fourth day.</p>
