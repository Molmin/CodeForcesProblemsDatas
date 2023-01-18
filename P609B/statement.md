## Description

<div><p>Emily's birthday is next week and Jack has decided to buy a present for her. He knows she loves books so he goes to the local bookshop, where there are <span class="tex-span"><i>n</i></span> books on sale from one of <span class="tex-span"><i>m</i></span> genres.</p><p>In the bookshop, Jack decides to buy <span class="tex-font-style-it">two books of different genres</span>.</p><p>Based on the genre of books on sale in the shop, find the number of options available to Jack for choosing two books of different genres for Emily. Options are considered different if they differ in at least one book.</p><p>The books are given by indices of their genres. The genres are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, 2 ≤ <i>m</i> ≤ 10</span>) — the number of books in the bookstore and the number of genres.</p><p>The second line contains a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) equals the genre of the <span class="tex-span"><i>i</i></span>-th book.</p><p>It is guaranteed that for each genre there is at least one book of that genre.</p></div><div class="output-specification"><p>Print the only integer — the number of ways in which Jack can choose books.</p><p>It is guaranteed that the answer doesn't exceed the value <span class="tex-span">2·10<sup class="upper-index">9</sup></span>.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup>, 2 ≤ <i>m</i> ≤ 10</span>) — the number of books in the bookstore and the number of genres.</p><p>The second line contains a sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>, where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>) equals the genre of the <span class="tex-span"><i>i</i></span>-th book.</p><p>It is guaranteed that for each genre there is at least one book of that genre.</p>

## Output

<p>Print the only integer — the number of ways in which Jack can choose books.</p><p>It is guaranteed that the answer doesn't exceed the value <span class="tex-span">2·10<sup class="upper-index">9</sup></span>.</p>





```input1
4 3
2 1 3 1

```




```input2
7 4
4 2 3 1 2 4 3

```




```output1
5

```




```output2
18

```



## Note

<p>The answer to the first test sample equals 5 as Sasha can choose:</p><ol> <li> the first and second books, </li><li> the first and third books, </li><li> the first and fourth books, </li><li> the second and third books, </li><li> the third and fourth books. </li></ol>
