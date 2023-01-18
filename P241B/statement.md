## Description

<div><p>You have <span class="tex-span"><i>n</i></span> friends and you want to take <span class="tex-span"><i>m</i></span> pictures of them. Exactly two of your friends should appear in each picture and no two pictures should contain the same pair of your friends. So if you have <span class="tex-span"><i>n</i> = 3</span> friends you can take <span class="tex-span">3</span> different pictures, each containing a pair of your friends.</p><p>Each of your friends has an attractiveness level which is specified by the integer number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> for the <span class="tex-span"><i>i</i></span>-th friend. You know that the attractiveness of a picture containing the <span class="tex-span"><i>i</i></span>-th and the <span class="tex-span"><i>j</i></span>-th friends is equal to the exclusive-or (<span class="tex-span"><i>xor</i></span> operation) of integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>a</i><sub class="lower-index"><i>j</i></sub></span>.</p><p>You want to take pictures in a way that the total sum of attractiveness of your pictures is maximized. You have to calculate this value. Since the result may not fit in a 32-bit integer number, print it modulo <span class="tex-span">1000000007</span> <span class="tex-span">(10<sup class="upper-index">9</sup> + 7)</span>.</p></div><div class="input-specification"><p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <img align="middle" class="tex-formula" src="file://iDge2mwk.png" style="max-width: 100.0%;max-height: 100.0%;"> — the number of friends and the number of pictures that you want to take. </p><p>Next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the values of attractiveness of the friends.</p></div><div class="output-specification"><p>The only line of output should contain an integer — the optimal total sum of attractiveness of your pictures.</p></div>

## Input

<p>The first line of input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> <img align="middle" class="tex-formula" src="file://iDge2mwk.png" style="max-width: 100.0%;max-height: 100.0%;"> — the number of friends and the number of pictures that you want to take. </p><p>Next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>) — the values of attractiveness of the friends.</p>

## Output

<p>The only line of output should contain an integer — the optimal total sum of attractiveness of your pictures.</p>





```input1
3 1
1 2 3

```




```input2
3 2
1 2 3

```




```input3
3 3
1 2 3

```




```output1
3

```




```output2
5

```




```output3
6

```


