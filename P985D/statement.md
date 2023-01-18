## Description

<div><p>You are going to the beach with the idea to build the greatest sand castle ever in your head! The beach is not as three-dimensional as you could have imagined, it can be decribed as a line of spots to pile up sand pillars. Spots are numbered <span class="tex-span">1</span> through infinity from left to right. </p><p>Obviously, there is not enough sand on the beach, so you brought <span class="tex-span"><i>n</i></span> packs of sand with you. Let height <span class="tex-span"><i>h</i><sub class="lower-index"><i>i</i></sub></span> of the sand pillar on some spot <span class="tex-span"><i>i</i></span> be the number of sand packs you spent on it. <span class="tex-font-style-bf">You can't split a sand pack to multiple pillars, all the sand from it should go to a single one.</span> There is a fence of height equal to the height of pillar with <span class="tex-span"><i>H</i></span> sand packs to the left of the first spot and you should prevent sand from going over it. </p><p>Finally you ended up with the following conditions to building the castle:</p><ul> <li> <span class="tex-span"><i>h</i><sub class="lower-index">1</sub> ≤ <i>H</i></span>: no sand from the leftmost spot should go over the fence; </li><li> For any <img align="middle" class="tex-formula" src="file://crPZFBet.png" style="max-width: 100.0%;max-height: 100.0%;"> <span class="tex-span">|<i>h</i><sub class="lower-index"><i>i</i></sub> - <i>h</i><sub class="lower-index"><i>i</i> + 1</sub>| ≤ 1</span>: large difference in heights of two neighboring pillars can lead sand to fall down from the higher one to the lower, you really don't want this to happen; </li><li> <img align="middle" class="tex-formula" src="file://4eVXonSv.png" style="max-width: 100.0%;max-height: 100.0%;">: you want to spend all the sand you brought with you. </li></ul><p>As you have infinite spots to build, it is always possible to come up with some valid castle structure. Though you want the castle to be as compact as possible. </p><p>Your task is to calculate the minimum number of spots you can occupy so that all the aforementioned conditions hold.</p></div><div class="input-specification"><p>The only line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>H</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>H</i> ≤ 10<sup class="upper-index">18</sup></span>) — the number of sand packs you have and the height of the fence, respectively.</p></div><div class="output-specification"><p>Print the minimum number of spots you can occupy so the all the castle building conditions hold.</p></div>

## Input

<p>The only line contains two integer numbers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>H</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>H</i> ≤ 10<sup class="upper-index">18</sup></span>) — the number of sand packs you have and the height of the fence, respectively.</p>

## Output

<p>Print the minimum number of spots you can occupy so the all the castle building conditions hold.</p>





```input1
5 2

```




```input2
6 8

```




```output1
3

```




```output2
3

```



## Note

<p>Here are the heights of some valid castles: </p><ul> <li> <span class="tex-span"><i>n</i> = 5, <i>H</i> = 2, [2, 2, 1, 0, ...], [2, 1, 1, 1, 0, ...], [1, 0, 1, 2, 1, 0, ...]</span> </li><li> <span class="tex-span"><i>n</i> = 6, <i>H</i> = 8, [3, 2, 1, 0, ...], [2, 2, 1, 1, 0, ...], [0, 1, 0, 1, 2, 1, 1, 0...]</span> (this one has <span class="tex-span">5</span> spots occupied) </li></ul><p>The first list for both cases is the optimal answer, <span class="tex-span">3</span> spots are occupied in them.</p><p>And here are some invalid ones:</p><ul> <li> <span class="tex-span"><i>n</i> = 5, <i>H</i> = 2, [3, 2, 0, ...], [2, 3, 0, ...], [1, 0, 2, 2, ...]</span> </li><li> <span class="tex-span"><i>n</i> = 6, <i>H</i> = 8, [2, 2, 2, 0, ...], [6, 0, ...], [1, 4, 1, 0...], [2, 2, 1, 0, ...]</span> </li></ul>
