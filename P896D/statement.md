## Description

<div><p>Lakhesh loves to make movies, so Nephren helps her run a cinema. We may call it No. 68 Cinema.</p><center><p><img class="tex-graphics" src="file://0x4c3tMB.png" style="max-width: 100.0%;max-height: 100.0%;"></p></center><p>However, one day, the No. 68 Cinema runs out of changes (they don't have 50-<span class="tex-font-style-it">yuan</span> notes currently), but Nephren still wants to start their business. (Assume that <span class="tex-font-style-it">yuan</span> is a kind of currency in Regulu Ere.)</p><p>There are three types of customers: some of them bring exactly a 50-<span class="tex-font-style-it">yuan</span> note; some of them bring a 100-<span class="tex-font-style-it">yuan</span> note and Nephren needs to give a 50-<span class="tex-font-style-it">yuan</span> note back to him/her; some of them bring VIP cards so that they don't need to pay for the ticket.</p><p>Now <span class="tex-span"><i>n</i></span> customers are waiting outside in queue. Nephren wants to know how many possible queues are there that they are able to run smoothly (i.e. every customer can receive his/her change), and that the number of 50-<span class="tex-font-style-it">yuan</span> notes they have after selling tickets to all these customers is between <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span>, inclusive. Two queues are considered different if there exists a customer whose type is different in two queues. As the number can be large, please output the answer modulo <span class="tex-span"><i>p</i></span>.</p></div><div class="input-specification"><p>One line containing four integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ 2·10<sup class="upper-index">9</sup>)</span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">0 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>). </p></div><div class="output-specification"><p>One line indicating the answer modulo <span class="tex-span"><i>p</i></span>.</p></div>

## Input

<p>One line containing four integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, <span class="tex-span"><i>p</i></span> (<span class="tex-span">1 ≤ <i>p</i> ≤ 2·10<sup class="upper-index">9</sup>)</span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">0 ≤ <i>l</i> ≤ <i>r</i> ≤ <i>n</i></span>). </p>

## Output

<p>One line indicating the answer modulo <span class="tex-span"><i>p</i></span>.</p>





```input1
4 97 2 3

```




```input2
4 100 0 4

```




```output1
13

```




```output2
35

```



## Note

<p>We use A, B and C to indicate customers with 50-<span class="tex-font-style-it">yuan</span> notes, customers with 100-<span class="tex-font-style-it">yuan</span> notes and customers with VIP cards respectively.</p><p>For the first sample, the different possible queues that there are <span class="tex-span">2</span> 50-<span class="tex-font-style-it">yuan</span> notes left are AAAB, AABA, ABAA, AACC, ACAC, ACCA, CAAC, CACA and CCAA, and the different possible queues that there are <span class="tex-span">3</span> 50-<span class="tex-font-style-it">yuan</span> notes left are AAAC, AACA, ACAA and CAAA. So there are <span class="tex-span">13</span> different queues satisfying the first sample. Similarly, there are <span class="tex-span">35</span> different queues satisfying the second sample.</p>
