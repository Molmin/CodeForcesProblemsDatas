## Description

<div><p>Princess Twilight went to Celestia and Luna's old castle to research the chest from the Elements of Harmony.</p><center> <img class="tex-graphics" src="file://sNqeqqyw.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>A sequence of positive integers <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is harmony if and only if for every two elements of the sequence their greatest common divisor equals 1. According to an ancient book, the key of the chest is a harmony sequence <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> which minimizes the following expression:</p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://Q2HKFFlr.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>You are given sequence <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, help Princess Twilight to find the key.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of elements of the sequences <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 30</span>).</p></div><div class="output-specification"><p>Output the key — sequence <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> that minimizes the sum described above. If there are multiple optimal sequences, you can output any of them.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of elements of the sequences <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span>. The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 30</span>).</p>

## Output

<p>Output the key — sequence <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> that minimizes the sum described above. If there are multiple optimal sequences, you can output any of them.</p>





```input1
5
1 1 1 1 1

```




```input2
5
1 6 4 2 8

```




```output1
1 1 1 1 1
```




```output2
1 5 3 1 8
```


