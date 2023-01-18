## Description

<div><p><span class="tex-font-style-bf">The only difference between easy and hard versions is the constraints.</span></p><p>Vova likes pictures with kittens. The news feed in the social network he uses can be represented as an array of $n$ consecutive pictures (with kittens, of course). Vova likes all these pictures, but some are more beautiful than the others: the $i$-th picture has beauty $a_i$.</p><p>Vova wants to repost exactly $x$ pictures in such a way that: </p><ul> <li> each segment of the news feed of at least $k$ consecutive pictures has at least one picture reposted by Vova; </li><li> the sum of beauty values of reposted pictures is maximum possible. </li></ul><p>For example, if $k=1$ then Vova has to repost all the pictures in the news feed. If $k=2$ then Vova can skip some pictures, but between every pair of consecutive pictures Vova has to repost at least one of them.</p><p>Your task is to calculate the maximum possible sum of values of reposted pictures if Vova follows conditions described above, or say that there is no way to satisfy all conditions.</p></div><div class="input-specification"><p>The first line of the input contains three integers $n, k$ and $x$ ($1 \le k, x \le n \le 5000$) — the number of pictures in the news feed, the minimum length of segment with at least one repost in it and the number of pictures Vova is ready to repost.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the beauty of the $i$-th picture.</p></div><div class="output-specification"><p>Print <span class="tex-font-style-tt">-1</span> if there is no way to repost some pictures to satisfy all the conditions in the problem statement.</p><p>Otherwise print one integer — the maximum sum of values of reposted pictures if Vova follows conditions described in the problem statement.</p></div>

## Input

<p>The first line of the input contains three integers $n, k$ and $x$ ($1 \le k, x \le n \le 5000$) — the number of pictures in the news feed, the minimum length of segment with at least one repost in it and the number of pictures Vova is ready to repost.</p><p>The second line of the input contains $n$ integers $a_1, a_2, \dots, a_n$ ($1 \le a_i \le 10^9$), where $a_i$ is the beauty of the $i$-th picture.</p>

## Output

<p>Print <span class="tex-font-style-tt">-1</span> if there is no way to repost some pictures to satisfy all the conditions in the problem statement.</p><p>Otherwise print one integer — the maximum sum of values of reposted pictures if Vova follows conditions described in the problem statement.</p>





```input1
5 2 3
5 1 3 10 1
```




```input2
6 1 5
10 30 30 70 10 10
```




```input3
4 3 1
1 100 1 1
```




```output1
18
```




```output2
-1
```




```output3
100
```


