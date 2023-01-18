## Description

<div><p>You are playing a video game and you have just reached the bonus level, where the only possible goal is to score as many points as possible. Being a perfectionist, you've decided that you won't leave this level until you've gained the maximum possible number of points there.</p><p>The bonus level consists of <span class="tex-span"><i>n</i></span> small platforms placed in a line and numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right and (<span class="tex-span"><i>n</i> - 1</span>) bridges connecting adjacent platforms. The bridges between the platforms are very fragile, and for each bridge the number of times one can pass this bridge from one of its ends to the other before it collapses forever is known in advance.</p><p>The player's actions are as follows. First, he selects one of the platforms to be the starting position for his hero. After that the player can freely move the hero across the platforms moving by the undestroyed bridges. As soon as the hero finds himself on a platform with no undestroyed bridge attached to it, the level is automatically ended. The number of points scored by the player at the end of the level is calculated as the number of transitions made by the hero between the platforms. Note that if the hero started moving by a certain bridge, he has to continue moving in the same direction until he is on a platform.</p><p>Find how many points you need to score to be sure that nobody will beat your record, and move to the next level with a quiet heart.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of platforms on the bonus level. The second line contains (<span class="tex-span"><i>n</i> - 1</span>) integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>) — the number of transitions from one end to the other that the bridge between platforms <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> can bear.</p></div><div class="output-specification"><p>Print a single integer — the maximum number of points a player can get on the bonus level.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of platforms on the bonus level. The second line contains (<span class="tex-span"><i>n</i> - 1</span>) integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>, <span class="tex-span">1 ≤ <i>i</i> &lt; <i>n</i></span>) — the number of transitions from one end to the other that the bridge between platforms <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>i</i> + 1</span> can bear.</p>

## Output

<p>Print a single integer — the maximum number of points a player can get on the bonus level.</p><p>Please, do not use the <span class="tex-font-style-tt">%lld</span> specifier to read or write 64-bit integers in С++. It is preferred to use the <span class="tex-font-style-tt">cin</span>, <span class="tex-font-style-tt">cout</span> streams or the <span class="tex-font-style-tt">%I64d</span> specifier.</p>





```input1
5
2 1 2 1

```




```output1
5

```



## Note

<p>One possibility of getting <span class="tex-span">5</span> points in the sample is starting from platform <span class="tex-span">3</span> and consequently moving to platforms <span class="tex-span">4</span>, <span class="tex-span">3</span>, <span class="tex-span">2</span>, <span class="tex-span">1</span> and <span class="tex-span">2</span>. After that the only undestroyed bridge is the bridge between platforms <span class="tex-span">4</span> and <span class="tex-span">5</span>, but this bridge is too far from platform <span class="tex-span">2</span> where the hero is located now.</p>
