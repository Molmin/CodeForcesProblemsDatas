## Description

<div><p>Polycarp is working on a new operating system called BerOS. He asks you to help with implementation of a file suggestion feature.</p><p>There are $n$ files on hard drive and their names are $f_1, f_2, \dots, f_n$. Any file name contains between $1$ and $8$ characters, inclusive. All file names are unique.</p><p>The file suggestion feature handles queries, each represented by a string $s$. For each query $s$ it should count number of files containing $s$ as a substring (i.e. some continuous segment of characters in a file name equals $s$) and suggest any such file name.</p><p>For example, if file names are "<span class="tex-font-style-tt">read.me</span>", "<span class="tex-font-style-tt">hosts</span>", "<span class="tex-font-style-tt">ops</span>", and "<span class="tex-font-style-tt">beros.18</span>", and the query is "<span class="tex-font-style-tt">os</span>", the number of matched files is $2$ (two file names contain "<span class="tex-font-style-tt">os</span>" as a substring) and suggested file name can be either "<span class="tex-font-style-tt">hosts</span>" or "<span class="tex-font-style-tt">beros.18</span>".</p></div><div class="input-specification"><p>The first line of the input contains integer $n$ ($1 \le n \le 10000$) — the total number of files.</p><p>The following $n$ lines contain file names, one per line. The $i$-th line contains $f_i$ — the name of the $i$-th file. Each file name contains between $1$ and $8$ characters, inclusive. File names contain only lowercase Latin letters, digits and dot characters ('<span class="tex-font-style-tt">.</span>'). Any sequence of valid characters can be a file name (for example, in BerOS "<span class="tex-font-style-tt">.</span>", "<span class="tex-font-style-tt">..</span>" and "<span class="tex-font-style-tt">...</span>" are valid file names). All file names are unique.</p><p>The following line contains integer $q$ ($1 \le q \le 50000$) — the total number of queries.</p><p>The following $q$ lines contain queries $s_1, s_2, \dots, s_q$, one per line. Each $s_j$ has length between $1$ and $8$ characters, inclusive. It contains only lowercase Latin letters, digits and dot characters ('<span class="tex-font-style-tt">.</span>').</p></div><div class="output-specification"><p>Print $q$ lines, one per query. The $j$-th line should contain the response on the $j$-th query — two values $c_j$ and $t_j$, where</p><ul> <li> $c_j$ is the number of matched files for the $j$-th query, </li><li> $t_j$ is the name of any file matched by the $j$-th query. If there is no such file, print a single character '<span class="tex-font-style-tt">-</span>' instead. If there are multiple matched files, print any. </li></ul></div>

## Input

<p>The first line of the input contains integer $n$ ($1 \le n \le 10000$) — the total number of files.</p><p>The following $n$ lines contain file names, one per line. The $i$-th line contains $f_i$ — the name of the $i$-th file. Each file name contains between $1$ and $8$ characters, inclusive. File names contain only lowercase Latin letters, digits and dot characters ('<span class="tex-font-style-tt">.</span>'). Any sequence of valid characters can be a file name (for example, in BerOS "<span class="tex-font-style-tt">.</span>", "<span class="tex-font-style-tt">..</span>" and "<span class="tex-font-style-tt">...</span>" are valid file names). All file names are unique.</p><p>The following line contains integer $q$ ($1 \le q \le 50000$) — the total number of queries.</p><p>The following $q$ lines contain queries $s_1, s_2, \dots, s_q$, one per line. Each $s_j$ has length between $1$ and $8$ characters, inclusive. It contains only lowercase Latin letters, digits and dot characters ('<span class="tex-font-style-tt">.</span>').</p>

## Output

<p>Print $q$ lines, one per query. The $j$-th line should contain the response on the $j$-th query — two values $c_j$ and $t_j$, where</p><ul> <li> $c_j$ is the number of matched files for the $j$-th query, </li><li> $t_j$ is the name of any file matched by the $j$-th query. If there is no such file, print a single character '<span class="tex-font-style-tt">-</span>' instead. If there are multiple matched files, print any. </li></ul>





```input1
4
test
contests
test.
.test
6
ts
.
st.
.test
contes.
st

```




```output1
1 contests
2 .test
1 test.
1 .test
0 -
4 test.

```


