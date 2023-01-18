## Description

<div><p>One common way of digitalizing sound is to record sound intensity at particular time moments. For each time moment intensity is recorded as a non-negative integer. Thus we can represent a sound file as an array of $n$ non-negative integers.</p><p>If there are exactly $K$ distinct values in the array, then we need $k = \lceil \log_{2} K \rceil$ bits to store each value. It then takes $nk$ bits to store the whole file.</p><p>To reduce the memory consumption we need to apply some compression. One common way is to reduce the number of possible intensity values. We choose two integers $l \le r$, and after that all intensity values are changed in the following way: if the intensity value is within the range $[l;r]$, we don't change it. If it is less than $l$, we change it to $l$; if it is greater than $r$, we change it to $r$. You can see that we lose some low and some high intensities.</p><p>Your task is to apply this compression in such a way that the file fits onto a disk of size $I$ bytes, and the number of changed elements in the array is minimal possible.</p><p>We remind you that $1$ byte contains $8$ bits.</p><p>$k = \lceil log_{2} K \rceil$ is the smallest integer such that $K \le 2^{k}$. In particular, if $K = 1$, then $k = 0$.</p></div><div class="input-specification"><p>The first line contains two integers $n$ and $I$ ($1 \le n \le 4 \cdot 10^{5}$, $1 \le I \le 10^{8}$)&nbsp;— the length of the array and the size of the disk in bytes, respectively.</p><p>The next line contains $n$ integers $a_{i}$ ($0 \le a_{i} \le 10^{9}$)&nbsp;— the array denoting the sound file.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimal possible number of changed elements.</p></div>

## Input

<p>The first line contains two integers $n$ and $I$ ($1 \le n \le 4 \cdot 10^{5}$, $1 \le I \le 10^{8}$)&nbsp;— the length of the array and the size of the disk in bytes, respectively.</p><p>The next line contains $n$ integers $a_{i}$ ($0 \le a_{i} \le 10^{9}$)&nbsp;— the array denoting the sound file.</p>

## Output

<p>Print a single integer&nbsp;— the minimal possible number of changed elements.</p>





```input1
6 1
2 1 2 3 4 3
```




```input2
6 2
2 1 2 3 4 3
```




```input3
6 1
1 1 2 2 3 3
```




```output1
2
```




```output2
0
```




```output3
2
```



## Note

<p>In the first example we can choose $l=2, r=3$. The array becomes <span class="tex-font-style-tt">2 2 2 3 3 3</span>, the number of distinct elements is $K=2$, and the sound file fits onto the disk. Only two values are changed.</p><p>In the second example the disk is larger, so the initial file fits it and no changes are required.</p><p>In the third example we have to change both 1s or both 3s.</p>
