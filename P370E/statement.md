## Description

<div><p>At school Vasya got an impressive list of summer reading books. Unlike other modern schoolchildren, Vasya loves reading, so he read some book each day of the summer.</p><p>As Vasya was reading books, he was making notes in the Reader's Diary. Each day he wrote the orderal number of the book he was reading. The books in the list are numbered starting from 1 and Vasya was reading them in the order they go in the list. Vasya never reads a new book until he finishes reading the previous one. Unfortunately, Vasya wasn't accurate and some days he forgot to note the number of the book and the notes for those days remained empty.</p><p>As Vasya knows that the literature teacher will want to check the Reader's Diary, so he needs to restore the lost records. Help him do it and fill all the blanks. Vasya is sure that he spends at least two and at most five days for each book. Vasya finished reading all the books he had started. Assume that the reading list contained many books. So many, in fact, that it is impossible to read all of them in a summer. If there are multiple valid ways to restore the diary records, Vasya prefers the one that shows the maximum number of read books.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of summer days (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> — the records in the diary in the order they were written (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). If Vasya forgot to write the number of the book on the <span class="tex-span"><i>i</i></span>-th day, then <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals 0. </p></div><div class="output-specification"><p>If it is impossible to correctly fill the blanks in the diary (the diary may contain mistakes initially), print "-1". </p><p>Otherwise, print in the first line the maximum number of books Vasya could have read in the summer if we stick to the diary. In the second line print <span class="tex-span"><i>n</i></span> integers — the diary with correctly inserted records. If there are multiple optimal solutions, you can print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> — the number of summer days (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>). The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ... <i>a</i><sub class="lower-index"><i>n</i></sub></span> — the records in the diary in the order they were written (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>). If Vasya forgot to write the number of the book on the <span class="tex-span"><i>i</i></span>-th day, then <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> equals 0. </p>

## Output

<p>If it is impossible to correctly fill the blanks in the diary (the diary may contain mistakes initially), print "-1". </p><p>Otherwise, print in the first line the maximum number of books Vasya could have read in the summer if we stick to the diary. In the second line print <span class="tex-span"><i>n</i></span> integers — the diary with correctly inserted records. If there are multiple optimal solutions, you can print any of them.</p>





```input1
7
0 1 0 0 0 3 0

```




```input2
8
0 0 0 0 0 0 0 0

```




```input3
4
0 0 1 0

```




```input4
4
0 0 0 3

```




```output1
3
1 1 2 2 3 3 3 

```




```output2
4
1 1 2 2 3 3 4 4 

```




```output3
1
1 1 1 1 

```




```output4
-1

```


