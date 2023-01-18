## Description

<div><p>After learning a lot about space exploration, a little girl named Ana wants to change the subject.</p><p>Ana is a girl who loves palindromes (string that can be read the same backwards as forward). She has learned how to check for a given string whether it's a palindrome or not, but soon she grew tired of this problem, so she came up with a more interesting one and she needs your help to solve it:</p><p>You are given an array of strings which consist of only small letters of the alphabet. Your task is to find <span class="tex-font-style-bf">how many</span> palindrome pairs are there in the array. A palindrome pair is a pair of strings such that the following condition holds: <span class="tex-font-style-bf">at least one</span> permutation of the concatenation of the two strings is a palindrome. In other words, if you have two strings, let's say "<span class="tex-font-style-tt">aab</span>" and "<span class="tex-font-style-tt">abcac</span>", and you concatenate them into "<span class="tex-font-style-tt">aababcac</span>", we have to check if there exists a permutation of this new string such that it is a palindrome (in this case there exists the permutation "<span class="tex-font-style-tt">aabccbaa</span>"). </p><p>Two pairs are considered different if the strings are located on <span class="tex-font-style-bf">different indices</span>. The pair of strings with indices $(i,j)$ is considered <span class="tex-font-style-bf">the same</span> as the pair $(j,i)$.</p></div><div class="input-specification"><p>The first line contains a positive integer $N$ ($1 \le N \le 100\,000$), representing the length of the input array.</p><p>Eacg of the next $N$ lines contains a string (consisting of lowercase English letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">z</span>')&nbsp;— an element of the input array. </p><p>The total number of characters in the input array will be less than $1\,000\,000$.</p></div><div class="output-specification"><p>Output one number, representing <span class="tex-font-style-bf">how many palindrome pairs</span> there are in the array.</p></div>

## Input

<p>The first line contains a positive integer $N$ ($1 \le N \le 100\,000$), representing the length of the input array.</p><p>Eacg of the next $N$ lines contains a string (consisting of lowercase English letters from '<span class="tex-font-style-tt">a</span>' to '<span class="tex-font-style-tt">z</span>')&nbsp;— an element of the input array. </p><p>The total number of characters in the input array will be less than $1\,000\,000$.</p>

## Output

<p>Output one number, representing <span class="tex-font-style-bf">how many palindrome pairs</span> there are in the array.</p>





```input1
3
aa
bb
cd

```




```input2
6
aab
abcac
dffe
ed
aa
aade

```




```output1
1

```




```output2
6

```



## Note

<p>The first example:</p><ol> <li> <span class="tex-font-style-tt">aa</span> $+$ <span class="tex-font-style-tt">bb</span> $\to$ <span class="tex-font-style-tt">abba</span>. </li></ol><p>The second example:</p><ol> <li> <span class="tex-font-style-tt">aab</span> $+$ <span class="tex-font-style-tt">abcac</span> $=$ <span class="tex-font-style-tt">aababcac</span> $\to$ <span class="tex-font-style-tt">aabccbaa</span></li><li> <span class="tex-font-style-tt">aab</span> $+$ <span class="tex-font-style-tt">aa</span> $=$ <span class="tex-font-style-tt">aabaa</span></li><li> <span class="tex-font-style-tt">abcac</span> $+$ <span class="tex-font-style-tt">aa</span> $=$ <span class="tex-font-style-tt">abcacaa</span> $\to$ <span class="tex-font-style-tt">aacbcaa</span></li><li> <span class="tex-font-style-tt">dffe</span> $+$ <span class="tex-font-style-tt">ed</span> $=$ <span class="tex-font-style-tt">dffeed</span> $\to$ <span class="tex-font-style-tt">fdeedf</span></li><li> <span class="tex-font-style-tt">dffe</span> $+$ <span class="tex-font-style-tt">aade</span> $=$ <span class="tex-font-style-tt">dffeaade</span> $\to$ <span class="tex-font-style-tt">adfaafde</span></li><li> <span class="tex-font-style-tt">ed</span> $+$ <span class="tex-font-style-tt">aade</span> $=$ <span class="tex-font-style-tt">edaade</span> $\to$ <span class="tex-font-style-tt">aeddea</span> </li></ol>
