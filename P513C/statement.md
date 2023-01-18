## Description

<div><p>Nowadays, most of the internet advertisements are not statically linked to a web page. Instead, what will be shown to the person opening a web page is determined within 100 milliseconds after the web page is opened. Usually, multiple companies compete for each ad slot on the web page in an auction. Each of them receives a request with details about the user, web page and ad slot and they have to respond within those 100 milliseconds with a bid they would pay for putting an advertisement on that ad slot. The company that suggests the highest bid wins the auction and gets to place its advertisement. If there are several companies tied for the highest bid, the winner gets picked at random.</p><p>However, the company that won the auction does not have to pay the exact amount of its bid. In most of the cases, a second-price auction is used. This means that the amount paid by the company is equal to the maximum of all the other bids placed for this ad slot.</p><p>Let's consider one such bidding. There are <span class="tex-span"><i>n</i></span> companies competing for placing an ad. The <span class="tex-span"><i>i</i></span>-th of these companies will bid an integer number of microdollars equiprobably randomly chosen from the range between <span class="tex-span"><i>L</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span>, inclusive. In the other words, the value of the <span class="tex-span"><i>i</i></span>-th company bid can be any integer from the range <span class="tex-span">[<i>L</i><sub class="lower-index"><i>i</i></sub>, <i>R</i><sub class="lower-index"><i>i</i></sub>]</span> with the same probability. </p><p>Determine the expected value that the winner will have to pay in a second-price auction.</p></div><div class="input-specification"><p>The first line of input contains an integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5</span>). <span class="tex-span"><i>n</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th of them containing two numbers <span class="tex-span"><i>L</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>L</i><sub class="lower-index"><i>i</i></sub> ≤ <i>R</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>) describing the <span class="tex-span"><i>i</i></span>-th company's bid preferences.</p><p><span class="tex-font-style-it">This problem doesn't have subproblems. You will get 8 points for the correct submission.</span></p></div><div class="output-specification"><p>Output the answer with absolute or relative error no more than <span class="tex-span">1<i>e</i> - 9</span>.</p></div>

## Input

<p>The first line of input contains an integer number <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 5</span>). <span class="tex-span"><i>n</i></span> lines follow, the <span class="tex-span"><i>i</i></span>-th of them containing two numbers <span class="tex-span"><i>L</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>R</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>L</i><sub class="lower-index"><i>i</i></sub> ≤ <i>R</i><sub class="lower-index"><i>i</i></sub> ≤ 10000</span>) describing the <span class="tex-span"><i>i</i></span>-th company's bid preferences.</p><p><span class="tex-font-style-it">This problem doesn't have subproblems. You will get 8 points for the correct submission.</span></p>

## Output

<p>Output the answer with absolute or relative error no more than <span class="tex-span">1<i>e</i> - 9</span>.</p>





```input1
3
4 7
8 10
5 5

```




```input2
3
2 5
3 4
1 6

```




```output1
5.7500000000

```




```output2
3.5000000000

```



## Note

<p>Consider the first example. The first company bids a random integer number of microdollars in range <span class="tex-span">[4, 7]</span>; the second company bids between <span class="tex-span">8</span> and <span class="tex-span">10</span>, and the third company bids <span class="tex-span">5</span> microdollars. The second company will win regardless of the exact value it bids, however the price it will pay depends on the value of first company's bid. With probability <span class="tex-span">0.5</span> the first company will bid at most <span class="tex-span">5</span> microdollars, and the second-highest price of the whole auction will be <span class="tex-span">5</span>. With probability <span class="tex-span">0.25</span> it will bid <span class="tex-span">6</span> microdollars, and with probability <span class="tex-span">0.25</span> it will bid <span class="tex-span">7</span> microdollars. Thus, the expected value the second company will have to pay is <span class="tex-span">0.5·5 + 0.25·6 + 0.25·7 = 5.75</span>.</p>
