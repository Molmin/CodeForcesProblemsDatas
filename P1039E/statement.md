## Description

<div><p>While some people enjoy spending their time solving programming contests, Dina prefers taking beautiful pictures. As soon as Byteland Botanical Garden announced Summer Oenothera Exhibition she decided to test her new camera there.</p><p>The exhibition consists of $l = 10^{100}$ Oenothera species arranged in a row and consecutively numbered with integers from $0$ to $l - 1$. Camera lens allows to take a photo of $w$ species on it, i.e. Dina can take a photo containing flowers with indices from $x$ to $x + w - 1$ for some integer $x$ between $0$ and $l - w$. We will denote such photo with $[x, x + w - 1]$.</p><p>She has taken $n$ photos, the $i$-th of which (in chronological order) is $[x_i, x_i + w - 1]$ in our notation. She decided to build a time-lapse video from these photos once she discovered that Oenothera blossoms open in the evening. </p><p>Dina takes each photo and truncates it, leaving its segment containing exactly $k$ flowers, then she composes a video of these photos keeping their original order and voilà, a beautiful artwork has been created!</p><p>A scene is a contiguous sequence of photos such that the set of flowers on them is the same. The change between two scenes is called a <span class="tex-font-style-it">cut</span>. For example, consider the first photo contains flowers $[1, 5]$, the second photo contains flowers $[3, 7]$ and the third photo contains flowers $[8, 12]$. If $k = 3$, then Dina can truncate the first and the second photo into $[3, 5]$, and the third photo into $[9, 11]$. First two photos form a scene, third photo also forms a scene and the transition between these two scenes which happens between the second and the third photos is a cut. If $k = 4$, then each of the transitions between photos has to be a cut.</p><p>Dina wants the number of cuts to be as small as possible. Please help her! Calculate the minimum possible number of cuts for different values of $k$.</p></div><div class="input-specification"><p>The first line contains three positive integer $n$, $w$, $q$ ($1 \leq n, q \leq 100\,000$, $1 \leq w \leq 10^9$)&nbsp;— the number of taken photos, the number of flowers on a single photo and the number of queries.</p><p>Next line contains $n$ non-negative integers $x_i$ ($0 \le x_i \le 10^9$)&nbsp;— the indices of the leftmost flowers on each of the photos.</p><p>Next line contains $q$ positive integers $k_i$ ($1 \le k_i \le w$)&nbsp;— the values of $k$ for which you have to solve the problem.</p><p>It's guaranteed that all $k_i$ are distinct.</p></div><div class="output-specification"><p>Print $q$ integers&nbsp;— for each width of the truncated photo $k_i$, the minimum number of cuts that is possible.</p></div>

## Input

<p>The first line contains three positive integer $n$, $w$, $q$ ($1 \leq n, q \leq 100\,000$, $1 \leq w \leq 10^9$)&nbsp;— the number of taken photos, the number of flowers on a single photo and the number of queries.</p><p>Next line contains $n$ non-negative integers $x_i$ ($0 \le x_i \le 10^9$)&nbsp;— the indices of the leftmost flowers on each of the photos.</p><p>Next line contains $q$ positive integers $k_i$ ($1 \le k_i \le w$)&nbsp;— the values of $k$ for which you have to solve the problem.</p><p>It's guaranteed that all $k_i$ are distinct.</p>

## Output

<p>Print $q$ integers&nbsp;— for each width of the truncated photo $k_i$, the minimum number of cuts that is possible.</p>





```input1
3 6 5
2 4 0
1 2 3 4 5

```




```input2
6 4 3
1 2 3 4 3 2
1 2 3

```




```output1
0
0
1
1
2

```




```output2
0
1
2

```


