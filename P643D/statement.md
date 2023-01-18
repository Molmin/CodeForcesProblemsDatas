## Description

<div><p>There is a social website with <span class="tex-span"><i>n</i></span> fanpages, numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>. There are also <span class="tex-span"><i>n</i></span> companies, and the <span class="tex-span"><i>i</i></span>-th company owns the <span class="tex-span"><i>i</i></span>-th fanpage.</p><p>Recently, the website created a feature called following. Each fanpage must choose exactly one other fanpage to follow.</p><p>The website doesn’t allow a situation where <span class="tex-span"><i>i</i></span> follows <span class="tex-span"><i>j</i></span> and at the same time <span class="tex-span"><i>j</i></span> follows <span class="tex-span"><i>i</i></span>. Also, a fanpage can't follow itself.</p><p>Let’s say that fanpage <span class="tex-span"><i>i</i></span> follows some other fanpage <span class="tex-span"><i>j</i><sub class="lower-index">0</sub></span>. Also, let’s say that <span class="tex-span"><i>i</i></span> is followed by <span class="tex-span"><i>k</i></span> other fanpages <span class="tex-span"><i>j</i><sub class="lower-index">1</sub>, <i>j</i><sub class="lower-index">2</sub>, ..., <i>j</i><sub class="lower-index"><i>k</i></sub></span>. Then, when people visit fanpage <span class="tex-span"><i>i</i></span> they see ads from <span class="tex-span"><i>k</i> + 2</span> distinct companies: <span class="tex-span"><i>i</i>, <i>j</i><sub class="lower-index">0</sub>, <i>j</i><sub class="lower-index">1</sub>, ..., <i>j</i><sub class="lower-index"><i>k</i></sub></span>. Exactly <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> people subscribe (like) the <span class="tex-span"><i>i</i></span>-th fanpage, and each of them will click exactly one add. For each of <span class="tex-span"><i>k</i> + 1</span> companies <span class="tex-span"><i>j</i><sub class="lower-index">0</sub>, <i>j</i><sub class="lower-index">1</sub>, ..., <i>j</i><sub class="lower-index"><i>k</i></sub></span>, exactly <img align="middle" class="tex-formula" src="file://14r07zlc.png" style="max-width: 100.0%;max-height: 100.0%;"> people will click their ad. Remaining <img align="middle" class="tex-formula" src="file://pLhhiclw.png" style="max-width: 100.0%;max-height: 100.0%;"> people will click an ad from company <span class="tex-span"><i>i</i></span> (the owner of the fanpage).</p><p>The total income of the company is equal to the number of people who click ads from this copmany.</p><p>Limak and Radewoosh ask you for help. Initially, fanpage <span class="tex-span"><i>i</i></span> follows fanpage <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>. Your task is to handle <span class="tex-span"><i>q</i></span> queries of three types:</p><ul> <li> <span class="tex-font-style-tt">1 i j</span>&nbsp;— fanpage <span class="tex-span"><i>i</i></span> follows fanpage <span class="tex-span"><i>j</i></span> from now. It's guaranteed that <span class="tex-span"><i>i</i></span> didn't follow <span class="tex-span"><i>j</i></span> just before the query. Note an extra constraint for the number of queries of this type (below, in the Input section). </li><li> <span class="tex-font-style-tt">2 i</span>&nbsp;— print the total income of the <span class="tex-span"><i>i</i></span>-th company. </li><li> <span class="tex-font-style-tt">3</span>&nbsp;— print two integers: the smallest income of one company and the biggest income of one company. </li></ul></div><div class="input-specification"><p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>)&nbsp;— the number of fanpages and the number of queries, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> denotes the number of people subscribing the <span class="tex-span"><i>i</i></span>-th fanpage.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). Initially, fanpage <span class="tex-span"><i>i</i></span> follows fanpage <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Then, <span class="tex-span"><i>q</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them describes the <span class="tex-span"><i>i</i></span>-th query. The first number in the line is an integer <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>)&nbsp;— the type of the query.</p><p>There will be at most <span class="tex-span">50 000</span> queries of the first type. There will be at least one query of the second or the third type (so, the output won't be empty).</p><p>It's guaranteed that at each moment a fanpage doesn't follow itself, and that no two fanpages follow each other.</p></div><div class="output-specification"><p>For each query of the second type print one integer in a separate line - the total income of the given company. For each query of the third type print two integers in a separate line - the minimum and the maximum total income, respectively.</p></div>

## Input

<p>The first line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 100 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 100 000</span>)&nbsp;— the number of fanpages and the number of queries, respectively.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub>, <i>t</i><sub class="lower-index">2</sub>, ..., <i>t</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">12</sup></span>) where <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> denotes the number of people subscribing the <span class="tex-span"><i>i</i></span>-th fanpage.</p><p>The third line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>f</i><sub class="lower-index">1</sub>, <i>f</i><sub class="lower-index">2</sub>, ..., <i>f</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>f</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). Initially, fanpage <span class="tex-span"><i>i</i></span> follows fanpage <span class="tex-span"><i>f</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>Then, <span class="tex-span"><i>q</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them describes the <span class="tex-span"><i>i</i></span>-th query. The first number in the line is an integer <span class="tex-span"><i>type</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>type</i><sub class="lower-index"><i>i</i></sub> ≤ 3</span>)&nbsp;— the type of the query.</p><p>There will be at most <span class="tex-span">50 000</span> queries of the first type. There will be at least one query of the second or the third type (so, the output won't be empty).</p><p>It's guaranteed that at each moment a fanpage doesn't follow itself, and that no two fanpages follow each other.</p>

## Output

<p>For each query of the second type print one integer in a separate line - the total income of the given company. For each query of the third type print two integers in a separate line - the minimum and the maximum total income, respectively.</p>





```input1
5 12
10 20 30 40 50
2 3 4 5 2
2 1
2 2
2 3
2 4
2 5
1 4 2
2 1
2 2
2 3
2 4
2 5
3

```




```output1
10
36
28
40
36
9
57
27
28
29
9 57

```



## Note

<center> <img class="tex-graphics" src="file://QDr8qsQs.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>In the sample test, there are <span class="tex-span">5</span> fanpages. The <span class="tex-span"><i>i</i></span>-th of them has <span class="tex-span"><i>i</i>·10</span> subscribers.</p><p>On drawings, numbers of subscribers are written in circles. An arrow from <span class="tex-span"><i>A</i></span> to <span class="tex-span"><i>B</i></span> means that <span class="tex-span"><i>A</i></span> follows <span class="tex-span"><i>B</i></span>.</p><p>The left drawing shows the initial situation. The first company gets income <img align="middle" class="tex-formula" src="file://PZX0vtVG.png" style="max-width: 100.0%;max-height: 100.0%;"> from its own fanpage, and gets income <img align="middle" class="tex-formula" src="file://bbeAJcef.png" style="max-width: 100.0%;max-height: 100.0%;"> from the <span class="tex-span">2</span>-nd fanpage. So, the total income is <span class="tex-span">5 + 5 = 10</span>. After the first query ("<span class="tex-font-style-tt">2 1</span>") you should print <span class="tex-span">10</span>.</p><p>The right drawing shows the situation after a query "<span class="tex-font-style-tt">1 4 2</span>" (after which fanpage <span class="tex-span">4</span> follows fanpage <span class="tex-span">2</span>). Then, the first company still gets income <span class="tex-span">5</span> from its own fanpage, but now it gets only <img align="middle" class="tex-formula" src="file://gTVnVAv2.png" style="max-width: 100.0%;max-height: 100.0%;"> from the <span class="tex-span">2</span>-nd fanpage. So, the total income is <span class="tex-span">5 + 4 = 9</span> now.</p>
