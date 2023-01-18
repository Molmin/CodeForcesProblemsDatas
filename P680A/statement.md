## Description

<div><p>A little bear Limak plays a game. He has five cards. There is one number written on each card. Each number is a positive integer.</p><p>Limak can discard (throw out) some cards. His goal is to minimize the sum of numbers written on remaining (not discarded) cards.</p><p>He is allowed to <span class="tex-font-style-bf">at most once</span> discard two or three cards with the same number. Of course, he won't discard cards if it's impossible to choose two or three cards with the same number.</p><p>Given five numbers written on cards, cay you find the minimum sum of numbers on remaining cards?</p></div><div class="input-specification"><p>The only line of the input contains five integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">4</sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index">5</sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>)&nbsp;— numbers written on cards.</p></div><div class="output-specification"><p>Print the minimum possible sum of numbers written on remaining cards.</p></div>

## Input

<p>The only line of the input contains five integers <span class="tex-span"><i>t</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">2</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">3</sub></span>, <span class="tex-span"><i>t</i><sub class="lower-index">4</sub></span> and <span class="tex-span"><i>t</i><sub class="lower-index">5</sub></span> (<span class="tex-span">1 ≤ <i>t</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>)&nbsp;— numbers written on cards.</p>

## Output

<p>Print the minimum possible sum of numbers written on remaining cards.</p>





```input1
7 3 7 3 20

```




```input2
7 9 3 1 8

```




```input3
10 10 10 10 10

```




```output1
26

```




```output2
28

```




```output3
20

```



## Note

<p>In the first sample, Limak has cards with numbers <span class="tex-span">7</span>, <span class="tex-span">3</span>, <span class="tex-span">7</span>, <span class="tex-span">3</span> and <span class="tex-span">20</span>. Limak can do one of the following.</p><ul> <li> Do nothing and the sum would be <span class="tex-span">7 + 3 + 7 + 3 + 20 = 40</span>. </li><li> Remove two cards with a number <span class="tex-span">7</span>. The remaining sum would be <span class="tex-span">3 + 3 + 20 = 26</span>. </li><li> Remove two cards with a number <span class="tex-span">3</span>. The remaining sum would be <span class="tex-span">7 + 7 + 20 = 34</span>. </li></ul><p>You are asked to minimize the sum so the answer is <span class="tex-span">26</span>.</p><p>In the second sample, it's impossible to find two or three cards with the same number. Hence, Limak does nothing and the sum is <span class="tex-span">7 + 9 + 1 + 3 + 8 = 28</span>.</p><p>In the third sample, all cards have the same number. It's optimal to discard any three cards. The sum of two remaining numbers is <span class="tex-span">10 + 10 = 20</span>.</p>
