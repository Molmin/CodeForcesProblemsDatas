## Description

<div><p>The Central Company has an office with a sophisticated security system. There are $10^6$ employees, numbered from $1$ to $10^6$.</p><p>The security system logs entrances and departures. The entrance of the $i$-th employee is denoted by the integer $i$, while the departure of the $i$-th employee is denoted by the integer $-i$.</p><p>The company has some strict rules about access to its office:</p><ul> <li> An employee can enter the office <span class="tex-font-style-bf">at most</span> once per day. </li><li> He obviously can't leave the office if he didn't enter it earlier that day. </li><li> In the beginning and at the end of every day, the office is empty (employees can't stay at night). <span class="tex-font-style-it">It may also be empty at any moment of the day.</span> </li></ul><p>Any array of events satisfying these conditions is called a <span class="tex-font-style-it">valid day</span>.</p><p>Some examples of valid or invalid days:</p><ul> <li> $[1, 7, -7, 3, -1, -3]$ is a valid day ($1$ enters, $7$ enters, $7$ leaves, $3$ enters, $1$ leaves, $3$ leaves). </li><li> $[2, -2, 3, -3]$ is also a valid day. </li><li> $[2, 5, -5, 5, -5, -2]$ is <span class="tex-font-style-underline">not</span> a valid day, because $5$ entered the office twice during the same day. </li><li> $[-4, 4]$ is <span class="tex-font-style-underline">not</span> a valid day, because $4$ left the office without being in it. </li><li> $[4]$ is <span class="tex-font-style-underline">not</span> a valid day, because $4$ entered the office and didn't leave it before the end of the day. </li></ul><p>There are $n$ events $a_1, a_2, \ldots, a_n$, in the order they occurred. This array corresponds to one or more consecutive days. The system administrator erased the dates of events by mistake, but he didn't change the order of the events.</p><p>You must partition (to cut) the array $a$ of events into <span class="tex-font-style-bf">contiguous subarrays</span>, which must represent non-empty valid days (or say that it's impossible). Each array element should belong to exactly one contiguous subarray of a partition. Each contiguous subarray of a partition should be a <span class="tex-font-style-it">valid day</span>.</p><p>For example, if $n=8$ and $a=[1, -1, 1, 2, -1, -2, 3, -3]$ then he can partition it into two contiguous subarrays which are valid days: $a = [1, -1~ \boldsymbol{|}~ 1, 2, -1, -2, 3, -3]$.</p><p>Help the administrator to partition the given array $a$ in the required way or report that it is impossible to do. Find any required partition, you should not minimize or maximize the number of parts.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^6 \le a_i \le 10^6$ and $a_i \neq 0$).</p></div><div class="output-specification"><p>If there is no valid partition, print $-1$. Otherwise, print any valid partition in the following format:</p><ul> <li> On the first line print the number $d$ of days ($1 \le d \le n$). </li><li> On the second line, print $d$ integers $c_1, c_2, \ldots, c_d$ ($1 \le c_i \le n$ and $c_1 + c_2 + \ldots + c_d = n$), where $c_i$ is the number of events in the $i$-th day. </li></ul><p>If there are many valid solutions, you can print <span class="tex-font-style-bf">any</span> of them. You don't have to minimize nor maximize the number of days.</p></div>

## Input

<p>The first line contains a single integer $n$ ($1 \le n \le 10^5$).</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($-10^6 \le a_i \le 10^6$ and $a_i \neq 0$).</p>

## Output

<p>If there is no valid partition, print $-1$. Otherwise, print any valid partition in the following format:</p><ul> <li> On the first line print the number $d$ of days ($1 \le d \le n$). </li><li> On the second line, print $d$ integers $c_1, c_2, \ldots, c_d$ ($1 \le c_i \le n$ and $c_1 + c_2 + \ldots + c_d = n$), where $c_i$ is the number of events in the $i$-th day. </li></ul><p>If there are many valid solutions, you can print <span class="tex-font-style-bf">any</span> of them. You don't have to minimize nor maximize the number of days.</p>





```input1
6
1 7 -7 3 -1 -3
```




```input2
8
1 -1 1 2 -1 -2 3 -3
```




```input3
6
2 5 -5 5 -5 -2
```




```input4
3
-8 1 1
```




```output1
1
6
```




```output2
2
2 6
```




```output3
-1
```




```output4
-1
```



## Note

<p>In the first example, the whole array is a valid day.</p><p>In the second example, one possible valid solution is to split the array into $[1, -1]$ and $[1, 2, -1, -2, 3, -3]$ ($d = 2$ and $c = [2, 6]$). The only other valid solution would be to split the array into $[1, -1]$, $[1, 2, -1, -2]$ and $[3, -3]$ ($d = 3$ and $c = [2, 4, 2]$). <span class="tex-font-style-underline">Both solutions are accepted.</span></p><p>In the third and fourth examples, we can prove that there exists no valid solution. Please note that the array given in input is <span class="tex-font-style-bf">not</span> guaranteed to represent a coherent set of events.</p>
