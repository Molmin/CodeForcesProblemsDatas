## Description

<div><p>Limak is an old brown bear. He often goes bowling with his friends. Today he feels really good and tries to beat his own record!</p><p>For rolling a ball one gets a score — an integer (maybe negative) number of points. Score for <span class="tex-span"><i>i</i></span>-th roll is multiplied by <span class="tex-span"><i>i</i></span> and scores are summed up. So, for <span class="tex-span"><i>k</i></span> rolls with scores <span class="tex-span"><i>s</i><sub class="lower-index">1</sub>, <i>s</i><sub class="lower-index">2</sub>, ..., <i>s</i><sub class="lower-index"><i>k</i></sub></span>, total score is <img align="middle" class="tex-formula" src="file://97WzQTei.png" style="max-width: 100.0%;max-height: 100.0%;">. Total score is <span class="tex-span">0</span> if there were no rolls.</p><p>Limak made <span class="tex-span"><i>n</i></span> rolls and got score <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> for <span class="tex-span"><i>i</i></span>-th of them. He wants to maximize his total score and he came up with an interesting idea. He will cancel some rolls, saying that something distracted him or there was a strong wind.</p><p>Limak is able to cancel any number of rolls, maybe even all or none of them. Total score is calculated as if there were only non-canceled rolls. Look at the sample tests for clarification. What maximum total score can Limak get?</p></div><div class="input-specification"><p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">7</sup>)</span> - scores for Limak's rolls.</p></div><div class="output-specification"><p>Print the maximum possible total score after choosing rolls to cancel.</p></div>

## Input

<p>The first line contains single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>).</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">|<i>a</i><sub class="lower-index"><i>i</i></sub>| ≤ 10<sup class="upper-index">7</sup>)</span> - scores for Limak's rolls.</p>

## Output

<p>Print the maximum possible total score after choosing rolls to cancel.</p>





```input1
5
-2 -8 0 5 -3

```




```input2
6
-10 20 -30 40 -50 60

```




```output1
13

```




```output2
400

```



## Note

<p>In first sample Limak should cancel rolls with scores <span class="tex-span"> - 8</span> and <span class="tex-span"> - 3</span>. Then he is left with three rolls with scores <span class="tex-span"> - 2, 0, 5</span>. Total score is <span class="tex-span">1·( - 2) + 2·0 + 3·5 = 13</span>.</p><p>In second sample Limak should cancel roll with score <span class="tex-span"> - 50</span>. Total score is <span class="tex-span">1·( - 10) + 2·20 + 3·( - 30) + 4·40 + 5·60 = 400</span>.</p>
