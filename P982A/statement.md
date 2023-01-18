## Description

<div><p>You're given a row with $n$ chairs. We call a seating of people "maximal" if the two following conditions hold:</p><ol> <li> There are no neighbors adjacent to anyone seated. </li><li> It's impossible to seat one more person without violating the first rule. </li></ol><p>The seating is given as a string consisting of zeros and ones ($0$ means that the corresponding seat is empty, $1$ — occupied). The goal is to determine whether this seating is "maximal".</p><p>Note that the first and last seats are <span class="tex-font-style-bf">not</span> adjacent (if $n \ne 2$).</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \leq n \leq 1000$)&nbsp;— the number of chairs.</p><p>The next line contains a string of $n$ characters, each of them is either zero or one, describing the seating.</p></div><div class="output-specification"><p>Output "<span class="tex-font-style-tt">Yes</span>" (without quotation marks) if the seating is "maximal". Otherwise print "<span class="tex-font-style-tt">No</span>".</p><p>You are allowed to print letters in whatever case you'd like (uppercase or lowercase).</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \leq n \leq 1000$)&nbsp;— the number of chairs.</p><p>The next line contains a string of $n$ characters, each of them is either zero or one, describing the seating.</p>

## Output

<p>Output "<span class="tex-font-style-tt">Yes</span>" (without quotation marks) if the seating is "maximal". Otherwise print "<span class="tex-font-style-tt">No</span>".</p><p>You are allowed to print letters in whatever case you'd like (uppercase or lowercase).</p>





```input1
3
101

```




```input2
4
1011

```




```input3
5
10001

```




```output1
Yes

```




```output2
No

```




```output3
No

```



## Note

<p>In sample case one the given seating is maximal.</p><p>In sample case two the person at chair three has a neighbour to the right.</p><p>In sample case three it is possible to seat yet another person into chair three.</p>
