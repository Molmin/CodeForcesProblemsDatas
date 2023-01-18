## Description

<div><p>There are <span class="tex-span"><i>n</i></span> students who have taken part in an olympiad. Now it's time to award the students.</p><p>Some of them will receive diplomas, some wiil get certificates, and others won't receive anything. Students with diplomas and certificates are called <span class="tex-font-style-it">winners</span>. But there are some rules of counting the number of diplomas and certificates. The number of certificates must be <span class="tex-font-style-bf">exactly</span> <span class="tex-span"><i>k</i></span> times greater than the number of diplomas. The number of <span class="tex-font-style-it">winners</span> must <span class="tex-font-style-bf">not be greater than half of the number of all students</span> (i.e. not be greater than half of <span class="tex-span"><i>n</i></span>). It's possible that there are no <span class="tex-font-style-it">winners</span>.</p><p>You have to identify the maximum possible number of <span class="tex-font-style-it">winners</span>, according to these rules. Also for this case you have to calculate the number of students with diplomas, the number of students with certificates and the number of students who are not <span class="tex-font-style-it">winners</span>.</p></div><div class="input-specification"><p>The first (and the only) line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">12</sup></span>), where <span class="tex-span"><i>n</i></span> is the number of students and <span class="tex-span"><i>k</i></span> is the ratio between the number of certificates and the number of diplomas.</p></div><div class="output-specification"><p>Output three numbers: the number of students with diplomas, the number of students with certificates and the number of students who are not <span class="tex-font-style-it">winners</span> in case when the number of <span class="tex-font-style-it">winners</span> is maximum possible.</p><p>It's possible that there are no <span class="tex-font-style-it">winners</span>.</p></div>

## Input

<p>The first (and the only) line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>k</i> ≤ 10<sup class="upper-index">12</sup></span>), where <span class="tex-span"><i>n</i></span> is the number of students and <span class="tex-span"><i>k</i></span> is the ratio between the number of certificates and the number of diplomas.</p>

## Output

<p>Output three numbers: the number of students with diplomas, the number of students with certificates and the number of students who are not <span class="tex-font-style-it">winners</span> in case when the number of <span class="tex-font-style-it">winners</span> is maximum possible.</p><p>It's possible that there are no <span class="tex-font-style-it">winners</span>.</p>





```input1
18 2

```




```input2
9 10

```




```input3
1000000000000 5

```




```input4
1000000000000 499999999999

```




```output1
3 6 9

```




```output2
0 0 9

```




```output3
83333333333 416666666665 500000000002

```




```output4
1 499999999999 500000000000

```


