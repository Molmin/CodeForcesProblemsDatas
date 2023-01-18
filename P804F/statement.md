## Description

<div><p>In Isart people don't die. There are <span class="tex-span"><i>n</i></span> gangs of criminals. The <span class="tex-span"><i>i</i></span>-th gang contains <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> evil people numerated from <span class="tex-span">0</span> to <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub> - 1</span>. Some of these people took part in a big mine robbery and picked <span class="tex-font-style-bf">one</span> gold bullion each (these people are given in the input). That happened <span class="tex-span">10<sup class="upper-index">100</sup></span> years ago and then all of the gangs escaped to a remote area, far from towns.</p><p>During the years, they were copying some gold bullions according to an organized plan in order to not get arrested. They constructed a <span class="tex-font-style-bf">tournament</span> directed graph (a graph where there is exactly one directed edge between every pair of vertices) of gangs (the graph is given in the input). In this graph an edge from <span class="tex-span"><i>u</i></span> to <span class="tex-span"><i>v</i></span> means that in the <span class="tex-span"><i>i</i></span>-th hour the person <img align="middle" class="tex-formula" src="file://3s6XA13S.png" style="max-width: 100.0%;max-height: 100.0%;"> of the gang <span class="tex-span"><i>u</i></span> can send a fake gold bullion to person <img align="middle" class="tex-formula" src="file://VafrJmhq.png" style="max-width: 100.0%;max-height: 100.0%;"> of gang <span class="tex-span"><i>v</i></span>. He sends it if he has some bullion (real or fake), while the receiver doesn't have any. Thus, at any moment each of the gangsters has zero or one gold bullion. Some of them have real bullions, and some of them have fake ones.</p><p>In the beginning of this year, the police has finally found the gangs, but they couldn't catch them, as usual. The police decided to open a jewelry store so that the gangsters would sell the bullions. Thus, every gangster that has a bullion (fake or real) will try to sell it. If he has a real gold bullion, he sells it without problems, but if he has a fake one, there is a choice of two events that can happen: </p><ul> <li> The person sells the gold bullion successfully. </li><li> The person is arrested by police. </li></ul><p>The power of a gang is the number of people in it that successfully sold their bullion. After all selling is done, the police arrests <span class="tex-span"><i>b</i></span> gangs out of <span class="tex-font-style-it">top</span> gangs. Sort the gangs by powers, we call the first <span class="tex-span"><i>a</i></span> gang <span class="tex-font-style-it">top</span> gangs(you can sort the equal powers in each order). Consider all possible results of selling fake gold bullions and all possible choice of <span class="tex-span"><i>b</i></span> gangs among the <span class="tex-font-style-it">top</span> gangs. Count the number of different sets of these <span class="tex-span"><i>b</i></span> gangs modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. Two sets <span class="tex-span"><i>X</i></span> and <span class="tex-span"><i>Y</i></span> are considered different if some gang is in <span class="tex-span"><i>X</i></span> and isn't in <span class="tex-span"><i>Y</i></span>.</p></div><div class="input-specification"><p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ <i>a</i> ≤ <i>n</i> ≤ 5·10<sup class="upper-index">3</sup></span>)&nbsp;— the number of gangs, the constants <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> from the statement.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line contains a string of size <span class="tex-span"><i>n</i></span> consisting of zeros and ones. The <span class="tex-span"><i>j</i></span>-th character in the <span class="tex-span"><i>i</i></span>-th of these lines is equal to <span class="tex-span">1</span>, then the vertex <span class="tex-span"><i>i</i></span> have a directed edge to the vertex <span class="tex-span"><i>j</i></span>. It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>ii</i></sub> = 0</span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> + <i>a</i><sub class="lower-index"><i>ji</i></sub> = 1</span> if <span class="tex-span"><i>i</i> ≠ <i>j</i></span>.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line starts with the integer <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">6</sup></span>)&nbsp;— the number of gangsters in the <span class="tex-span"><i>i</i></span>-th gang, and then contains a string of zeros and ones with length <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. The <span class="tex-span"><i>j</i></span>-th character is <span class="tex-span">0</span> if the <span class="tex-span"><i>j</i></span>-th person of the <span class="tex-span"><i>i</i></span>-th gang had a real gold bullion initially, otherwise it is <span class="tex-span">1</span>. It is guaranteed that the sum of <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> does not exceed <span class="tex-span">2·10<sup class="upper-index">6</sup></span>.</p></div><div class="output-specification"><p>Print single integer: the number of different sets of <span class="tex-span"><i>b</i></span> gangs the police can arrest modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains four integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>b</i> ≤ <i>a</i> ≤ <i>n</i> ≤ 5·10<sup class="upper-index">3</sup></span>)&nbsp;— the number of gangs, the constants <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> from the statement.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line contains a string of size <span class="tex-span"><i>n</i></span> consisting of zeros and ones. The <span class="tex-span"><i>j</i></span>-th character in the <span class="tex-span"><i>i</i></span>-th of these lines is equal to <span class="tex-span">1</span>, then the vertex <span class="tex-span"><i>i</i></span> have a directed edge to the vertex <span class="tex-span"><i>j</i></span>. It is guaranteed that <span class="tex-span"><i>a</i><sub class="lower-index"><i>ii</i></sub> = 0</span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>ij</i></sub> + <i>a</i><sub class="lower-index"><i>ji</i></sub> = 1</span> if <span class="tex-span"><i>i</i> ≠ <i>j</i></span>.</p><p>Then <span class="tex-span"><i>n</i></span> lines follow, each line starts with the integer <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>s</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">6</sup></span>)&nbsp;— the number of gangsters in the <span class="tex-span"><i>i</i></span>-th gang, and then contains a string of zeros and ones with length <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span>. The <span class="tex-span"><i>j</i></span>-th character is <span class="tex-span">0</span> if the <span class="tex-span"><i>j</i></span>-th person of the <span class="tex-span"><i>i</i></span>-th gang had a real gold bullion initially, otherwise it is <span class="tex-span">1</span>. It is guaranteed that the sum of <span class="tex-span"><i>s</i><sub class="lower-index"><i>i</i></sub></span> does not exceed <span class="tex-span">2·10<sup class="upper-index">6</sup></span>.</p>

## Output

<p>Print single integer: the number of different sets of <span class="tex-span"><i>b</i></span> gangs the police can arrest modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
2 2 1
01
00
5 11000
6 100000

```




```input2
5 2 1
00000
10000
11011
11000
11010
2 00
1 1
6 100110
1 0
1 0

```




```output1
2

```




```output2
5

```


