## Description

<div><p>There are <span class="tex-span"><i>n</i></span> walruses standing in a queue in an airport. They are numbered starting from the queue's tail: the <span class="tex-span">1</span>-st walrus stands at the end of the queue and the <span class="tex-span"><i>n</i></span>-th walrus stands at the beginning of the queue. The <span class="tex-span"><i>i</i></span>-th walrus has the age equal to <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>.</p><p>The <span class="tex-span"><i>i</i></span>-th walrus becomes displeased if there's a younger walrus standing in front of him, that is, if exists such <span class="tex-span"><i>j</i></span> (<span class="tex-span"><i>i</i> &lt; <i>j</i></span>), that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> &gt; <i>a</i><sub class="lower-index"><i>j</i></sub></span>. The <span class="tex-font-style-underline">displeasure</span> of the <span class="tex-span"><i>i</i></span>-th walrus is equal to the number of walruses between him and the furthest walrus ahead of him, which is younger than the <span class="tex-span"><i>i</i></span>-th one. That is, the further that young walrus stands from him, the stronger the displeasure is.</p><p>The airport manager asked you to count for each of <span class="tex-span"><i>n</i></span> walruses in the queue his displeasure.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of walruses in the queue. The second line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Note that some walruses can have the same age but for the displeasure to emerge the walrus that is closer to the head of the queue needs to be <span class="tex-font-style-bf">strictly younger</span> than the other one.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> numbers: if the <span class="tex-span"><i>i</i></span>-th walrus is pleased with everything, print "-1" (without the quotes). Otherwise, print the <span class="tex-span"><i>i</i></span>-th walrus's displeasure: the number of other walruses that stand between him and the furthest from him younger walrus.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of walruses in the queue. The second line contains integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>).</p><p>Note that some walruses can have the same age but for the displeasure to emerge the walrus that is closer to the head of the queue needs to be <span class="tex-font-style-bf">strictly younger</span> than the other one.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> numbers: if the <span class="tex-span"><i>i</i></span>-th walrus is pleased with everything, print "-1" (without the quotes). Otherwise, print the <span class="tex-span"><i>i</i></span>-th walrus's displeasure: the number of other walruses that stand between him and the furthest from him younger walrus.</p>





```input1
6
10 8 5 3 50 45

```




```input2
7
10 4 6 3 2 8 15

```




```input3
5
10 3 1 10 11

```




```output1
2 1 0 -1 0 -1
```




```output2
4 2 1 0 -1 -1 -1
```




```output3
1 0 -1 -1 -1
```


