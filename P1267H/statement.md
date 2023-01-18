## Description

<div><p>Very soon, the new cell phone services provider "BerLine" will begin its work in Berland!</p><p>The start of customer service is planned along the main street of the capital. There are $n$&nbsp;base stations that are already installed. They are located one after another along the main street in the order from the&nbsp;$1$-st to the&nbsp;$n$-th from left to right. </p><p>Currently, all these base stations are turned off. They will be turned on one by one, one base station per day, according to some permutation $p = [p_1, p_2, \dots, p_n]$ ($ 1 \le p_i \le n$), where $p_i$ is the index of a base station that will be turned on on the $i$-th day. Thus, it will take $n$ days to turn on all base stations.</p><p>Each base station is characterized by its operating frequency $f_i$&nbsp;— an integer between $1$ and $24$, inclusive.</p><p>There is an important requirement for operating frequencies of base stations. Consider an arbitrary moment in time. For any phone owner, if we consider all base stations turned on in the access area of their phone, then in this set of base stations there should be at least one whose operating frequency is unique among the frequencies of these stations. Since the power of the phone and the position are not known in advance, this means that for any nonempty subsegment of turned on base stations, at least one of them has to have the operating frequency that is unique among the stations of this subsegment.</p><p>For example, let's take a look at a case of $n = 7$, all $n$ stations are turned on, and their frequencies are equal to $f = [1, 2, 1, 3, 1, 2, 1]$. Consider any subsegment of the base stations&nbsp;— there is a base station with a unique frequency within this subsegment. However, if $f = [1, 2, 1, 2, 3, 2, 1]$, then there is no unique frequency on the segment $[1, 2, 1, 2]$ from the index $1$ to the index $4$, inclusive.</p><p>Your task is to assign a frequency from $1$ to $24$ to each of $n$ base stations in such a way that the frequency requirement is met at every moment. Remember that the base stations are turned on in the order of the given permutation $p$.</p></div><div class="input-specification"><p>The first line of the input contains an integer $t$ ($1 \le t \le 50$)&nbsp;— the number of test cases in the input. Then $t$ test case descriptions follow.</p><p>The first line of a test case contains an integer $n$ ($ 1 \le n \le 8\,500$)&nbsp;— the number of "BerLine" base stations.</p><p>The following line contains $n$ distinct integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$)&nbsp;— the order in which the base stations are turned on, i.&nbsp;e. on the $i$-th day the base station with the index $p_i$ is turned on.</p><p>It is guaranteed that a correct answer exists for all test cases in the input.</p></div><div class="output-specification"><p>Print exactly $t$ lines, where the $j$-th line contains the answer for the $j$-th test case in the input. Print the required frequencies $f_1, f_2, \dots, f_n$ ($1 \le f_i \le 24$). If there are several possible answers, print any of them.</p></div>

## Input

<p>The first line of the input contains an integer $t$ ($1 \le t \le 50$)&nbsp;— the number of test cases in the input. Then $t$ test case descriptions follow.</p><p>The first line of a test case contains an integer $n$ ($ 1 \le n \le 8\,500$)&nbsp;— the number of "BerLine" base stations.</p><p>The following line contains $n$ distinct integers $p_1, p_2, \dots, p_n$ ($1 \le p_i \le n$)&nbsp;— the order in which the base stations are turned on, i.&nbsp;e. on the $i$-th day the base station with the index $p_i$ is turned on.</p><p>It is guaranteed that a correct answer exists for all test cases in the input.</p>

## Output

<p>Print exactly $t$ lines, where the $j$-th line contains the answer for the $j$-th test case in the input. Print the required frequencies $f_1, f_2, \dots, f_n$ ($1 \le f_i \le 24$). If there are several possible answers, print any of them.</p>





```input1
5
3
1 3 2
3
1 2 3
1
1
10
6 10 4 2 7 9 5 8 3 1
10
2 4 6 9 1 8 10 5 3 7
```




```output1
1 3 2 
10 20 10
1 
2 3 4 5 3 1 3 5 4 2 
1 2 3 4 5 6 7 8 9 10
```



## Note

<p>In the first test case $n = 3$ and $p = [1, 3, 2]$. The base stations can be assigned frequencies $[1, 3, 2]$.</p><ul> <li> Day 1: only the base station $1$ is turned on, its frequency is $1$. </li><li> Day 2: the base stations $1$ and $3$ are turned on, their frequencies are $[1, 2]$. </li><li> Day 3: all base stations are turned on, their frequencies are $[1, 3, 2]$ (in the direction along the street). </li></ul><p>On each day, each nonempty subsegment of turned on base stations has a base station with a unique frequency among this subsegment. It can be shown that three distinct frequencies are necessary in this test case.</p>
