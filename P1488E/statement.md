## Description

<div><p>A subsequence is a sequence that can be obtained from another sequence by removing some elements without changing the order of the remaining elements.</p><p>A palindromic sequence is a sequence that is equal to the reverse of itself.</p><p>You are given a sequence of $n$ integers $a_1, a_2, \dots, a_n$. <span class="tex-font-style-bf">Any integer value appears in $a$ no more than twice</span>.</p><p>What is the length of the longest palindromic subsequence of sequence $a$?</p></div><div class="input-specification"><p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 250\,000$)&nbsp;— the number of elements in the sequence.</p><p>The second line of each testcase contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$).</p><p>Any integer value appears in $a$ no more than twice. The sum of $n$ over all testcases doesn't exceed $250\,000$.</p></div><div class="output-specification"><p>For each testcase print a single integer&nbsp;— the length of the longest palindromic subsequence of sequence $a$.</p></div>

## Input

<p>The first line contains a single integer $t$ ($1 \le t \le 1000$)&nbsp;— the number of testcases.</p><p>Then the descriptions of $t$ testcases follow.</p><p>The first line of each testcase contains a single integer $n$ ($1 \le n \le 250\,000$)&nbsp;— the number of elements in the sequence.</p><p>The second line of each testcase contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le n$).</p><p>Any integer value appears in $a$ no more than twice. The sum of $n$ over all testcases doesn't exceed $250\,000$.</p>

## Output

<p>For each testcase print a single integer&nbsp;— the length of the longest palindromic subsequence of sequence $a$.</p>





```input1
5
6
2 1 3 1 5 2
6
1 3 3 4 4 1
1
1
2
1 1
7
4 4 2 5 7 2 3
```




```output1
5
4
1
2
3
```



## Note

<p>Here are the longest palindromic subsequences for the example testcases: </p><ul> <li> <span class="tex-font-style-underline"><span class="tex-font-style-bf">2</span></span> <span class="tex-font-style-underline"><span class="tex-font-style-bf">1</span></span> <span class="tex-font-style-underline"><span class="tex-font-style-bf">3</span></span> <span class="tex-font-style-underline"><span class="tex-font-style-bf">1</span></span> 5 <span class="tex-font-style-underline"><span class="tex-font-style-bf">2</span></span> </li><li> <span class="tex-font-style-underline"><span class="tex-font-style-bf">1</span></span> <span class="tex-font-style-underline"><span class="tex-font-style-bf">3</span></span> <span class="tex-font-style-underline"><span class="tex-font-style-bf">3</span></span> 4 4 <span class="tex-font-style-underline"><span class="tex-font-style-bf">1</span></span> or <span class="tex-font-style-underline"><span class="tex-font-style-bf">1</span></span> 3 3 <span class="tex-font-style-underline"><span class="tex-font-style-bf">4</span></span> <span class="tex-font-style-underline"><span class="tex-font-style-bf">4</span></span> <span class="tex-font-style-underline"><span class="tex-font-style-bf">1</span></span> </li><li> <span class="tex-font-style-underline"><span class="tex-font-style-bf">1</span></span> </li><li> <span class="tex-font-style-underline"><span class="tex-font-style-bf">1</span></span> <span class="tex-font-style-underline"><span class="tex-font-style-bf">1</span></span> </li><li> 4 4 <span class="tex-font-style-underline"><span class="tex-font-style-bf">2</span></span> <span class="tex-font-style-underline"><span class="tex-font-style-bf">5</span></span> 7 <span class="tex-font-style-underline"><span class="tex-font-style-bf">2</span></span> 3 or 4 4 <span class="tex-font-style-underline"><span class="tex-font-style-bf">2</span></span> 5 <span class="tex-font-style-underline"><span class="tex-font-style-bf">7</span></span> <span class="tex-font-style-underline"><span class="tex-font-style-bf">2</span></span> 3 </li></ul>
