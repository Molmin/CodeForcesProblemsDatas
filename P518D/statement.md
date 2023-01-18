## Description

<div><p>Ilya got tired of sports programming, left university and got a job in the subway. He was given the task to determine the escalator load factor. </p><p>Let's assume that <span class="tex-span"><i>n</i></span> people stand in the queue for the escalator. At each second one of the two following possibilities takes place: either the first person in the queue enters the escalator with probability <span class="tex-span"><i>p</i></span>, or the first person in the queue doesn't move with probability <span class="tex-span">(1 - <i>p</i>)</span>, paralyzed by his fear of escalators and making the whole queue wait behind him.</p><p>Formally speaking, the <span class="tex-span"><i>i</i></span>-th person in the queue cannot enter the escalator until people with indices from <span class="tex-span">1</span> to <span class="tex-span"><i>i</i> - 1</span> inclusive enter it. In one second only one person can enter the escalator. The escalator is infinite, so if a person enters it, he never leaves it, that is he will be standing on the escalator at any following second. Ilya needs to count the expected value of the number of people standing on the escalator after <span class="tex-span"><i>t</i></span> seconds. </p><p>Your task is to help him solve this complicated task.</p></div><div class="input-specification"><p>The first line of the input contains three numbers <span class="tex-span"><i>n</i>, <i>p</i>, <i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>t</i> ≤ 2000</span>, <span class="tex-span">0 ≤ <i>p</i> ≤ 1</span>). Numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> are integers, number <span class="tex-span"><i>p</i></span> is real, given with exactly two digits after the decimal point.</p></div><div class="output-specification"><p>Print a single real number — the expected number of people who will be standing on the escalator after <span class="tex-span"><i>t</i></span> seconds. The absolute or relative error mustn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line of the input contains three numbers <span class="tex-span"><i>n</i>, <i>p</i>, <i>t</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>t</i> ≤ 2000</span>, <span class="tex-span">0 ≤ <i>p</i> ≤ 1</span>). Numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> are integers, number <span class="tex-span"><i>p</i></span> is real, given with exactly two digits after the decimal point.</p>

## Output

<p>Print a single real number — the expected number of people who will be standing on the escalator after <span class="tex-span"><i>t</i></span> seconds. The absolute or relative error mustn't exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
1 0.50 1

```




```input2
1 0.50 4

```




```input3
4 0.20 2

```




```output1
0.5

```




```output2
0.9375

```




```output3
0.4

```


