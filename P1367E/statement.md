## Description

<div><p>The store sells $n$ beads. The color of each bead is described by a lowercase letter of the English alphabet ("<span class="tex-font-style-tt">a</span>"–"<span class="tex-font-style-tt">z</span>"). You want to buy some beads to assemble a necklace from them.</p><p>A necklace is a set of beads connected in a circle.</p><p>For example, if the store sells beads "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">b</span>", "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">c</span>", "<span class="tex-font-style-tt">c</span>", then you can assemble the following necklaces (these are not all possible options):</p><center> <img class="tex-graphics" src="file://OFFaCVnI.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>And the following necklaces cannot be assembled from beads sold in the store:</p><center> <img class="tex-graphics" src="file://l3TYuArD.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-font-size-small">The first necklace cannot be assembled because it has three beads "<span class="tex-font-style-tt">a</span>" (of the two available). The second necklace cannot be assembled because it contains a bead "<span class="tex-font-style-tt">d</span>", which is not sold in the store.</span> </center><p>We call a necklace $k$-beautiful if, when it is turned clockwise by $k$ beads, the necklace remains unchanged. For example, here is a sequence of three turns of a necklace. </p><center> <img class="tex-graphics" src="file://8PP4cmQO.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> As you can see, this necklace is, for example, $3$-beautiful, $6$-beautiful, $9$-beautiful, and so on, but it is not $1$-beautiful or $2$-beautiful.<p>In particular, a necklace of length $1$ is $k$-beautiful for any integer $k$. A necklace that consists of beads of the same color is also beautiful for any $k$.</p><p>You are given the integers $n$ and $k$, and also the string $s$ containing $n$ lowercase letters of the English alphabet&nbsp;— each letter defines a bead in the store. You can buy any subset of beads and connect them in any order. Find the maximum length of a $k$-beautiful necklace you can assemble.</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases in the test. Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n, k \le 2000$).</p><p>The second line of each test case contains the string $s$ containing $n$ lowercase English letters&nbsp;— the beads in the store.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2000$.</p></div><div class="output-specification"><p>Output $t$ answers to the test cases. Each answer is a positive integer&nbsp;— the maximum length of the $k$-beautiful necklace you can assemble.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 100$)&nbsp;— the number of test cases in the test. Then $t$ test cases follow.</p><p>The first line of each test case contains two integers $n$ and $k$ ($1 \le n, k \le 2000$).</p><p>The second line of each test case contains the string $s$ containing $n$ lowercase English letters&nbsp;— the beads in the store.</p><p>It is guaranteed that the sum of $n$ for all test cases does not exceed $2000$.</p>

## Output

<p>Output $t$ answers to the test cases. Each answer is a positive integer&nbsp;— the maximum length of the $k$-beautiful necklace you can assemble.</p>





```input1
6
6 3
abcbac
3 6
aaa
7 1000
abczgyo
5 4
ababa
20 10
aaebdbabdbbddaadaadc
20 5
ecbedececacbcbccbdec
```




```output1
6
3
5
4
15
10
```



## Note

<p>The first test case is explained in the statement.</p><p>In the second test case, a $6$-beautiful necklace can be assembled from all the letters.</p><p>In the third test case, a $1000$-beautiful necklace can be assembled, for example, from beads "<span class="tex-font-style-tt">abzyo</span>".</p>
