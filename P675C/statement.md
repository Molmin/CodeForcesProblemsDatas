## Description

<div><p>There are <span class="tex-span"><i>n</i></span> banks in the city where Vasya lives, they are located in a circle, such that any two banks are neighbouring if their indices differ by no more than <span class="tex-span">1</span>. Also, bank <span class="tex-span">1</span> and bank <span class="tex-span"><i>n</i></span> are neighbours if <span class="tex-span"><i>n</i> &gt; 1</span>. No bank is a neighbour of itself.</p><p>Vasya has an account in each bank. Its balance may be negative, meaning Vasya owes some money to this bank.</p><p>There is only one type of operations available: transfer some amount of money from any bank to account in any <span class="tex-font-style-bf">neighbouring</span> bank. There are no restrictions on the size of the sum being transferred or balance requirements to perform this operation.</p><p>Vasya doesn't like to deal with large numbers, so he asks you to determine the minimum number of operations required to change the balance of each bank account to zero. It's guaranteed, that this is possible to achieve, that is, the total balance of Vasya in all banks is equal to zero.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of banks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the <span class="tex-span"><i>i</i></span>-th of them is equal to the initial balance of the account in the <span class="tex-span"><i>i</i></span>-th bank. It's guaranteed that the sum of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to <span class="tex-span">0</span>.</p></div><div class="output-specification"><p>Print the minimum number of operations required to change balance in each bank to zero.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>)&nbsp;— the number of banks.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span"> - 10<sup class="upper-index">9</sup> ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), the <span class="tex-span"><i>i</i></span>-th of them is equal to the initial balance of the account in the <span class="tex-span"><i>i</i></span>-th bank. It's guaranteed that the sum of all <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to <span class="tex-span">0</span>.</p>

## Output

<p>Print the minimum number of operations required to change balance in each bank to zero.</p>





```input1
3
5 0 -5

```




```input2
4
-1 0 1 0

```




```input3
4
1 2 3 -6

```




```output1
1

```




```output2
2

```




```output3
3

```



## Note

<p>In the first sample, Vasya may transfer <span class="tex-span">5</span> from the first bank to the third.</p><p>In the second sample, Vasya may first transfer <span class="tex-span">1</span> from the third bank to the second, and then <span class="tex-span">1</span> from the second to the first.</p><p>In the third sample, the following sequence provides the optimal answer: </p><ol> <li> transfer <span class="tex-span">1</span> from the first bank to the second bank; </li><li> transfer <span class="tex-span">3</span> from the second bank to the third; </li><li> transfer <span class="tex-span">6</span> from the third bank to the fourth. </li></ol>
