## Description

<div><p><span class="tex-span"><i>n</i></span> pupils, who love to read books, study at school. It is known that each student has exactly one best friend, and each pupil is the best friend of exactly one other pupil. Each of the pupils has exactly one interesting book.</p><p>The pupils decided to share books with each other. Every day, all pupils give their own books to their best friends. Thus, every day each of the pupils has exactly one book.</p><p>Your task is to use the list of the best friends and determine the exchange of books among pupils after <span class="tex-span"><i>k</i></span> days. For simplicity, all students are numbered from 1 to <span class="tex-span"><i>n</i></span> in all tests.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100000, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">16</sup></span>) — the number of pupils and days during which they will exchange books.</p><p>The second line contains <span class="tex-span"><i>n</i></span> different integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the number of the pupil who has the best friend with the number <span class="tex-span"><i>i</i></span>.</p><p>It is guaranteed that no pupil is the best friend of himself.</p></div><div class="output-specification"><p>In a single line print <span class="tex-span"><i>n</i></span> different integers, where <span class="tex-span"><i>i</i></span>-th integer should be equal to the number of the pupil who will have the book, which the pupil with the number <span class="tex-span"><i>i</i></span> had in the beginning, after <span class="tex-span"><i>k</i></span> days.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100000, 1 ≤ <i>k</i> ≤ 10<sup class="upper-index">16</sup></span>) — the number of pupils and days during which they will exchange books.</p><p>The second line contains <span class="tex-span"><i>n</i></span> different integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the number of the pupil who has the best friend with the number <span class="tex-span"><i>i</i></span>.</p><p>It is guaranteed that no pupil is the best friend of himself.</p>

## Output

<p>In a single line print <span class="tex-span"><i>n</i></span> different integers, where <span class="tex-span"><i>i</i></span>-th integer should be equal to the number of the pupil who will have the book, which the pupil with the number <span class="tex-span"><i>i</i></span> had in the beginning, after <span class="tex-span"><i>k</i></span> days.</p>





```input1
4 1
2 4 1 3

```




```input2
5 5
3 4 5 2 1

```




```input3
6 18
2 3 5 1 6 4

```




```output1
3 1 4 2 

```




```output2
3 4 5 2 1 

```




```output3
1 2 3 4 5 6 

```



## Note

<p>The explanation to the first test.</p><p>There are 4 pupils and 1 day. The list of the best friends equals to {2, 4, 1, 3}. It means that:</p><ul> <li> the pupil with the number 3 — is the best friend of pupil with the number 1, </li><li> the pupil with the number 1 — is the best friend of pupil with the number 2, </li><li> the pupil with the number 4 — is the best friend of pupil with the number 3, </li><li> the pupil with the number 2 — is the best friend of pupil with the number 4. </li></ul><p>After the first day the exchange of books will be {3, 1, 4, 2}.</p><ul> <li> the pupil with the number 3 will have the book, which the pupil with the number 1 had in the beginning, </li><li> the pupil with the number 1 will have the book, which the pupil with the number 2 had in the beginning, </li><li> the pupil with the number 4 will have the book, which the pupil with the number 3 had in the beginning </li><li> the pupil with the number 2 will have the book, which the pupil with the number 4 had in the beginning. </li></ul><p>Thus, the answer is <span class="tex-font-style-bf">3 1 4 2</span>.</p>
