## Description

<div><p><span class="tex-font-style-it">Just to remind, girls in Arpa's land are really nice.</span></p><p>Mehrdad wants to invite some Hoses to the palace for a dancing party. Each Hos has some weight <span class="tex-span"><i>w</i><sub class="lower-index"><i>i</i></sub></span> and some beauty <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span>. Also each Hos may have some friends. Hoses are divided in some friendship groups. Two Hoses <span class="tex-span"><i>x</i></span> and <span class="tex-span"><i>y</i></span> are in the same friendship group if and only if there is a sequence of Hoses <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>k</i></sub></span> such that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i> + 1</sub></span> are friends for each <span class="tex-span">1 ≤ <i>i</i> &lt; <i>k</i></span>, and <span class="tex-span"><i>a</i><sub class="lower-index">1</sub> = <i>x</i></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>k</i></sub> = <i>y</i></span>.</p><center> <img class="tex-graphics" height="222px" src="file://4AgE06fw.png" style="max-width: 100.0%;max-height: 100.0%;" width="172px"> </center><p>Arpa allowed to use the amphitheater of palace to Mehrdad for this party. Arpa's amphitheater can hold at most <span class="tex-span"><i>w</i></span> weight on it. </p><p>Mehrdad is so greedy that he wants to invite some Hoses such that sum of their weights is not greater than <span class="tex-span"><i>w</i></span> and sum of their beauties is as large as possible. Along with that, from each friendship group he can either invite all Hoses, or no more than one. Otherwise, some Hoses will be hurt. Find for Mehrdad the maximum possible total beauty of Hoses he can invite so that no one gets hurt and the total weight doesn't exceed <span class="tex-span"><i>w</i></span>.</p></div><div class="input-specification"><p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1  ≤  <i>n</i>  ≤  1000</span>, <img align="middle" class="tex-formula" src="file://qEby1h1A.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span">1 ≤ <i>w</i> ≤ 1000</span>)&nbsp;— the number of Hoses, the number of pair of friends and the maximum total weight of those who are invited.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;— the weights of the Hoses.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the beauties of the Hoses.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain pairs of friends, the <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>), meaning that Hoses <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are friends. Note that friendship is bidirectional. All pairs <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> are distinct.</p></div><div class="output-specification"><p>Print the maximum possible total beauty of Hoses Mehrdad can invite so that no one gets hurt and the total weight doesn't exceed <span class="tex-span"><i>w</i></span>.</p></div>

## Input

<p>The first line contains integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>m</i></span> and <span class="tex-span"><i>w</i></span> (<span class="tex-span">1  ≤  <i>n</i>  ≤  1000</span>, <img align="middle" class="tex-formula" src="file://qEby1h1A.png" style="max-width: 100.0%;max-height: 100.0%;">, <span class="tex-span">1 ≤ <i>w</i> ≤ 1000</span>)&nbsp;— the number of Hoses, the number of pair of friends and the maximum total weight of those who are invited.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>w</i><sub class="lower-index">1</sub>, <i>w</i><sub class="lower-index">2</sub>, ..., <i>w</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>w</i><sub class="lower-index"><i>i</i></sub> ≤ 1000</span>)&nbsp;— the weights of the Hoses.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>)&nbsp;— the beauties of the Hoses.</p><p>The next <span class="tex-span"><i>m</i></span> lines contain pairs of friends, the <span class="tex-span"><i>i</i></span>-th of them contains two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≠ <i>y</i><sub class="lower-index"><i>i</i></sub></span>), meaning that Hoses <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> are friends. Note that friendship is bidirectional. All pairs <span class="tex-span">(<i>x</i><sub class="lower-index"><i>i</i></sub>, <i>y</i><sub class="lower-index"><i>i</i></sub>)</span> are distinct.</p>

## Output

<p>Print the maximum possible total beauty of Hoses Mehrdad can invite so that no one gets hurt and the total weight doesn't exceed <span class="tex-span"><i>w</i></span>.</p>





```input1
3 1 5
3 2 5
2 4 2
1 2

```




```input2
4 2 11
2 4 6 6
6 4 2 1
1 2
2 3

```




```output1
6

```




```output2
7

```



## Note

<p>In the first sample there are two friendship groups: Hoses <span class="tex-span">{1, 2}</span> and Hos <span class="tex-span">{3}</span>. The best way is to choose all of Hoses in the first group, sum of their weights is equal to <span class="tex-span">5</span> and sum of their beauty is <span class="tex-span">6</span>.</p><p>In the second sample there are two friendship groups: Hoses <span class="tex-span">{1, 2, 3}</span> and Hos <span class="tex-span">{4}</span>. Mehrdad can't invite all the Hoses from the first group because their total weight is <span class="tex-span">12 &gt; 11</span>, thus the best way is to choose the first Hos from the first group and the only one from the second group. The total weight will be <span class="tex-span">8</span>, and the total beauty will be <span class="tex-span">7</span>.</p>
