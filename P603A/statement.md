## Description

<div><p>Kevin has just recevied his disappointing results on the USA Identification of Cows Olympiad (USAICO) in the form of a binary string of length <span class="tex-span"><i>n</i></span>. Each character of Kevin's string represents Kevin's score on one of the <span class="tex-span"><i>n</i></span> questions of the olympiad—<span class="tex-font-style-tt">'1'</span> for a correctly identified cow and <span class="tex-font-style-tt">'0'</span> otherwise.</p><p>However, all is not lost. Kevin is a big proponent of alternative thinking and believes that his score, instead of being the sum of his points, should be the length of the longest alternating subsequence of his string. Here, we define an <span class="tex-font-style-underline">alternating subsequence</span> of a string as a <span class="tex-font-style-bf">not-necessarily contiguous</span> subsequence where no two consecutive elements are equal. For example, <span class="tex-span">{0, 1, 0, 1}</span>, <span class="tex-span">{1, 0, 1}</span>, and <span class="tex-span">{1, 0, 1, 0}</span> are alternating sequences, while <span class="tex-span">{1, 0, 0}</span> and <span class="tex-span">{0, 1, 0, 1, 1}</span> are not.</p><p>Kevin, being the sneaky little puffball that he is, is willing to hack into the USAICO databases to improve his score. In order to be subtle, he decides that he will flip exactly one substring—that is, take a <span class="tex-font-style-bf">contiguous</span> non-empty substring of his score and change all <span class="tex-font-style-tt">'0'</span>s in that substring to <span class="tex-font-style-tt">'1'</span>s and vice versa. After such an operation, Kevin wants to know the length of the longest possible alternating subsequence that his string could have.</p></div><div class="input-specification"><p>The first line contains the number of questions on the olympiad <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>).</p><p>The following line contains a binary string of length <span class="tex-span"><i>n</i></span> representing Kevin's results on the USAICO. </p></div><div class="output-specification"><p>Output a single integer, the length of the longest possible alternating subsequence that Kevin can create in his string after flipping a single substring.</p></div>

## Input

<p>The first line contains the number of questions on the olympiad <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100 000</span>).</p><p>The following line contains a binary string of length <span class="tex-span"><i>n</i></span> representing Kevin's results on the USAICO. </p>

## Output

<p>Output a single integer, the length of the longest possible alternating subsequence that Kevin can create in his string after flipping a single substring.</p>





```input1
8
10000011

```




```input2
2
01

```




```output1
5

```




```output2
2

```



## Note

<p>In the first sample, Kevin can flip the bolded substring '<span class="tex-font-style-tt">100</span><span class="tex-font-style-bf">00</span><span class="tex-font-style-tt">011</span>' and turn his string into '<span class="tex-font-style-tt">10011011</span>', which has an alternating subsequence of length 5: '<span class="tex-font-style-bf">1</span><span class="tex-font-style-tt">0</span><span class="tex-font-style-bf">01</span><span class="tex-font-style-tt">1</span><span class="tex-font-style-bf">01</span><span class="tex-font-style-tt">1</span>'.</p><p>In the second sample, Kevin can flip the entire string and still have the same score.</p>
