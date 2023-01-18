## Description

<div><p>Vladik is a competitive programmer. This year he is going to win the International Olympiad in Informatics. But it is not as easy as it sounds: the question Vladik face now is to find the cheapest way to get to the olympiad.</p><p>Vladik knows <span class="tex-span"><i>n</i></span> airports. All the airports are located on a straight line. Each airport has unique id from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>, Vladik's house is situated next to the airport with id <span class="tex-span"><i>a</i></span>, and the place of the olympiad is situated next to the airport with id <span class="tex-span"><i>b</i></span>. It is possible that Vladik's house and the place of the olympiad are located near the same airport. </p><p>To get to the olympiad, Vladik can fly between any pair of airports any number of times, but he has to start his route at the airport <span class="tex-span"><i>a</i></span> and finish it at the airport <span class="tex-span"><i>b</i></span>.</p><p>Each airport belongs to one of two companies. The cost of flight from the airport <span class="tex-span"><i>i</i></span> to the airport <span class="tex-span"><i>j</i></span> is zero if both airports belong to the same company, and <span class="tex-span">|<i>i</i> - <i>j</i>|</span> if they belong to different companies.</p><p>Print the minimum cost Vladik has to pay to get to the olympiad.</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>)&nbsp;— the number of airports, the id of the airport from which Vladik starts his route and the id of the airport which he has to reach. </p><p>The second line contains a string with length <span class="tex-span"><i>n</i></span>, which consists only of characters <span class="tex-span">0</span> and <span class="tex-span">1</span>. If the <span class="tex-span"><i>i</i></span>-th character in this string is <span class="tex-span">0</span>, then <span class="tex-span"><i>i</i></span>-th airport belongs to first company, otherwise it belongs to the second.</p></div><div class="output-specification"><p>Print single integer&nbsp;— the minimum cost Vladik has to pay to get to the olympiad.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>a</i></span>, and <span class="tex-span"><i>b</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>a</i>, <i>b</i> ≤ <i>n</i></span>)&nbsp;— the number of airports, the id of the airport from which Vladik starts his route and the id of the airport which he has to reach. </p><p>The second line contains a string with length <span class="tex-span"><i>n</i></span>, which consists only of characters <span class="tex-span">0</span> and <span class="tex-span">1</span>. If the <span class="tex-span"><i>i</i></span>-th character in this string is <span class="tex-span">0</span>, then <span class="tex-span"><i>i</i></span>-th airport belongs to first company, otherwise it belongs to the second.</p>

## Output

<p>Print single integer&nbsp;— the minimum cost Vladik has to pay to get to the olympiad.</p>





```input1
4 1 4
1010

```




```input2
5 5 2
10110

```




```output1
1
```




```output2
0
```



## Note

<p>In the first example Vladik can fly to the airport <span class="tex-span">2</span> at first and pay <span class="tex-span">|1 - 2| = 1</span> (because the airports belong to different companies), and then fly from the airport <span class="tex-span">2</span> to the airport <span class="tex-span">4</span> for free (because the airports belong to the same company). So the cost of the whole flight is equal to <span class="tex-span">1</span>. It's impossible to get to the olympiad for free, so the answer is equal to <span class="tex-span">1</span>. </p><p>In the second example Vladik can fly directly from the airport <span class="tex-span">5</span> to the airport <span class="tex-span">2</span>, because they belong to the same company.</p>
