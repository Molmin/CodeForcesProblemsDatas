## Description

<div><p>You are running for a governor in a small city in Russia. You ran some polls and did some research, and for every person in the city you know whom he will vote for, and how much it will cost to bribe that person to vote for you instead of whomever he wants to vote for right now. You are curious, what is the smallest amount of money you need to spend on bribing to win the elections. To win elections you need to have strictly more votes than any other candidate.</p></div><div class="input-specification"><p>First line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of voters in the city. Each of the next <span class="tex-span"><i>n</i></span> lines describes one voter and contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — number of the candidate that voter is going to vote for and amount of money you need to pay him to change his mind. You are the candidate <span class="tex-span">0</span> (so if a voter wants to vote for you, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to zero, in which case <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> will also be equal to zero).</p></div><div class="output-specification"><p>Print one integer — smallest amount of money you need to spend to win the elections.</p></div>

## Input

<p>First line contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — number of voters in the city. Each of the next <span class="tex-span"><i>n</i></span> lines describes one voter and contains two integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup>;&nbsp;0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">4</sup></span>) — number of the candidate that voter is going to vote for and amount of money you need to pay him to change his mind. You are the candidate <span class="tex-span">0</span> (so if a voter wants to vote for you, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to zero, in which case <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> will also be equal to zero).</p>

## Output

<p>Print one integer — smallest amount of money you need to spend to win the elections.</p>





```input1
5
1 2
1 2
1 2
2 1
0 0

```




```input2
4
1 2
1 2
2 1
0 0

```




```input3
1
100000 0

```




```output1
3

```




```output2
2

```




```output3
0

```


