## Description

<div><p>Sereja owns a restaurant for <span class="tex-span"><i>n</i></span> people. The restaurant hall has a coat rack with <span class="tex-span"><i>n</i></span> hooks. Each restaurant visitor can use a hook to hang his clothes on it. Using the <span class="tex-span"><i>i</i></span>-th hook costs <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> rubles. Only one person can hang clothes on one hook.</p><p>Tonight Sereja expects <span class="tex-span"><i>m</i></span> guests in the restaurant. Naturally, each guest wants to hang his clothes on an available hook with minimum price (if there are multiple such hooks, he chooses any of them). However if the moment a guest arrives the rack has no available hooks, Sereja must pay a <span class="tex-span"><i>d</i></span> ruble fine to the guest. </p><p>Help Sereja find out the profit in rubles (possibly negative) that he will get tonight. You can assume that before the guests arrive, all hooks on the rack are available, all guests come at different time, nobody besides the <span class="tex-span"><i>m</i></span> guests is visiting Sereja's restaurant tonight.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>d</i> ≤ 100)</span>. The next line contains integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>. The third line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 100)</span>.</p></div><div class="output-specification"><p>In a single line print a single integer — the answer to the problem.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>d</i></span> <span class="tex-span">(1 ≤ <i>n</i>, <i>d</i> ≤ 100)</span>. The next line contains integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index">2</sub></span>, <span class="tex-span">...</span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100)</span>. The third line contains integer <span class="tex-span"><i>m</i></span> <span class="tex-span">(1 ≤ <i>m</i> ≤ 100)</span>.</p>

## Output

<p>In a single line print a single integer — the answer to the problem.</p>





```input1
2 1
2 1
2

```




```input2
2 1
2 1
10

```




```output1
3

```




```output2
-5

```



## Note

<p>In the first test both hooks will be used, so Sereja gets <span class="tex-span">1 + 2 = 3</span> rubles.</p><p>In the second test both hooks will be used but Sereja pays a fine <span class="tex-span">8</span> times, so the answer is <span class="tex-span">3 - 8 =  - 5</span>.</p>
