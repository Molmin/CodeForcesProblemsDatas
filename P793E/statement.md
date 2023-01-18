## Description

<div><p>Earlier, when there was no Internet, each bank had a lot of offices all around Bankopolis, and it caused a lot of problems. Namely, each day the bank had to collect cash from all the offices.</p><p>Once Oleg the bank client heard a dialogue of two cash collectors. Each day they traveled through all the departments and offices of the bank following the same route every day. The collectors started from the central department and moved between some departments or between some department and some office using special roads. Finally, they returned to the central department. The total number of departments and offices was <span class="tex-span"><i>n</i></span>, the total number of roads was <span class="tex-span"><i>n</i> - 1</span>. In other words, the special roads system was a rooted tree in which the root was the central department, the leaves were offices, the internal vertices were departments. The collectors always followed the same route in which the number of roads was minimum possible, that is <span class="tex-span">2<i>n</i> - 2</span>.</p><p>One of the collectors said that the number of offices they visited between their visits to offices <span class="tex-span"><i>a</i></span> and then <span class="tex-span"><i>b</i></span> (in the given order) is equal to the number of offices they visited between their visits to offices <span class="tex-span"><i>b</i></span> and then <span class="tex-span"><i>a</i></span> (in this order). The other collector said that the number of offices they visited between their visits to offices <span class="tex-span"><i>c</i></span> and then <span class="tex-span"><i>d</i></span> (in this order) is equal to the number of offices they visited between their visits to offices <span class="tex-span"><i>d</i></span> and then <span class="tex-span"><i>c</i></span> (in this order). The interesting part in this talk was that the shortest path (using special roads only) between any pair of offices among <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> <span class="tex-font-style-bf">passed through the central department</span>.</p><p>Given the special roads map and the indexes of offices <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span>, determine if the situation described by the collectors was possible, or not.</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the total number of offices and departments. The departments and offices are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, the central office has index <span class="tex-span">1</span>.</p><p>The second line contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">2 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ <i>n</i></span>)&nbsp;— the indexes of the departments mentioned in collector's dialogue. It is guaranteed that these indexes are offices (i.e. leaves of the tree), not departments. It is guaranteed that the shortest path between any pair of these offices passes through the central department.</p><p>On the third line <span class="tex-span"><i>n</i> - 1</span> integers follow: <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> denotes that there is a special road between the <span class="tex-span"><i>i</i></span>-th office or department and the <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>-th department.</p><p>Please note the joint enumeration of departments and offices.</p><p>It is guaranteed that the given graph is a tree. The offices are the leaves, the departments are the internal vertices.</p></div><div class="output-specification"><p>If the situation described by the cash collectors was possible, print "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">5 ≤ <i>n</i> ≤ 5000</span>)&nbsp;— the total number of offices and departments. The departments and offices are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, the central office has index <span class="tex-span">1</span>.</p><p>The second line contains four integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">2 ≤ <i>a</i>, <i>b</i>, <i>c</i>, <i>d</i> ≤ <i>n</i></span>)&nbsp;— the indexes of the departments mentioned in collector's dialogue. It is guaranteed that these indexes are offices (i.e. leaves of the tree), not departments. It is guaranteed that the shortest path between any pair of these offices passes through the central department.</p><p>On the third line <span class="tex-span"><i>n</i> - 1</span> integers follow: <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span>), where <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> denotes that there is a special road between the <span class="tex-span"><i>i</i></span>-th office or department and the <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>-th department.</p><p>Please note the joint enumeration of departments and offices.</p><p>It is guaranteed that the given graph is a tree. The offices are the leaves, the departments are the internal vertices.</p>

## Output

<p>If the situation described by the cash collectors was possible, print "<span class="tex-font-style-tt">YES</span>". Otherwise, print "<span class="tex-font-style-tt">NO</span>".</p>





```input1
5
2 3 4 5
1 1 1 1

```




```input2
10
3 8 9 10
1 2 2 2 2 2 1 1 1

```




```input3
13
13 12 9 7
1 1 1 1 5 5 2 2 2 3 3 4

```




```output1
YES
```




```output2
NO
```




```output3
YES
```



## Note

<p>In the first example the following collector's route was possible: <img align="middle" class="tex-formula" src="file://rBev56wy.png" style="max-width: 100.0%;max-height: 100.0%;">. We can note that between their visits to offices <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> the collectors visited the same number of offices as between visits to offices <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>a</i></span>; the same holds for <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> (the collectors' route is infinite as they follow it each day).</p><p>In the second example there is no route such that between their visits to offices <span class="tex-span"><i>c</i></span> and <span class="tex-span"><i>d</i></span> the collectors visited the same number of offices as between visits to offices <span class="tex-span"><i>d</i></span> and <span class="tex-span"><i>c</i></span>. Thus, there situation is impossible. </p><p>In the third example one of the following routes is: <img align="middle" class="tex-formula" src="file://Y2qTsP8L.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
