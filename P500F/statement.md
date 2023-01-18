## Description

<div><p>Dohyun is running a grocery store. He sells <span class="tex-span"><i>n</i></span> items numbered by integers from 1 to <span class="tex-span"><i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) of them costs <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> dollars, and if I buy it, my happiness increases by <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>. Each item can be displayed only for <span class="tex-span"><i>p</i></span> units of time because of freshness. As Dohyun displays the <span class="tex-span"><i>i</i></span>-th item at time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span>, the customers can buy the <span class="tex-span"><i>i</i></span>-th item only from time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> to time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub> + (<i>p</i> - 1)</span> inclusively. Also, each customer cannot buy the same item more than once.</p><p>I'd like to visit Dohyun's grocery store and buy some items for the New Year Party, and maximize my happiness. Because I am a really busy person, I can visit the store only once, and for very short period of time. In other words, if I visit the store at time <span class="tex-span"><i>t</i></span>, I can only buy the items available at time <span class="tex-span"><i>t</i></span>. But I can buy as many items as possible, if the budget holds. I can't buy same item several times due to store rules. It is not necessary to use the whole budget.</p><p>I made a list of <span class="tex-span"><i>q</i></span> pairs of integers <span class="tex-span">(<i>a</i><sub class="lower-index"><i>j</i></sub>, <i>b</i><sub class="lower-index"><i>j</i></sub>)</span>, which means I may visit the store at time <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, and spend at most <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> dollars at the store. For each pair, I'd like to know the maximum happiness I can obtain. But there are so many pairs that I can't handle them. Can you help me?</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4000</span>, <span class="tex-span">1 ≤ <i>p</i> ≤ 10 000</span>) — the number of items, and the display time of each item.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the items. The <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) of them contains three space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 4000</span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>) — the cost of the <span class="tex-span"><i>i</i></span>-th item, the happiness of the <span class="tex-span"><i>i</i></span>-th item, and the time when the <span class="tex-span"><i>i</i></span>-th item starts to be displayed.</p><p>The next line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 20 000</span>)— the number of candidates.</p><p>Next <span class="tex-span"><i>q</i></span> lines describe the candidates. The <span class="tex-span"><i>j</i></span>-th (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>q</i></span>) of them contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ 20 000</span>, <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 4000</span>) — the visit time and the budget for <span class="tex-span"><i>j</i></span>-th visit of store.</p></div><div class="output-specification"><p>For each candidate, print a single line containing the maximum happiness that I can obtain by buying some items.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 4000</span>, <span class="tex-span">1 ≤ <i>p</i> ≤ 10 000</span>) — the number of items, and the display time of each item.</p><p>Next <span class="tex-span"><i>n</i></span> lines describe the items. The <span class="tex-span"><i>i</i></span>-th (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) of them contains three space-separated integers <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>h</i><sub class="lower-index"><i>i</i></sub> ≤ 4000</span>, <span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>) — the cost of the <span class="tex-span"><i>i</i></span>-th item, the happiness of the <span class="tex-span"><i>i</i></span>-th item, and the time when the <span class="tex-span"><i>i</i></span>-th item starts to be displayed.</p><p>The next line contains an integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 20 000</span>)— the number of candidates.</p><p>Next <span class="tex-span"><i>q</i></span> lines describe the candidates. The <span class="tex-span"><i>j</i></span>-th (<span class="tex-span">1 ≤ <i>j</i> ≤ <i>q</i></span>) of them contains two space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>, <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>j</i></sub> ≤ 20 000</span>, <span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 4000</span>) — the visit time and the budget for <span class="tex-span"><i>j</i></span>-th visit of store.</p>

## Output

<p>For each candidate, print a single line containing the maximum happiness that I can obtain by buying some items.</p>





```input1
4 4
2 3 2
3 5 1
4 7 2
11 15 5
4
1 3
2 5
2 6
5 14

```




```input2
5 4
3 2 1
7 4 4
2 1 2
6 3 5
3 2 2
10
1 5
2 5
4 8
4 9
4 10
5 8
5 9
5 10
8 4
7 9

```




```output1
5
8
10
18

```




```output2
2
3
5
5
6
4
5
6
0
4

```



## Note

<p>Consider the first sample. </p><center> <img class="tex-graphics" src="file://TsP70vfH.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><ol> <li> At time 1, only the 2nd item is available. I can buy the 2nd item using 3 dollars and my happiness will increase by 5. </li><li> At time 2, the 1st, 2nd, and 3rd item is available. I can buy the 1st item using 2 dollars, and the 2nd item using 3 dollars. My happiness will increase by 3 + 5 = 8. </li><li> At time 2, the 1st, 2nd, and 3rd item is available. I can buy the 1st item using 2 dollars, and the 3nd item using 4 dollars. My happiness will increase by 3 + 7 = 10. </li><li> At time 5, the 1st, 3rd, and 4th item is available. I can buy the 1st item using 2 dollars, and the 4th item using 11 dollars. My happiness will increase by 3 + 15 = 18. Note that I don't need to use the whole budget in this case. </li></ol>
