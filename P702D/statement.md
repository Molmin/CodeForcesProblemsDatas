## Description

<div><p>Vasiliy has a car and he wants to get from home to the post office. The distance which he needs to pass equals to <span class="tex-span"><i>d</i></span> kilometers.</p><p>Vasiliy's car is not new — it breaks after driven every <span class="tex-span"><i>k</i></span> kilometers and Vasiliy needs <span class="tex-span"><i>t</i></span> seconds to repair it. After repairing his car Vasiliy can drive again (but after <span class="tex-span"><i>k</i></span> kilometers it will break again, and so on). In the beginning of the trip the car is just from repair station.</p><p>To drive one kilometer on car Vasiliy spends <span class="tex-span"><i>a</i></span> seconds, to walk one kilometer on foot he needs <span class="tex-span"><i>b</i></span> seconds (<span class="tex-span"><i>a</i> &lt; <i>b</i></span>).</p><p>Your task is to find minimal time after which Vasiliy will be able to reach the post office. Consider that in every moment of time Vasiliy can left his car and start to go on foot.</p></div><div class="input-specification"><p>The first line contains 5 positive integers <span class="tex-span"><i>d</i>, <i>k</i>, <i>a</i>, <i>b</i>, <i>t</i></span> (<span class="tex-span">1 ≤ <i>d</i> ≤ 10<sup class="upper-index">12</sup></span>; <span class="tex-span">1 ≤ <i>k</i>, <i>a</i>, <i>b</i>, <i>t</i> ≤ 10<sup class="upper-index">6</sup></span>; <span class="tex-span"><i>a</i> &lt; <i>b</i></span>), where:</p><ul> <li> <span class="tex-span"><i>d</i></span> — the distance from home to the post office; </li><li> <span class="tex-span"><i>k</i></span> — the distance, which car is able to drive before breaking; </li><li> <span class="tex-span"><i>a</i></span> — the time, which Vasiliy spends to drive 1 kilometer on his car; </li><li> <span class="tex-span"><i>b</i></span> — the time, which Vasiliy spends to walk 1 kilometer on foot; </li><li> <span class="tex-span"><i>t</i></span> — the time, which Vasiliy spends to repair his car. </li></ul></div><div class="output-specification"><p>Print the minimal time after which Vasiliy will be able to reach the post office.</p></div>

## Input

<p>The first line contains 5 positive integers <span class="tex-span"><i>d</i>, <i>k</i>, <i>a</i>, <i>b</i>, <i>t</i></span> (<span class="tex-span">1 ≤ <i>d</i> ≤ 10<sup class="upper-index">12</sup></span>; <span class="tex-span">1 ≤ <i>k</i>, <i>a</i>, <i>b</i>, <i>t</i> ≤ 10<sup class="upper-index">6</sup></span>; <span class="tex-span"><i>a</i> &lt; <i>b</i></span>), where:</p><ul> <li> <span class="tex-span"><i>d</i></span> — the distance from home to the post office; </li><li> <span class="tex-span"><i>k</i></span> — the distance, which car is able to drive before breaking; </li><li> <span class="tex-span"><i>a</i></span> — the time, which Vasiliy spends to drive 1 kilometer on his car; </li><li> <span class="tex-span"><i>b</i></span> — the time, which Vasiliy spends to walk 1 kilometer on foot; </li><li> <span class="tex-span"><i>t</i></span> — the time, which Vasiliy spends to repair his car. </li></ul>

## Output

<p>Print the minimal time after which Vasiliy will be able to reach the post office.</p>





```input1
5 2 1 4 10

```




```input2
5 2 1 4 5

```




```output1
14

```




```output2
13

```



## Note

<p>In the first example Vasiliy needs to drive the first 2 kilometers on the car (in 2 seconds) and then to walk on foot 3 kilometers (in 12 seconds). So the answer equals to 14 seconds.</p><p>In the second example Vasiliy needs to drive the first 2 kilometers on the car (in 2 seconds), then repair his car (in 5 seconds) and drive 2 kilometers more on the car (in 2 seconds). After that he needs to walk on foot 1 kilometer (in 4 seconds). So the answer equals to 13 seconds.</p>
