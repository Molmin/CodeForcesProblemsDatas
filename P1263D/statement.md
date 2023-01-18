## Description

<div><p>One unknown hacker wants to get the admin's password of AtForces testing system, to get problems from the next contest. To achieve that, he sneaked into the administrator's office and stole a piece of paper with a list of $n$ passwords — strings, consists of small Latin letters.</p><p>Hacker went home and started preparing to hack AtForces. He found that the system contains only passwords from the stolen list and that the system determines the equivalence of the passwords $a$ and $b$ as follows:</p><ul> <li> two passwords $a$ and $b$ are equivalent if there is a letter, that exists in both $a$ and $b$; </li><li> two passwords $a$ and $b$ are equivalent if there is a password $c$ from the list, which is equivalent to both $a$ and $b$. </li></ul><p>If a password is set in the system and an equivalent one is applied to access the system, then the user is accessed into the system.</p><p>For example, if the list contain passwords "a", "b", "ab", "d", then passwords "a", "b", "ab" are equivalent to each other, but the password "d" is not equivalent to any other password from list. In other words, if:</p><ul> <li> admin's password is "b", then you can access to system by using any of this passwords: "a", "b", "ab"; </li><li> admin's password is "d", then you can access to system by using only "d". </li></ul><p><span class="tex-font-style-bf">Only one</span> password from the list is the admin's password from the testing system. Help hacker to calculate the minimal number of passwords, required to <span class="tex-font-style-bf">guaranteed</span> access to the system. Keep in mind that the hacker does not know which password is set in the system.</p></div><div class="input-specification"><p>The first line contain integer $n$ ($1 \le n \le 2 \cdot 10^5$) — number of passwords in the list. Next $n$ lines contains passwords from the list – non-empty strings $s_i$, with length at most $50$ letters. Some of the passwords may be equal.</p><p>It is guaranteed that the total length of all passwords does not exceed $10^6$ letters. All of them consist only of lowercase Latin letters.</p></div><div class="output-specification"><p>In a single line print the minimal number of passwords, the use of which will allow <span class="tex-font-style-bf">guaranteed</span> to access the system.</p></div>

## Input

<p>The first line contain integer $n$ ($1 \le n \le 2 \cdot 10^5$) — number of passwords in the list. Next $n$ lines contains passwords from the list – non-empty strings $s_i$, with length at most $50$ letters. Some of the passwords may be equal.</p><p>It is guaranteed that the total length of all passwords does not exceed $10^6$ letters. All of them consist only of lowercase Latin letters.</p>

## Output

<p>In a single line print the minimal number of passwords, the use of which will allow <span class="tex-font-style-bf">guaranteed</span> to access the system.</p>





```input1
4
a
b
ab
d
```




```input2
3
ab
bc
abc
```




```input3
1
codeforces
```




```output1
2
```




```output2
1
```




```output3
1
```



## Note

<p>In the second example hacker need to use any of the passwords to access the system.</p>
