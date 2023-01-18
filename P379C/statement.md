## Description

<div><p>One very well-known internet resource site (let's call it X) has come up with a New Year adventure. Specifically, they decided to give ratings to all visitors.</p><p>There are <span class="tex-span"><i>n</i></span> users on the site, for each user we know the rating value he wants to get as a New Year Present. We know that user <span class="tex-span"><i>i</i></span> wants to get at least <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> rating units as a present.</p><p>The X site is administered by very creative and thrifty people. On the one hand, they want to give distinct ratings and on the other hand, the total sum of the ratings in the present must be as small as possible.</p><p>Help site X cope with the challenging task of rating distribution. Find the optimal distribution.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>)</span> — the number of users on the site. The next line contains integer sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p></div><div class="output-specification"><p>Print a sequence of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. Number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> means that user <span class="tex-span"><i>i</i></span> gets <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> of rating as a present. The printed sequence must meet the problem conditions. </p><p>If there are multiple optimal solutions, print any of them.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup>)</span> — the number of users on the site. The next line contains integer sequence <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>.</p>

## Output

<p>Print a sequence of integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span>. Number <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> means that user <span class="tex-span"><i>i</i></span> gets <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> of rating as a present. The printed sequence must meet the problem conditions. </p><p>If there are multiple optimal solutions, print any of them.</p>





```input1
3
5 1 1

```




```input2
1
1000000000

```




```output1
5 1 2

```




```output2
1000000000

```


