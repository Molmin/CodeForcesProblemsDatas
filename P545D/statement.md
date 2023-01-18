## Description

<div><p>Little girl Susie went shopping with her mom and she wondered how to improve service quality. </p><p>There are <span class="tex-span"><i>n</i></span> people in the queue. For each person we know time <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> needed to serve him. A person will be disappointed if the time he waits is more than the time needed to serve him. The time a person waits is the total time when all the people who stand in the queue in front of him are served. Susie thought that if we swap some people in the queue, then we can decrease the number of people who are disappointed. </p><p>Help Susie find out what is the maximum number of not disappointed people can be achieved by swapping people in the queue.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), separated by spaces.</p></div><div class="output-specification"><p>Print a single number — the maximum number of not disappointed people in the queue.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The next line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>t</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), separated by spaces.</p>

## Output

<p>Print a single number — the maximum number of not disappointed people in the queue.</p>





```input1
5
15 2 1 5 3

```




```output1
4

```



## Note

<p>Value <span class="tex-span">4</span> is achieved at such an arrangement, for example: <span class="tex-span">1, 2, 3, 5, 15</span>. Thus, you can make everything feel not disappointed except for the person with time 5.</p>
