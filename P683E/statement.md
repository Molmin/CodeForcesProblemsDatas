## Description

<div><p><span class="tex-span"><i>n</i></span> athletes take part in the hammer throw. Each of them has his own unique identifier — the integer from 1 to <span class="tex-span"><i>n</i></span> (all athletes have distinct identifiers). After the draw, the order in which the athletes will throw the hammer has been determined (they will do it one by one).</p><p>Unfortunately, a not very attentive judge lost the list with the order of athletes, but each of the athletes has remembered how many competitors with identifiers larger than his own will throw the hammer before him.</p><p>Your task is to help the organizers as quickly as possible to restore the order of the athletes.</p></div><div class="input-specification"><p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of athletes.</p><p>The next line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the number of the athletes with identifiers larger than <span class="tex-span"><i>i</i></span>, who should throw the hammer before the athlete with identifier <span class="tex-span"><i>i</i></span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> distinct numbers — the sequence of athletes' identifiers in the order in which they will throw the hammer. If there are several answers it is allowed to print any of them. </p></div>

## Input

<p>The first line contains the positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>) — the number of athletes.</p><p>The next line contains the sequence of integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> &lt; <i>n</i></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is equal to the number of the athletes with identifiers larger than <span class="tex-span"><i>i</i></span>, who should throw the hammer before the athlete with identifier <span class="tex-span"><i>i</i></span>.</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> distinct numbers — the sequence of athletes' identifiers in the order in which they will throw the hammer. If there are several answers it is allowed to print any of them. </p>





```input1
4
2 0 1 0

```




```input2
6
2 2 0 1 1 0

```




```output1
2 4 1 3 

```




```output2
3 6 1 2 4 5 

```


