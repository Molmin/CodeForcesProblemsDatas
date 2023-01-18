## Description

<div><p>One of Arkady's friends works at a huge radio telescope. A few decades ago the telescope has sent a signal $s$ towards a faraway galaxy. Recently they've received a response $t$ which they believe to be a response from aliens! The scientists now want to check if the signal $t$ is similar to $s$.</p><p>The original signal $s$ was a sequence of zeros and ones (everyone knows that binary code is the universe-wide language). The returned signal $t$, however, does not look as easy as $s$, but the scientists don't give up! They represented $t$ as a sequence of English letters and say that $t$ is similar to $s$ if you can replace all zeros in $s$ with some string $r_0$ and all ones in $s$ with some other string $r_1$ and obtain $t$. The strings $r_0$ and $r_1$ must be different and non-empty.</p><p>Please help Arkady's friend and find the number of possible replacements for zeros and ones (the number of pairs of strings $r_0$ and $r_1$) that transform $s$ to $t$.</p></div><div class="input-specification"><p>The first line contains a string $s$ ($2 \le |s| \le 10^5$) consisting of zeros and ones&nbsp;— the original signal.</p><p>The second line contains a string $t$ ($1 \le |t| \le 10^6$) consisting of lowercase English letters only&nbsp;— the received signal.</p><p>It is guaranteed, that the string $s$ contains at least one '<span class="tex-font-style-tt">0</span>' and at least one '<span class="tex-font-style-tt">1</span>'.</p></div><div class="output-specification"><p>Print a single integer&nbsp;— the number of pairs of strings $r_0$ and $r_1$ that transform $s$ to $t$.</p><p>In case there are no such pairs, print $0$.</p></div>

## Input

<p>The first line contains a string $s$ ($2 \le |s| \le 10^5$) consisting of zeros and ones&nbsp;— the original signal.</p><p>The second line contains a string $t$ ($1 \le |t| \le 10^6$) consisting of lowercase English letters only&nbsp;— the received signal.</p><p>It is guaranteed, that the string $s$ contains at least one '<span class="tex-font-style-tt">0</span>' and at least one '<span class="tex-font-style-tt">1</span>'.</p>

## Output

<p>Print a single integer&nbsp;— the number of pairs of strings $r_0$ and $r_1$ that transform $s$ to $t$.</p><p>In case there are no such pairs, print $0$.</p>





```input1
01
aaaaaa
```




```input2
001
kokokokotlin
```




```output1
4
```




```output2
2
```



## Note

<p>In the first example, the possible pairs $(r_0, r_1)$ are as follows:</p><ul> <li> "<span class="tex-font-style-tt">a</span>", "<span class="tex-font-style-tt">aaaaa</span>" </li><li> "<span class="tex-font-style-tt">aa</span>", "<span class="tex-font-style-tt">aaaa</span>" </li><li> "<span class="tex-font-style-tt">aaaa</span>", "<span class="tex-font-style-tt">aa</span>" </li><li> "<span class="tex-font-style-tt">aaaaa</span>", "<span class="tex-font-style-tt">a</span>" </li></ul> <p>The pair "<span class="tex-font-style-tt">aaa</span>", "<span class="tex-font-style-tt">aaa</span>" is not allowed, since $r_0$ and $r_1$ must be different.</p><p>In the second example, the following pairs are possible: </p><ul> <li> "<span class="tex-font-style-tt">ko</span>", "<span class="tex-font-style-tt">kokotlin</span>" </li><li> "<span class="tex-font-style-tt">koko</span>", "<span class="tex-font-style-tt">tlin</span>" </li></ul>
