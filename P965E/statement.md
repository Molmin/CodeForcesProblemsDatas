## Description

<div><p>Arkady's code contains $n$ variables. Each variable has a unique name consisting of lowercase English letters only. One day Arkady decided to shorten his code.</p><p>He wants to replace each variable name with its non-empty prefix so that these new names are still unique (however, a new name of some variable can coincide with some old name of another or same variable). Among such possibilities he wants to find the way with the smallest possible total length of the new names.</p><p>A string $a$ is a prefix of a string $b$ if you can delete some (possibly none) characters from the end of $b$ and obtain $a$.</p><p>Please find this minimum possible total length of new names.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of variables.</p><p>The next $n$ lines contain variable names, one per line. Each name is non-empty and contains only lowercase English letters. The total length of these strings is not greater than $10^5$. The variable names are distinct.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum possible total length of new variable names.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$)&nbsp;— the number of variables.</p><p>The next $n$ lines contain variable names, one per line. Each name is non-empty and contains only lowercase English letters. The total length of these strings is not greater than $10^5$. The variable names are distinct.</p>

## Output

<p>Print a single integer&nbsp;— the minimum possible total length of new variable names.</p>





```input1
3
codeforces
codehorses
code

```




```input2
5
abba
abb
ab
aa
aacada

```




```input3
3
telegram
digital
resistance

```




```output1
6

```




```output2
11

```




```output3
3

```



## Note

<p>In the first example one of the best options is to shorten the names in the given order as "<span class="tex-font-style-tt">cod</span>", "<span class="tex-font-style-tt">co</span>", "<span class="tex-font-style-tt">c</span>".</p><p>In the second example we can shorten the last name to "<span class="tex-font-style-tt">aac</span>" and the first name to "<span class="tex-font-style-tt">a</span>" without changing the other names.</p>
