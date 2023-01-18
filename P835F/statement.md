## Description

<div><p>In the Kingdom K., there are <span class="tex-span"><i>n</i></span> towns numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The towns are connected by <span class="tex-span"><i>n</i></span> bi-directional roads numbered with integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The <span class="tex-span"><i>i</i></span>-th road connects the towns <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span> and <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span> and its length is <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span>. There is no more than one road between two towns. Also, there are no roads that connect the towns with itself.</p><p>Let's call the inconvenience of the roads the maximum of the shortest distances between all pairs of towns.</p><p>Because of lack of money, it was decided to close down one of the roads so that after its removal it is still possible to reach any town from any other. You have to find the minimum possible inconvenience of the roads after closing down one of the roads.</p></div><div class="input-specification"><p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of towns and roads.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the roads description. The <span class="tex-span"><i>i</i></span>-th from these lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the numbers of towns connected by the <span class="tex-span"><i>i</i></span>-th road and the length of the <span class="tex-span"><i>i</i></span>-th road. No road connects a town to itself, no two roads connect the same towns.</p><p><span class="tex-font-style-it">It's guaranteed that it's always possible to close down one of the roads so that all the towns are still reachable from each other.</span></p></div><div class="output-specification"><p>Print a single integer&nbsp;— the minimum possible inconvenience of the roads after the refusal from one of the roads.</p></div>

## Input

<p>The first line contains the integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>)&nbsp;— the number of towns and roads.</p><p>The next <span class="tex-span"><i>n</i></span> lines contain the roads description. The <span class="tex-span"><i>i</i></span>-th from these lines contains three integers <span class="tex-span"><i>u</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>v</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>l</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>u</i><sub class="lower-index"><i>i</i></sub>, <i>v</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>l</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— the numbers of towns connected by the <span class="tex-span"><i>i</i></span>-th road and the length of the <span class="tex-span"><i>i</i></span>-th road. No road connects a town to itself, no two roads connect the same towns.</p><p><span class="tex-font-style-it">It's guaranteed that it's always possible to close down one of the roads so that all the towns are still reachable from each other.</span></p>

## Output

<p>Print a single integer&nbsp;— the minimum possible inconvenience of the roads after the refusal from one of the roads.</p>





```input1
3
1 2 4
2 3 5
1 3 1

```




```input2
5
2 3 7
3 1 9
4 1 8
3 5 4
4 5 5

```




```output1
5

```




```output2
18

```


