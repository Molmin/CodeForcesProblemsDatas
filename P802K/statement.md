## Description

<div><p>Thank you for helping Heidi! It is now the second of April, but she has been summoned by Jenny again. The pranks do not seem to end...</p><p>In the meantime, Heidi has decided that she does not trust her friends anymore. Not too much, anyway. Her relative lack of trust is manifested as follows: whereas previously she would not be made to visit the same person twice, now she can only be sure that she will not be made to visit the same person more than <span class="tex-span"><i>k</i></span> times. (In the case of Jenny, this includes her first visit in the beginning. The situation from the easy version corresponds to setting <span class="tex-span"><i>k</i> = 1</span>.)</p><p>This is not as bad as it looks, since a single ticket for a route between two friends allows Heidi to travel between this pair of friends the whole day (in both directions). In other words, once she pays for travel between a pair of friends, all further travels between that pair are free.</p><p>How much money will Heidi waste now, in a worst-case scenario?</p></div><div class="input-specification"><p>The first line contains two space-separated integers – the number of friends <span class="tex-span"><i>n</i></span> (<img align="middle" class="tex-formula" src="file://PEOtoi9q.png" style="max-width: 100.0%;max-height: 100.0%;">) and the parameter <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>). The next <span class="tex-span"><i>n</i> - 1</span> lines each contain three space-separated integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">4</sup></span>) meaning that <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are friends and the cost for traveling between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> is <span class="tex-span"><i>c</i></span>.</p><p>It is again guaranteed that the social network of the input forms a tree.</p></div><div class="output-specification"><p>Again, output a single integer – the maximum sum of costs of tickets.</p></div>

## Input

<p>The first line contains two space-separated integers – the number of friends <span class="tex-span"><i>n</i></span> (<img align="middle" class="tex-formula" src="file://PEOtoi9q.png" style="max-width: 100.0%;max-height: 100.0%;">) and the parameter <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ 10<sup class="upper-index">5</sup></span>). The next <span class="tex-span"><i>n</i> - 1</span> lines each contain three space-separated integers <span class="tex-span"><i>u</i></span>, <span class="tex-span"><i>v</i></span> and <span class="tex-span"><i>c</i></span> (<span class="tex-span">0 ≤ <i>u</i>, <i>v</i> ≤ <i>n</i> - 1</span>, <span class="tex-span">1 ≤ <i>c</i> ≤ 10<sup class="upper-index">4</sup></span>) meaning that <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> are friends and the cost for traveling between <span class="tex-span"><i>u</i></span> and <span class="tex-span"><i>v</i></span> is <span class="tex-span"><i>c</i></span>.</p><p>It is again guaranteed that the social network of the input forms a tree.</p>

## Output

<p>Again, output a single integer – the maximum sum of costs of tickets.</p>





```input1
9 3
0 1 1
0 2 1
1 3 2
1 4 2
1 5 2
2 6 3
2 7 3
2 8 3

```




```input2
9 5
0 1 1
0 2 1
1 3 2
1 4 2
1 5 2
2 6 3
2 7 3
2 8 3

```




```input3
11 6
1 0 7932
2 1 1952
3 2 2227
4 0 9112
5 4 6067
6 0 6786
7 6 3883
8 4 7137
9 1 2796
10 5 6200

```




```output1
15

```




```output2
17

```




```output3
54092

```



## Note

<p>In the first example, the worst-case scenario for Heidi is to visit the friends in the following order: <span class="tex-span">0, 1, 5, 1, 3, 1, 0, 2, 6, 2, 7, 2, 8</span>. Observe that no friend is visited more than <span class="tex-span">3</span> times.</p>
