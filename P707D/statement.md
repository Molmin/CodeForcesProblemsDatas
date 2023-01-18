## Description

<div><p>Recently in school Alina has learned what are the <span class="tex-font-style-it">persistent data structures</span>: they are data structures that always preserves the previous version of itself and access to it when it is modified.</p><p>After reaching home Alina decided to invent her own persistent data structure. Inventing didn't take long: there is a bookcase right behind her bed. Alina thinks that the bookcase is a good choice for a persistent data structure. Initially the bookcase is empty, thus there is no book at any position at any shelf.</p><p>The bookcase consists of <span class="tex-span"><i>n</i></span> shelves, and each shelf has exactly <span class="tex-span"><i>m</i></span> positions for books at it. Alina enumerates shelves by integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> and positions at shelves&nbsp;— from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. Initially the bookcase is empty, thus there is no book at any position at any shelf in it.</p><p>Alina wrote down <span class="tex-span"><i>q</i></span> operations, which will be consecutively applied to the bookcase. Each of the operations has one of four types:</p><ul><li> <span class="tex-span">1</span> <span class="tex-span"><i>i</i></span> <span class="tex-span"><i>j</i></span>&nbsp;— Place a book at position <span class="tex-span"><i>j</i></span> at shelf <span class="tex-span"><i>i</i></span> if there is no book at it.</li><li> <span class="tex-span">2</span> <span class="tex-span"><i>i</i></span> <span class="tex-span"><i>j</i></span>&nbsp;— Remove the book from position <span class="tex-span"><i>j</i></span> at shelf <span class="tex-span"><i>i</i></span> if there is a book at it.</li><li> <span class="tex-span">3</span> <span class="tex-span"><i>i</i></span>&nbsp;— Invert book placing at shelf <span class="tex-span"><i>i</i></span>. This means that from every position at shelf <span class="tex-span"><i>i</i></span> which has a book at it, the book should be removed, and at every position at shelf <span class="tex-span"><i>i</i></span> which has not book at it, a book should be placed.</li><li> <span class="tex-span">4</span> <span class="tex-span"><i>k</i></span>&nbsp;— Return the books in the bookcase in a state they were after applying <span class="tex-span"><i>k</i></span>-th operation. In particular, <span class="tex-span"><i>k</i> = 0</span> means that the bookcase should be in initial state, thus every book in the bookcase should be removed from its position.</li></ul><p>After applying each of operation Alina is interested in the number of books in the bookcase. Alina got 'A' in the school and had no problem finding this values. Will you do so?</p></div><div class="input-specification"><p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">3</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the bookcase dimensions and the number of operations respectively.</p><p>The next <span class="tex-span"><i>q</i></span> lines describes operations in chronological order&nbsp;— <span class="tex-span"><i>i</i></span>-th of them describes <span class="tex-span"><i>i</i></span>-th operation in one of the four formats described in the statement.</p><p>It is guaranteed that shelf indices and position indices are correct, and in each of fourth-type operation the number <span class="tex-span"><i>k</i></span> corresponds to some operation before it or equals to <span class="tex-span">0</span>.</p></div><div class="output-specification"><p>For each operation, print the number of books in the bookcase after applying it in a separate line. The answers should be printed in chronological order.</p></div>

## Input

<p>The first line of the input contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">3</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the bookcase dimensions and the number of operations respectively.</p><p>The next <span class="tex-span"><i>q</i></span> lines describes operations in chronological order&nbsp;— <span class="tex-span"><i>i</i></span>-th of them describes <span class="tex-span"><i>i</i></span>-th operation in one of the four formats described in the statement.</p><p>It is guaranteed that shelf indices and position indices are correct, and in each of fourth-type operation the number <span class="tex-span"><i>k</i></span> corresponds to some operation before it or equals to <span class="tex-span">0</span>.</p>

## Output

<p>For each operation, print the number of books in the bookcase after applying it in a separate line. The answers should be printed in chronological order.</p>





```input1
2 3 3
1 1 1
3 2
4 0

```




```input2
4 2 6
3 2
2 2 2
3 3
3 2
2 2 2
3 2

```




```input3
2 2 2
3 2
2 2 1

```




```output1
1
4
0

```




```output2
2
1
3
3
2
4

```




```output3
2
1

```



## Note

<center><img class="tex-graphics" src="file://7Ah2UJXQ.png" style="max-width: 100.0%;max-height: 100.0%;"><p>This image illustrates the second sample case.</p></center>
