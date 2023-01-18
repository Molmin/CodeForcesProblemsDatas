## Description

<div><p>There are <span class="tex-span"><i>n</i></span> workers in a company, each of them has a unique id from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. <span class="tex-font-style-bf">Exaclty</span> one of them is a chief, his id is <span class="tex-span"><i>s</i></span>. Each worker except the chief has exactly one immediate superior.</p><p>There was a request to each of the workers to tell how how many superiors (not only immediate). Worker's superiors are his immediate superior, the immediate superior of the his immediate superior, and so on. For example, if there are three workers in the company, from which the first is the chief, the second worker's immediate superior is the first, the third worker's immediate superior is the second, then the third worker has two superiors, one of them is immediate and one not immediate. The chief is a superior to all the workers except himself.</p><p>Some of the workers were in a hurry and made a mistake. You are to find the minimum number of workers that could make a mistake.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>)&nbsp;— the number of workers and the id of the chief.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of superiors (not only immediate) the worker with id <span class="tex-span"><i>i</i></span> reported about.</p></div><div class="output-specification"><p>Print the minimum number of workers that could make a mistake.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>, <span class="tex-span">1 ≤ <i>s</i> ≤ <i>n</i></span>)&nbsp;— the number of workers and the id of the chief.</p><p>The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ <i>n</i> - 1</span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of superiors (not only immediate) the worker with id <span class="tex-span"><i>i</i></span> reported about.</p>

## Output

<p>Print the minimum number of workers that could make a mistake.</p>





```input1
3 2
2 0 2

```




```input2
5 3
1 0 0 4 1

```




```output1
1

```




```output2
2

```



## Note

<p>In the first example it is possible that only the first worker made a mistake. Then: </p><ul> <li> the immediate superior of the first worker is the second worker, </li><li> the immediate superior of the third worker is the first worker, </li><li> the second worker is the chief. </li></ul>
