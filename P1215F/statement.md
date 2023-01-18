## Description

<div><p>In addition to complaints about lighting, a lot of complaints about insufficient radio signal covering has been received by Bertown city hall recently. $n$ complaints were sent to the mayor, all of which are suspiciosly similar to each other: in the $i$-th complaint, one of the radio fans has mentioned that the signals of two radio stations $x_i$ and $y_i$ are not covering some parts of the city, and demanded that the signal of <span class="tex-font-style-bf">at least one</span> of these stations can be received in the whole city.</p><p>Of cousre, the mayor of Bertown is currently working to satisfy these complaints. A new radio tower has been installed in Bertown, it can transmit a signal with any integer power from $1$ to $M$ (let's denote the signal power as $f$). The mayor has decided that he will choose a set of radio stations and establish a contract with every chosen station. To establish a contract with the $i$-th station, the following conditions should be met:</p><ul> <li> the signal power $f$ should be not less than $l_i$, otherwise the signal of the $i$-th station won't cover the whole city; </li><li> the signal power $f$ should be not greater than $r_i$, otherwise the signal will be received by the residents of other towns which haven't established a contract with the $i$-th station. </li></ul><p>All this information was already enough for the mayor to realise that choosing the stations is hard. But after consulting with specialists, he learned that some stations the signals of some stations may interfere with each other: there are $m$ pairs of stations ($u_i$, $v_i$) that use the same signal frequencies, and for each such pair it is impossible to establish contracts with both stations. <span class="tex-font-style-bf">If stations $x$ and $y$ use the same frequencies, and $y$ and $z$ use the same frequencies, it does not imply that $x$ and $z$ use the same frequencies</span>.</p><p>The mayor finds it really hard to analyze this situation, so he hired you to help him. You have to choose signal power $f$ and a set of stations to establish contracts with such that:</p><ul> <li> all complaints are satisfied (formally, for every $i \in [1, n]$ the city establishes a contract either with station $x_i$, or with station $y_i$); </li><li> no two chosen stations interfere with each other (formally, for every $i \in [1, m]$ the city <span class="tex-font-style-bf">does not</span> establish a contract either with station $u_i$, or with station $v_i$); </li><li> for each chosen station, the conditions on signal power are met (formally, for each chosen station $i$ the condition $l_i \le f \le r_i$ is met). </li></ul></div><div class="input-specification"><p>The first line contains $4$ integers $n$, $p$, $M$ and $m$ ($2 \le n, p, M, m \le 4 \cdot 10^5$) — the number of complaints, the number of radio stations, maximum signal power and the number of interfering pairs, respectively.</p><p>Then $n$ lines follow, which describe the complains. Each line contains two integers $x_i$ and $y_i$ ($1 \le x_i &lt; y_i \le p$) — the indices of the radio stations mentioned in the $i$-th complaint). <span class="tex-font-style-bf">All complaints are distinct</span>.</p><p>Then $p$ lines follow, which describe the radio stations. Each line contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le M$) — the constrains on signal power that should be satisfied if the city establishes a contract with the $i$-th station.</p><p>Then $m$ lines follow, which describe the pairs of interfering radio stations. Each line contains two integers $u_i$ and $v_i$ ($1 \le u_i &lt; v_i \le p$) — the indices of interfering radio stations. <span class="tex-font-style-bf">All these pairs are distinct</span>.</p></div><div class="output-specification"><p>If it is impossible to choose signal power and a set of stations to meet all conditions, print $-1$.</p><p>Otherwise print two integers $k$ and $f$ in the first line — the number of stations in the chosen set and the chosen signal power, respectively. In the second line print $k$ <span class="tex-font-style-bf">distinct</span> integers from $1$ to $p$ — the indices of stations to establish contracts with (in any order). If there are multiple answers, print any of them; you don't have to minimize/maximize the number of chosen stations, and the same applies to signal power.</p></div>

## Input

<p>The first line contains $4$ integers $n$, $p$, $M$ and $m$ ($2 \le n, p, M, m \le 4 \cdot 10^5$) — the number of complaints, the number of radio stations, maximum signal power and the number of interfering pairs, respectively.</p><p>Then $n$ lines follow, which describe the complains. Each line contains two integers $x_i$ and $y_i$ ($1 \le x_i &lt; y_i \le p$) — the indices of the radio stations mentioned in the $i$-th complaint). <span class="tex-font-style-bf">All complaints are distinct</span>.</p><p>Then $p$ lines follow, which describe the radio stations. Each line contains two integers $l_i$ and $r_i$ ($1 \le l_i \le r_i \le M$) — the constrains on signal power that should be satisfied if the city establishes a contract with the $i$-th station.</p><p>Then $m$ lines follow, which describe the pairs of interfering radio stations. Each line contains two integers $u_i$ and $v_i$ ($1 \le u_i &lt; v_i \le p$) — the indices of interfering radio stations. <span class="tex-font-style-bf">All these pairs are distinct</span>.</p>

## Output

<p>If it is impossible to choose signal power and a set of stations to meet all conditions, print $-1$.</p><p>Otherwise print two integers $k$ and $f$ in the first line — the number of stations in the chosen set and the chosen signal power, respectively. In the second line print $k$ <span class="tex-font-style-bf">distinct</span> integers from $1$ to $p$ — the indices of stations to establish contracts with (in any order). If there are multiple answers, print any of them; you don't have to minimize/maximize the number of chosen stations, and the same applies to signal power.</p>





```input1
2 4 4 2
1 3
2 3
1 4
1 2
3 4
1 4
1 2
3 4
```




```input2
2 4 4 2
1 3
2 4
1 2
1 2
3 4
3 4
1 2
3 4
```




```output1
2 3
1 3
```




```output2
-1
```


