## Description

<div><p><span class="tex-font-style-it">This is the hard version of the problem. The only difference between the easy and the hard versions are removal queries, they are present only in the hard version.</span></p><p>"Interplanetary Software, Inc." together with "Robots of Cydonia, Ltd." has developed and released robot cats. These electronic pets can meow, catch mice and entertain the owner in various ways.</p><p>The developers from "Interplanetary Software, Inc." have recently decided to release a software update for these robots. After the update, the cats must solve the problems about bracket sequences. One of the problems is described below.</p><center> <img class="tex-graphics" src="file://b6YedsWw.png" style="max-width: 100.0%;max-height: 100.0%;" width="284px"> </center><p>First, we need to learn a bit of bracket sequence theory. Consider the strings that contain characters "<span class="tex-font-style-tt">(</span>", "<span class="tex-font-style-tt">)</span>" and "<span class="tex-font-style-tt">.</span>". Call a string <span class="tex-font-style-it">regular bracket sequence (RBS)</span>, if it can be transformed to an empty string by one or more operations of removing either single "<span class="tex-font-style-tt">.</span>" characters, or a continuous substring "<span class="tex-font-style-tt">()</span>". For instance, the string "<span class="tex-font-style-tt">(()(.))</span>" is an RBS, as it can be transformed to an empty string with the following sequence of removals:</p><center> "<span class="tex-font-style-tt">(()(<span class="tex-font-style-underline">.</span>))</span>" $\rightarrow$ "<span class="tex-font-style-tt">(()<span class="tex-font-style-underline">()</span>)</span>" $\rightarrow$ "<span class="tex-font-style-tt">(<span class="tex-font-style-underline">()</span>)</span>" $\rightarrow$ "<span class="tex-font-style-tt"><span class="tex-font-style-underline">()</span></span>" $\rightarrow$ "". </center><p>We got an empty string, so the initial string was an RBS. At the same time, the string "<span class="tex-font-style-tt">)(</span>" is not an RBS, as it is not possible to apply such removal operations to it.</p><p>An RBS is <span class="tex-font-style-it">simple</span> if this RBS is not empty, doesn't start with "<span class="tex-font-style-tt">.</span>", and doesn't end with "<span class="tex-font-style-tt">.</span>".</p><p>Denote the <span class="tex-font-style-it">substring</span> of the string $s$ as its sequential subsegment. In particular, $s[l\dots r] = s_ls_{l+1}\dots s_r$, where $s_i$ is the $i$-th character of the string $s$.</p><p>Now, move on to the problem statement itself. You are given a string $s$, initially consisting of characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>". You need to answer the following queries:</p><ol> <li> Given two indices, $l$ and $r$ ($1 \le l &lt; r \le n$). It's <span class="tex-font-style-bf">guaranteed</span> that the $l$-th character is equal to "<span class="tex-font-style-tt">(</span>", the $r$-th character is equal to "<span class="tex-font-style-tt">)</span>", and the characters between them are equal to "<span class="tex-font-style-tt">.</span>". Then the $l$-th and the $r$-th characters must be set to "<span class="tex-font-style-tt">.</span>". </li><li> Given two indices, $l$ and $r$ ($1 \le l &lt; r \le n$), and it's <span class="tex-font-style-bf">guaranteed</span> that the substring $s[l\dots r]$ is a <span class="tex-font-style-bf">simple RBS</span>. You need to find the number of substrings in $s[l\dots r]$ such that they are simple RBS. In other words, find the number of index pairs $i$, $j$ such that $l \le i &lt; j \le r$ and $s[i\dots j]$ is a simple RBS. </li></ol><p>You are an employee in "Interplanetary Software, Inc." and you were given the task to teach the cats to solve the problem above, after the update.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $q$ ($2 \le n \le 3\cdot10^5$, $1 \le q \le 3\cdot10^5$), the length of the string, and the number of queries.</p><p>The second line contains the string $s$, consisting of $n$ characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>".</p><p>Each of the following $q$ lines contains three integers $t$, $l$ and $r$ ($t \in \{1, 2\}$, $1 \le l &lt; r \le n$), the queries you need to answer. It is guaranteed that all the queries are valid and correspond to the problem statements.</p></div><div class="output-specification"><p>For each query, print a single integer in a separate line, the number of substrings that are simple RBS. The answers must be printed in the same order as the queries are specified in the input.</p></div>

## Input

<p>The first line contains two integers $n$ and $q$ ($2 \le n \le 3\cdot10^5$, $1 \le q \le 3\cdot10^5$), the length of the string, and the number of queries.</p><p>The second line contains the string $s$, consisting of $n$ characters "<span class="tex-font-style-tt">(</span>" and "<span class="tex-font-style-tt">)</span>".</p><p>Each of the following $q$ lines contains three integers $t$, $l$ and $r$ ($t \in \{1, 2\}$, $1 \le l &lt; r \le n$), the queries you need to answer. It is guaranteed that all the queries are valid and correspond to the problem statements.</p>

## Output

<p>For each query, print a single integer in a separate line, the number of substrings that are simple RBS. The answers must be printed in the same order as the queries are specified in the input.</p>





```input1
9 8
)(()())()
2 3 6
2 2 7
1 3 4
2 2 7
2 2 9
1 5 6
1 2 7
2 8 9
```




```output1
3
4
2
4
1
```



## Note

<p>Consider the example test case.</p><p>The answer to the first query is $3$, as there are three suitable substrings: $s[3\dots6]$, $s[3\dots4]$ and $s[5\dots6]$.</p><p>The answer to the second query is $4$. The substrings are $s[3\dots6]$, $s[3\dots4]$, $s[5\dots6]$ and $s[2\dots7]$.</p><p>After the third query, the string becomes "<span class="tex-font-style-tt">)(..())()</span>".</p><p>The answer to the fourth query is $2$. The substrings are $s[5\dots6]$ and $s[2\dots7]$. Note that $s[3\dots6]$ is not a simple RBS anymore, as it starts with "<span class="tex-font-style-tt">.</span>".</p><p>The answer to the fifth query is $4$. The substrings are $s[5\dots6]$, $s[2\dots7]$, $s[8\dots9]$ and $s[2\dots9]$.</p><p>After the sixth query, the string becomes "<span class="tex-font-style-tt">)(....)()</span>".</p><p>After the seventh query, the string becomes "<span class="tex-font-style-tt">)......()</span>".</p><p>The answer to the eighth query is $1$. The substring is $s[8\dots9]$.</p>
