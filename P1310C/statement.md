## Description

<div><p>VK just opened its second HQ in St. Petersburg! Side of its office building has a huge string $s$ written on its side. This part of the office is supposed to be split into $m$ meeting rooms in such way that meeting room walls are strictly between letters on the building. Obviously, meeting rooms should not be of size 0, but can be as small as one letter wide. Each meeting room will be named after the substring of $s$ written on its side.</p><center><img class="tex-graphics" src="file://sdLnW6KY.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>For each possible arrangement of $m$ meeting rooms we ordered a test meeting room label for the meeting room with lexicographically <span class="tex-font-style-bf">minimal</span> name. When delivered, those labels got sorted <span class="tex-font-style-bf">backward</span> lexicographically.</p><p>What is printed on $k$th label of the delivery?</p></div><div class="input-specification"><p>In the first line, you are given three integer numbers $n, m, k$&nbsp;— length of string $s$, number of planned meeting rooms to split $s$ into and number of the interesting label ($2 \le n \le 1\,000; 1 \le m \le 1\,000; 1 \le k \le 10^{18}$).</p><p>Second input line has string $s$, consisting of $n$ lowercase english letters.</p><p>For given $n, m, k$ there are at least $k$ ways to split $s$ into $m$ substrings.</p></div><div class="output-specification"><p>Output single string – name of meeting room printed on $k$-th label of the delivery.</p></div>

## Input

<p>In the first line, you are given three integer numbers $n, m, k$&nbsp;— length of string $s$, number of planned meeting rooms to split $s$ into and number of the interesting label ($2 \le n \le 1\,000; 1 \le m \le 1\,000; 1 \le k \le 10^{18}$).</p><p>Second input line has string $s$, consisting of $n$ lowercase english letters.</p><p>For given $n, m, k$ there are at least $k$ ways to split $s$ into $m$ substrings.</p>

## Output

<p>Output single string – name of meeting room printed on $k$-th label of the delivery.</p>





```input1
4 2 1
abac
```




```input2
19 5 1821
aupontrougevkoffice
```




```output1
aba
```




```output2
au
```



## Note

<p>In the first example, delivery consists of the labels "<span class="tex-font-style-tt">aba</span>", "<span class="tex-font-style-tt">ab</span>", "<span class="tex-font-style-tt">a</span>".</p><p>In the second example, delivery consists of $3060$ labels. The first label is "<span class="tex-font-style-tt">aupontrougevkof</span>" and the last one is "<span class="tex-font-style-tt">a</span>".</p>
