## Description

<div><p>Today on a math lesson the teacher told Vovochka that the Euler function of a positive integer <span class="tex-span">φ(<i>n</i>)</span> is an arithmetic function that counts the positive integers less than or equal to n that are relatively prime to n. The number <span class="tex-span">1</span> is coprime to all the positive integers and <span class="tex-span">φ(1) = 1</span>.</p><p>Now the teacher gave Vovochka an array of <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> and a task to process <span class="tex-span"><i>q</i></span> queries <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span>&nbsp;— to calculate and print <img align="middle" class="tex-formula" src="file://XR4IrtbR.png" style="max-width: 100.0%;max-height: 100.0%;"> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. As it is too hard for a second grade school student, you've decided to help Vovochka.</p></div><div class="input-specification"><p>The first line of the input contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the length of the array given to Vovochka. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The third line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>)&nbsp;— the number of queries. Next <span class="tex-span"><i>q</i></span> lines contain the queries, one per line. Each query is defined by the boundaries of the segment <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>q</i></span> numbers — the value of the Euler function for each query, calculated modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line of the input contains number <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the length of the array given to Vovochka. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>The third line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>)&nbsp;— the number of queries. Next <span class="tex-span"><i>q</i></span> lines contain the queries, one per line. Each query is defined by the boundaries of the segment <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>r</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ <i>r</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>).</p>

## Output

<p>Print <span class="tex-span"><i>q</i></span> numbers — the value of the Euler function for each query, calculated modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
10
1 2 3 4 5 6 7 8 9 10
7
1 1
3 8
5 6
4 8
8 10
7 9
7 10

```




```input2
7
24 63 13 52 6 10 1
6
3 5
4 7
1 7
2 4
3 6
2 6

```




```output1
1
4608
8
1536
192
144
1152

```




```output2
1248
768
12939264
11232
9984
539136

```



## Note

<p>In the second sample the values are calculated like that:</p><ul> <li> <span class="tex-span">φ(13·52·6) = φ(4056) = 1248</span> </li><li> <span class="tex-span">φ(52·6·10·1) = φ(3120) = 768</span> </li><li> <span class="tex-span">φ(24·63·13·52·6·10·1) = φ(61326720) = 12939264</span> </li><li> <span class="tex-span">φ(63·13·52) = φ(42588) = 11232</span> </li><li> <span class="tex-span">φ(13·52·6·10) = φ(40560) = 9984</span> </li><li> <span class="tex-span">φ(63·13·52·6·10) = φ(2555280) = 539136</span> </li></ul>
