## Description

<div><p>ATMs of a well-known bank of a small country are arranged so that they can not give any amount of money requested by the user. Due to the limited size of the bill dispenser (the device that is directly giving money from an ATM) and some peculiarities of the ATM structure, you can get at most <span class="tex-span"><i>k</i></span> bills from it, and the bills may be of at most two distinct denominations.</p><p>For example, if a country uses bills with denominations <span class="tex-span">10</span>, <span class="tex-span">50</span>, <span class="tex-span">100</span>, <span class="tex-span">500</span>, <span class="tex-span">1000</span> and <span class="tex-span">5000</span> burles, then at <span class="tex-span"><i>k</i> = 20</span> such ATM can give sums <span class="tex-span">100 000</span> burles and <span class="tex-span">96 000</span> burles, but it cannot give sums <span class="tex-span">99 000</span> and <span class="tex-span">101 000</span> burles.</p><p>Let's suppose that the country uses bills of <span class="tex-span"><i>n</i></span> distinct denominations, and the ATM that you are using has an unlimited number of bills of each type. You know that during the day you will need to withdraw a certain amount of cash <span class="tex-span"><i>q</i></span> times. You know that when the ATM has multiple ways to give money, it chooses the one which requires the minimum number of bills, or displays an error message if it cannot be done. Determine the result of each of the <span class="tex-span"><i>q</i></span> of requests for cash withdrawal.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 20</span>).</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>) — the denominations of the bills that are used in the country. Numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> follow in the strictly increasing order.</p><p>The next line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 20</span>) — the number of requests for cash withdrawal that you will make.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">8</sup></span>) — the sums of money in burles that you are going to withdraw from the ATM.</p></div><div class="output-specification"><p>For each request for cash withdrawal print on a single line the minimum number of bills it can be done, or print <span class="tex-span"> - 1</span>, if it is impossible to get the corresponding sum.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 5000</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 20</span>).</p><p>The next line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">7</sup></span>) — the denominations of the bills that are used in the country. Numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> follow in the strictly increasing order.</p><p>The next line contains integer <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>q</i> ≤ 20</span>) — the number of requests for cash withdrawal that you will make.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain numbers <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ 2·10<sup class="upper-index">8</sup></span>) — the sums of money in burles that you are going to withdraw from the ATM.</p>

## Output

<p>For each request for cash withdrawal print on a single line the minimum number of bills it can be done, or print <span class="tex-span"> - 1</span>, if it is impossible to get the corresponding sum.</p>





```input1
6 20
10 50 100 500 1000 5000
8
4200
100000
95000
96000
99000
10100
2015
9950

```




```input2
5 2
1 2 3 5 8
8
1
3
5
7
9
11
13
15

```




```output1
6
20
19
20
-1
3
-1
-1

```




```output2
1
1
1
2
2
2
2
-1

```


