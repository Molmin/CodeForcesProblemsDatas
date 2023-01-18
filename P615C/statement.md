## Description

<div><p>A boy named Ayrat lives on planet AMI-1511. Each inhabitant of this planet has a talent. Specifically, Ayrat loves running, moreover, just running is not enough for him. He is dreaming of making running a real art.</p><p>First, he wants to construct the running track with coating <span class="tex-span"><i>t</i></span>. On planet AMI-1511 the coating of the track is the sequence of colored blocks, where each block is denoted as the small English letter. Therefore, every coating can be treated as a string.</p><p>Unfortunately, blocks aren't freely sold to non-business customers, but Ayrat found an infinite number of coatings <span class="tex-span"><i>s</i></span>. Also, he has scissors and glue. Ayrat is going to buy some coatings <span class="tex-span"><i>s</i></span>, then cut out from each of them <span class="tex-font-style-bf">exactly one continuous piece</span> (substring) and glue it to the end of his track coating. Moreover, he may choose to flip this block before glueing it. Ayrat want's to know the minimum number of coating <span class="tex-span"><i>s</i></span> he needs to buy in order to get the coating <span class="tex-span"><i>t</i></span> for his running track. Of course, he also want's to know some way to achieve the answer.</p></div><div class="input-specification"><p>First line of the input contains the string <span class="tex-span"><i>s</i></span>&nbsp;— the coating that is present in the shop. Second line contains the string <span class="tex-span"><i>t</i></span>&nbsp;— the coating Ayrat wants to obtain. Both strings are non-empty, consist of only small English letters and their length doesn't exceed <span class="tex-span">2100</span>.</p></div><div class="output-specification"><p>The first line should contain the minimum needed number of coatings <span class="tex-span"><i>n</i></span> or <span class="tex-font-style-tt">-1</span> if it's impossible to create the desired coating.</p><p>If the answer is not <span class="tex-font-style-tt">-1</span>, then the following <span class="tex-span"><i>n</i></span> lines should contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— numbers of ending blocks in the corresponding piece. If <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>y</i><sub class="lower-index"><i>i</i></sub></span> then this piece is used in the regular order, and if <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &gt; <i>y</i><sub class="lower-index"><i>i</i></sub></span> piece is used in the reversed order. Print the pieces in the order they should be glued to get the string <span class="tex-span"><i>t</i></span>.</p></div>

## Input

<p>First line of the input contains the string <span class="tex-span"><i>s</i></span>&nbsp;— the coating that is present in the shop. Second line contains the string <span class="tex-span"><i>t</i></span>&nbsp;— the coating Ayrat wants to obtain. Both strings are non-empty, consist of only small English letters and their length doesn't exceed <span class="tex-span">2100</span>.</p>

## Output

<p>The first line should contain the minimum needed number of coatings <span class="tex-span"><i>n</i></span> or <span class="tex-font-style-tt">-1</span> if it's impossible to create the desired coating.</p><p>If the answer is not <span class="tex-font-style-tt">-1</span>, then the following <span class="tex-span"><i>n</i></span> lines should contain two integers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— numbers of ending blocks in the corresponding piece. If <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>y</i><sub class="lower-index"><i>i</i></sub></span> then this piece is used in the regular order, and if <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub> &gt; <i>y</i><sub class="lower-index"><i>i</i></sub></span> piece is used in the reversed order. Print the pieces in the order they should be glued to get the string <span class="tex-span"><i>t</i></span>.</p>





```input1
abc
cbaabc

```




```input2
aaabrytaaa
ayrat

```




```input3
ami
no

```




```output1
2
3 1
1 3

```




```output2
3
1 1
6 5
8 7

```




```output3
-1

```



## Note

<p>In the first sample string "<span class="tex-font-style-tt">cbaabc</span>" = "<span class="tex-font-style-tt">cba</span>" + "<span class="tex-font-style-tt">abc</span>".</p><p>In the second sample: "<span class="tex-font-style-tt">ayrat</span>" = "<span class="tex-font-style-tt">a</span>" + "<span class="tex-font-style-tt">yr</span>" + "<span class="tex-font-style-tt">at</span>".</p>
