## Description

<div><p>A factory produces thimbles in bulk. Typically, it can produce up to <span class="tex-span"><i>a</i></span> thimbles a day. However, some of the machinery is defective, so it can currently only produce <span class="tex-span"><i>b</i></span> thimbles each day. The factory intends to choose a <span class="tex-span"><i>k</i></span>-day period to do maintenance and construction; it cannot produce any thimbles during this time, but will be restored to its full production of <span class="tex-span"><i>a</i></span> thimbles per day after the <span class="tex-span"><i>k</i></span> days are complete.</p><p>Initially, no orders are pending. The factory receives updates of the form <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, indicating that <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> new orders have been placed for the <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>-th day. Each order requires a single thimble to be produced on precisely the specified day. The factory may opt to fill as many or as few of the orders in a single batch as it likes.</p><p>As orders come in, the factory owner would like to know the maximum number of orders he will be able to fill if he starts repairs on a given day <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>. Help the owner answer his questions.</p></div><div class="input-specification"><p>The first line contains five integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>b</i> &lt; <i>a</i> ≤ 10 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>)&nbsp;— the number of days, the length of the repair time, the production rates of the factory, and the number of updates, respectively.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the descriptions of the queries. Each query is of one of the following two forms: </p><ul> <li> <span class="tex-span">1 <i>d</i><sub class="lower-index"><i>i</i></sub> <i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>), representing an update of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> orders on day <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, or </li><li> <span class="tex-span">2 <i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - <i>k</i> + 1</span>), representing a question: at the moment, how many orders could be filled if the factory decided to commence repairs on day <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>? </li></ul><p>It's guaranteed that the input will contain at least one query of the second type.</p></div><div class="output-specification"><p>For each query of the second type, print a line containing a single integer — the maximum number of orders that the factory can fill over all <span class="tex-span"><i>n</i></span> days.</p></div>

## Input

<p>The first line contains five integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span>, and <span class="tex-span"><i>q</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 200 000</span>, <span class="tex-span">1 ≤ <i>b</i> &lt; <i>a</i> ≤ 10 000</span>, <span class="tex-span">1 ≤ <i>q</i> ≤ 200 000</span>)&nbsp;— the number of days, the length of the repair time, the production rates of the factory, and the number of updates, respectively.</p><p>The next <span class="tex-span"><i>q</i></span> lines contain the descriptions of the queries. Each query is of one of the following two forms: </p><ul> <li> <span class="tex-span">1 <i>d</i><sub class="lower-index"><i>i</i></sub> <i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>d</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i></span>, <span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10 000</span>), representing an update of <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> orders on day <span class="tex-span"><i>d</i><sub class="lower-index"><i>i</i></sub></span>, or </li><li> <span class="tex-span">2 <i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - <i>k</i> + 1</span>), representing a question: at the moment, how many orders could be filled if the factory decided to commence repairs on day <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span>? </li></ul><p>It's guaranteed that the input will contain at least one query of the second type.</p>

## Output

<p>For each query of the second type, print a line containing a single integer — the maximum number of orders that the factory can fill over all <span class="tex-span"><i>n</i></span> days.</p>





```input1
5 2 2 1 8
1 1 2
1 5 3
1 2 1
2 2
1 4 2
1 3 2
2 1
2 3

```




```input2
5 4 10 1 6
1 1 5
1 5 5
1 3 2
1 5 2
2 1
2 2

```




```output1
3
6
4

```




```output2
7
1

```



## Note

<p>Consider the first sample.</p><p>We produce up to <span class="tex-span">1</span> thimble a day currently and will produce up to <span class="tex-span">2</span> thimbles a day after repairs. Repairs take <span class="tex-span">2</span> days.</p><p>For the first question, we are able to fill <span class="tex-span">1</span> order on day <span class="tex-span">1</span>, no orders on days <span class="tex-span">2</span> and <span class="tex-span">3</span> since we are repairing, no orders on day <span class="tex-span">4</span> since no thimbles have been ordered for that day, and <span class="tex-span">2</span> orders for day <span class="tex-span">5</span> since we are limited to our production capacity, for a total of <span class="tex-span">3</span> orders filled.</p><p>For the third question, we are able to fill <span class="tex-span">1</span> order on day <span class="tex-span">1</span>, <span class="tex-span">1</span> order on day <span class="tex-span">2</span>, and <span class="tex-span">2</span> orders on day <span class="tex-span">5</span>, for a total of <span class="tex-span">4</span> orders.</p>
