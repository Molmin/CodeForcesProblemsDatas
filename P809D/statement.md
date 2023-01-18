## Description

<div><p>Leha and Noora decided to go on a trip in the Baltic States. As you know from the previous problem, Leha has lost his car on the parking of the restaurant. Unfortunately, requests to the watchman didn't helped hacker find the car, so friends decided to go hitchhiking.</p><p>In total, they intended to visit <span class="tex-span"><i>n</i></span> towns. However it turned out that sights in <span class="tex-span"><i>i</i></span>-th town are open for visitors only on days from <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> to <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>What to do? Leha proposed to choose for each town <span class="tex-span"><i>i</i></span> a day, when they will visit this town, i.e any integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> in interval <span class="tex-span">[<i>l</i><sub class="lower-index"><i>i</i></sub>, <i>r</i><sub class="lower-index"><i>i</i></sub>]</span>. After that Noora choses some subsequence of towns <span class="tex-span"><i>id</i><sub class="lower-index">1</sub>, <i>id</i><sub class="lower-index">2</sub>, ..., <i>id</i><sub class="lower-index"><i>k</i></sub></span>, which friends are going to visit, that at first they are strictly increasing, i.e <span class="tex-span"><i>id</i><sub class="lower-index"><i>i</i></sub> &lt; <i>id</i><sub class="lower-index"><i>i</i> + 1</sub></span> is for all integers <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i> - 1</span>, but also the dates of the friends visits are strictly increasing, i.e <span class="tex-span"><i>x</i><sub class="lower-index"><i>id</i><sub class="lower-index"><i>i</i></sub></sub> &lt; <i>x</i><sub class="lower-index"><i>id</i><sub class="lower-index"><i>i</i> + 1</sub></sub></span> is true for all integers <span class="tex-span"><i>i</i></span> from <span class="tex-span">1</span> to <span class="tex-span"><i>k</i> - 1</span>.</p><p>Please help Leha and Noora in choosing such <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> for each town <span class="tex-span"><i>i</i></span>, and such subsequence of towns <span class="tex-span"><i>id</i><sub class="lower-index">1</sub>, <i>id</i><sub class="lower-index">2</sub>, ..., <i>id</i><sub class="lower-index"><i>k</i></sub></span>, so that friends can visit maximal number of towns.</p><p>You may assume, that Leha and Noora can start the trip any day.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) denoting the number of towns Leha and Noora intended to visit.</p><p>Each line <span class="tex-span"><i>i</i></span> of the <span class="tex-span"><i>n</i></span> subsequent lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, denoting that sights in <span class="tex-span"><i>i</i></span>-th town are open for visitors on any day <img align="middle" class="tex-formula" src="file://nHaORBnq.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div><div class="output-specification"><p>Print a single integer denoting the maximal number of towns, that Leha and Noora can visit.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 3·10<sup class="upper-index">5</sup></span>) denoting the number of towns Leha and Noora intended to visit.</p><p>Each line <span class="tex-span"><i>i</i></span> of the <span class="tex-span"><i>n</i></span> subsequent lines contains two integers <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup>)</span>, denoting that sights in <span class="tex-span"><i>i</i></span>-th town are open for visitors on any day <img align="middle" class="tex-formula" src="file://nHaORBnq.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>

## Output

<p>Print a single integer denoting the maximal number of towns, that Leha and Noora can visit.</p>





```input1
5
6 6
1 2
3 4
2 2
1 4

```




```output1
3

```



## Note

<p>Consider the first example.</p><p>Let's take this plan: let's visit the sight in the second town on the first day, in the third town on the third day and in the fifth town on the fourth. That's would be the optimal answer.</p>
