## Description

<div><p>Allen wants to enter a fan zone that occupies a round square and has $n$ entrances.</p><p>There already is a queue of $a_i$ people in front of the $i$-th entrance. Each entrance allows one person from its queue to enter the fan zone in one minute.</p><p>Allen uses the following strategy to enter the fan zone: </p><ul> <li> Initially he stands in the end of the queue in front of the first entrance. </li><li> Each minute, if he is not allowed into the fan zone during the minute (meaning he is not the first in the queue), he leaves the current queue and stands in the end of the queue of the next entrance (or the first entrance if he leaves the last entrance). </li></ul><p>Determine the entrance through which Allen will finally enter the fan zone.</p></div><div class="input-specification"><p>The first line contains a single integer $n$ ($2 \le n \le 10^5$)&nbsp;— the number of entrances.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;— the number of people in queues. These numbers do not include Allen.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of entrance that Allen will use.</p></div>

## Input

<p>The first line contains a single integer $n$ ($2 \le n \le 10^5$)&nbsp;— the number of entrances.</p><p>The second line contains $n$ integers $a_1, a_2, \ldots, a_n$ ($0 \le a_i \le 10^9$)&nbsp;— the number of people in queues. These numbers do not include Allen.</p>

## Output

<p>Print a single integer&nbsp;— the number of entrance that Allen will use.</p>





```input1
4
2 3 2 0

```




```input2
2
10 10

```




```input3
6
5 2 6 5 7 4

```




```output1
3

```




```output2
1

```




```output3
6

```



## Note

<p>In the first example the number of people (not including Allen) changes as follows: $[\textbf{2}, 3, 2, 0] \to [1, \textbf{2}, 1, 0] \to [0, 1, \textbf{0}, 0]$. The number in bold is the queue Alles stands in. We see that he will enter the fan zone through the third entrance.</p><p>In the second example the number of people (not including Allen) changes as follows: $[\textbf{10}, 10] \to [9, \textbf{9}] \to [\textbf{8}, 8] \to [7, \textbf{7}] \to [\textbf{6}, 6] \to \\ [5, \textbf{5}] \to [\textbf{4}, 4] \to [3, \textbf{3}] \to [\textbf{2}, 2] \to [1, \textbf{1}] \to [\textbf{0}, 0]$.</p><p>In the third example the number of people (not including Allen) changes as follows: $[\textbf{5}, 2, 6, 5, 7, 4] \to [4, \textbf{1}, 5, 4, 6, 3] \to [3, 0, \textbf{4}, 3, 5, 2] \to \\ [2, 0, 3, \textbf{2}, 4, 1] \to [1, 0, 2, 1, \textbf{3}, 0] \to [0, 0, 1, 0, 2, \textbf{0}]$.</p>
