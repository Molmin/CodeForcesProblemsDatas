## Description

<div><p>New Year is coming, and Jaehyun decided to read many books during 2015, unlike this year. He has <span class="tex-span"><i>n</i></span> books numbered by integers from 1 to <span class="tex-span"><i>n</i></span>. The weight of the <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) book is <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>As Jaehyun's house is not large enough to have a bookshelf, he keeps the <span class="tex-span"><i>n</i></span> books by stacking them vertically. When he wants to read a certain book <span class="tex-span"><i>x</i></span>, he follows the steps described below.</p><ol> <li> He <span class="tex-font-style-it">lifts</span> all the books above book <span class="tex-span"><i>x</i></span>. </li><li> He pushes book <span class="tex-span"><i>x</i></span> out of the stack. </li><li> He puts down the lifted books without changing their order. </li><li> After reading book <span class="tex-span"><i>x</i></span>, he puts book <span class="tex-span"><i>x</i></span> on the top of the stack. </li></ol><center><p><img class="tex-graphics" src="file://xfkFKMaG.png" style="max-width: 100.0%;max-height: 100.0%;"> </p></center><p>He decided to read books for <span class="tex-span"><i>m</i></span> days. In the <span class="tex-span"><i>j</i></span>-th (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>m</i></span>) day, he will read the book that is numbered with integer <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>). To read the book, he has to use the process described in the paragraph above. It is possible that he decides to re-read the same book several times.</p><p>After making this plan, he realized that the total weight of books he should <span class="tex-font-style-it">lift</span> during <span class="tex-span"><i>m</i></span> days would be too heavy. So, he decided to change the order of the stacked books before the New Year comes, and minimize the total weight. You may assume that books can be stacked in any possible order. Note that book that he is going to read on certain step isn't considered as <span class="tex-font-style-it">lifted</span> on that step. Can you help him?</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>) — the number of books, and the number of days for which Jaehyun would read books.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the weight of each book.</p><p>The third line contains <span class="tex-span"><i>m</i></span> space separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the order of books that he would read. Note that he can read the same book more than once.</p></div><div class="output-specification"><p>Print the minimum total weight of books he should <span class="tex-font-style-it">lift</span>, which can be achieved by rearranging the order of stacked books.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 500</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>) — the number of books, and the number of days for which Jaehyun would read books.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the weight of each book.</p><p>The third line contains <span class="tex-span"><i>m</i></span> space separated integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ <i>n</i></span>) — the order of books that he would read. Note that he can read the same book more than once.</p>

## Output

<p>Print the minimum total weight of books he should <span class="tex-font-style-it">lift</span>, which can be achieved by rearranging the order of stacked books.</p>





```input1
3 5
1 2 3
1 3 2 3 1

```




```output1
12

```



## Note

<p>Here's a picture depicting the example. Each vertical column presents the stacked books.</p><center> <img class="tex-graphics" src="file://rjNzV1ni.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
