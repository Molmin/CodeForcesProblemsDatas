## Description

<div><p>The Little Elephant has an integer <span class="tex-span"><i>a</i></span>, written in the binary notation. He wants to write this number on a piece of paper.</p><p>To make sure that the number <span class="tex-span"><i>a</i></span> fits on the piece of paper, the Little Elephant <span class="tex-font-style-bf">ought</span> to delete exactly one any digit from number <span class="tex-span"><i>a</i></span> in the binary record. At that a new number appears. It consists of the remaining binary digits, written in the corresponding order (possible, with leading zeroes).</p><p>The Little Elephant wants the number he is going to write on the paper to be as large as possible. Help him find the maximum number that he can obtain after deleting exactly one binary digit and print it in the binary notation.</p></div><div class="input-specification"><p>The single line contains integer <span class="tex-span"><i>a</i></span>, written in the binary notation without leading zeroes. This number contains more than <span class="tex-span">1</span> and at most <span class="tex-span">10<sup class="upper-index">5</sup></span> digits.</p></div><div class="output-specification"><p>In the single line print the number that is written without leading zeroes in the binary notation — the answer to the problem.</p></div>

## Input

<p>The single line contains integer <span class="tex-span"><i>a</i></span>, written in the binary notation without leading zeroes. This number contains more than <span class="tex-span">1</span> and at most <span class="tex-span">10<sup class="upper-index">5</sup></span> digits.</p>

## Output

<p>In the single line print the number that is written without leading zeroes in the binary notation — the answer to the problem.</p>





```input1
101

```




```input2
110010

```




```output1
11

```




```output2
11010

```



## Note

<p>In the first sample the best strategy is to delete the second digit. That results in number <span class="tex-span">11<sub class="lower-index">2</sub> = 3<sub class="lower-index">10</sub></span>.</p><p>In the second sample the best strategy is to delete the third or fourth digits — that results in number <span class="tex-span">11010<sub class="lower-index">2</sub> = 26<sub class="lower-index">10</sub></span>.</p>
