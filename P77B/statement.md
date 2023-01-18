## Description

<div><p>For some reason in many American cartoons anvils fall from time to time onto heroes' heads. Of course, safes, wardrobes, cruisers, planes fall sometimes too... But anvils do so most of all.</p><p>Anvils come in different sizes and shapes. Quite often they get the hero stuck deep in the ground. But have you ever thought who throws anvils from the sky? From what height? We are sure that such questions have never troubled you!</p><p>It turns out that throwing an anvil properly is not an easy task at all. Let's describe one of the most popular anvil throwing models.</p><p>Let the height <span class="tex-span"><i>p</i></span> of the potential victim vary in the range <span class="tex-span">[0;<i>a</i>]</span> and the direction of the wind <span class="tex-span"><i>q</i></span> vary in the range <span class="tex-span">[ - <i>b</i>;<i>b</i>]</span>. <span class="tex-span"><i>p</i></span> <span class="tex-font-style-bf">and</span> <span class="tex-span"><i>q</i></span> <span class="tex-font-style-bf">could be any real (floating) numbers.</span> Then we can assume that the anvil will fit the toon's head perfectly only if the following equation has at least one real root: </p><center> <img align="middle" class="tex-formula" src="file://JXdAvkr8.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>Determine the probability with which an aim can be successfully hit by an anvil.</p><p>You can assume that the <span class="tex-span"><i>p</i></span> and <span class="tex-span"><i>q</i></span> coefficients are chosen equiprobably and independently in their ranges.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10000</span>) — amount of testcases.</p><p>Each of the following <span class="tex-span"><i>t</i></span> lines contain two space-separated integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>Pretests contain all the tests with <span class="tex-span">0 &lt; <i>a</i> &lt; 10, 0 ≤ <i>b</i> &lt; 10</span>.</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>t</i></span> lines — the probability of a successful anvil hit for each testcase. The absolute or relative error of the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>t</i></span> (<span class="tex-span">1 ≤ <i>t</i> ≤ 10000</span>) — amount of testcases.</p><p>Each of the following <span class="tex-span"><i>t</i></span> lines contain two space-separated integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> (<span class="tex-span">0 ≤ <i>a</i>, <i>b</i> ≤ 10<sup class="upper-index">6</sup></span>).</p><p>Pretests contain all the tests with <span class="tex-span">0 &lt; <i>a</i> &lt; 10, 0 ≤ <i>b</i> &lt; 10</span>.</p>

## Output

<p>Print <span class="tex-span"><i>t</i></span> lines — the probability of a successful anvil hit for each testcase. The absolute or relative error of the answer should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
2
4 2
1 2

```




```output1
0.6250000000
0.5312500000

```


