## Description

<div><p>Hiasat registered a new account in NeckoForces and when his friends found out about that, each one of them asked to use his name as Hiasat's handle.</p><p>Luckily for Hiasat, he can change his handle in some points in time. Also he knows the exact moments friends will visit his profile page. Formally, you are given a sequence of events of two types:</p><ul> <li> $1$&nbsp;— Hiasat can change his handle. </li><li> $2$ $s$&nbsp;— friend $s$ visits Hiasat's profile. </li></ul><p>The friend $s$ will be happy, if each time he visits Hiasat's profile his handle would be $s$.</p><p>Hiasat asks you to help him, find the maximum possible number of happy friends he can get.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $m$ ($1 \le n \le 10^5, 1 \le m \le 40$)&nbsp;— the number of events and the number of friends.</p><p>Then $n$ lines follow, each denoting an event of one of two types: </p><ul> <li> $1$&nbsp;— Hiasat can change his handle. </li><li> $2$ $s$&nbsp;— friend $s$ ($1 \le |s| \le 40$) visits Hiasat's profile. </li></ul><p>It's guaranteed, that each friend's name consists only of lowercase Latin letters.</p><p>It's guaranteed, that the first event is always of the first type and each friend will visit Hiasat's profile at least once.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the maximum number of happy friends.</p></div>

## Input

<p>The first line contains two integers $n$ and $m$ ($1 \le n \le 10^5, 1 \le m \le 40$)&nbsp;— the number of events and the number of friends.</p><p>Then $n$ lines follow, each denoting an event of one of two types: </p><ul> <li> $1$&nbsp;— Hiasat can change his handle. </li><li> $2$ $s$&nbsp;— friend $s$ ($1 \le |s| \le 40$) visits Hiasat's profile. </li></ul><p>It's guaranteed, that each friend's name consists only of lowercase Latin letters.</p><p>It's guaranteed, that the first event is always of the first type and each friend will visit Hiasat's profile at least once.</p>

## Output

<p>Print a single integer&nbsp;— the maximum number of happy friends.</p>





```input1
5 3
1
2 motarack
2 mike
1
2 light
```




```input2
4 3
1
2 alice
2 bob
2 tanyaromanova
```




```output1
2
```




```output2
1
```



## Note

<p>In the first example, the best way is to change the handle to the "<span class="tex-font-style-tt">motarack</span>" in the first event and to the "<span class="tex-font-style-tt">light</span>" in the fourth event. This way, "<span class="tex-font-style-tt">motarack</span>" and "<span class="tex-font-style-tt">light</span>" will be happy, but "<span class="tex-font-style-tt">mike</span>" will not.</p><p>In the second example, you can choose either "<span class="tex-font-style-tt">alice</span>", "<span class="tex-font-style-tt">bob</span>" or "<span class="tex-font-style-tt">tanyaromanova</span>" and only that friend will be happy.</p>
