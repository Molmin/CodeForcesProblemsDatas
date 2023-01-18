## Description

<div><p>Misha and Grisha are funny boys, so they like to use new underground. The underground has <span class="tex-span"><i>n</i></span> stations connected with <span class="tex-span"><i>n</i> - 1</span> routes so that each route connects two stations, and it is possible to reach every station from any other.</p><p>The boys decided to have fun and came up with a plan. Namely, in some day in the morning Misha will ride the underground from station <span class="tex-span"><i>s</i></span> to station <span class="tex-span"><i>f</i></span> by the shortest path, and will draw with aerosol an ugly text "Misha was here" on every station he will pass through (including <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>f</i></span>). After that on the same day at evening Grisha will ride from station <span class="tex-span"><i>t</i></span> to station <span class="tex-span"><i>f</i></span> by the shortest path and will count stations with Misha's text. After that at night the underground workers will wash the texts out, because the underground should be clean. </p><p>The boys have already chosen three stations <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> for each of several following days, one of them should be station <span class="tex-span"><i>s</i></span> on that day, another should be station <span class="tex-span"><i>f</i></span>, and the remaining should be station <span class="tex-span"><i>t</i></span>. They became interested how they should choose these stations <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>f</i></span>, <span class="tex-span"><i>t</i></span> so that the number Grisha will count is as large as possible. They asked you for help.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of stations and the number of days.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). The integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> means that there is a route between stations <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>i</i></span>. It is guaranteed that it's possible to reach every station from any other.</p><p>The next <span class="tex-span"><i>q</i></span> lines contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> each (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ <i>n</i></span>)&nbsp;— the ids of stations chosen by boys for some day. Note that some of these ids could be same.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th of these lines print the maximum possible number Grisha can get counting when the stations <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>f</i></span> are chosen optimally from the three stations on the <span class="tex-span"><i>i</i></span>-th day.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>q</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 10<sup class="upper-index">5</sup></span>)&nbsp;— the number of stations and the number of days.</p><p>The second line contains <span class="tex-span"><i>n</i> - 1</span> integers <span class="tex-span"><i>p</i><sub class="lower-index">2</sub>, <i>p</i><sub class="lower-index">3</sub>, ..., <i>p</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>). The integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> means that there is a route between stations <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>i</i></span>. It is guaranteed that it's possible to reach every station from any other.</p><p>The next <span class="tex-span"><i>q</i></span> lines contains three integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> each (<span class="tex-span">1 ≤ <i>a</i>, <i>b</i>, <i>c</i> ≤ <i>n</i></span>)&nbsp;— the ids of stations chosen by boys for some day. Note that some of these ids could be same.</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> lines. In the <span class="tex-span"><i>i</i></span>-th of these lines print the maximum possible number Grisha can get counting when the stations <span class="tex-span"><i>s</i></span>, <span class="tex-span"><i>t</i></span> and <span class="tex-span"><i>f</i></span> are chosen optimally from the three stations on the <span class="tex-span"><i>i</i></span>-th day.</p>





```input1
3 2
1 1
1 2 3
2 3 3

```




```input2
4 1
1 2 3
1 2 3

```




```output1
2
3

```




```output2
2

```



## Note

<p>In the first example on the first day if <span class="tex-span"><i>s</i></span> = <span class="tex-span">1</span>, <span class="tex-span"><i>f</i></span> = <span class="tex-span">2</span>, <span class="tex-span"><i>t</i></span> = <span class="tex-span">3</span>, Misha would go on the route <span class="tex-span">1</span> <img align="middle" class="tex-formula" src="file://A5vk0XXp.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">2</span>, and Grisha would go on the route <span class="tex-span">3</span> <img align="middle" class="tex-formula" src="file://0gBadZV5.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">1</span> <img align="middle" class="tex-formula" src="file://XoQBx3n7.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">2</span>. He would see the text at the stations <span class="tex-span">1</span> and <span class="tex-span">2</span>. On the second day, if <span class="tex-span"><i>s</i></span> = <span class="tex-span">3</span>, <span class="tex-span"><i>f</i></span> = <span class="tex-span">2</span>, <span class="tex-span"><i>t</i></span> = <span class="tex-span">3</span>, both boys would go on the route <span class="tex-span">3</span> <img align="middle" class="tex-formula" src="file://wbjAcxJL.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">1</span> <img align="middle" class="tex-formula" src="file://vJlAjhs7.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">2</span>. Grisha would see the text at <span class="tex-span">3</span> stations.</p><p>In the second examle if <span class="tex-span"><i>s</i></span> = <span class="tex-span">1</span>, <span class="tex-span"><i>f</i></span> = <span class="tex-span">3</span>, <span class="tex-span"><i>t</i></span> = <span class="tex-span">2</span>, Misha would go on the route <span class="tex-span">1</span> <img align="middle" class="tex-formula" src="file://8u2l76LW.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">2</span> <img align="middle" class="tex-formula" src="file://G5igU2AZ.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">3</span>, and Grisha would go on the route <span class="tex-span">2</span> <img align="middle" class="tex-formula" src="file://YwgLNf3B.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">3</span> and would see the text at both stations.</p>
