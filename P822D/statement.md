## Description

<div><p>In Pavlopolis University where Noora studies it was decided to hold beauty contest "Miss Pavlopolis University". Let's describe the process of choosing the most beautiful girl in the university in more detail.</p><p>The contest is held in several stages. Suppose that exactly <span class="tex-span"><i>n</i></span> girls participate in the competition initially. All the participants are divided into equal groups, <span class="tex-span"><i>x</i></span> participants in each group. Furthermore the number <span class="tex-span"><i>x</i></span> is chosen arbitrarily, i. e. on every stage number <span class="tex-span"><i>x</i></span> can be different. Within each group the jury of the contest compares beauty of the girls in the format "each with each". In this way, if group consists of <span class="tex-span"><i>x</i></span> girls, then <img align="middle" class="tex-formula" src="file://uW2EvDWf.png" style="max-width: 100.0%;max-height: 100.0%;"> comparisons occur. Then, from each group, the most beautiful participant is selected. Selected girls enter the next stage of the competition. Thus if <span class="tex-span"><i>n</i></span> girls were divided into groups, <span class="tex-span"><i>x</i></span> participants in each group, then exactly <img align="middle" class="tex-formula" src="file://Zycpp1Li.png" style="max-width: 100.0%;max-height: 100.0%;"> participants will enter the next stage. The contest continues until there is exactly one girl left who will be "Miss Pavlopolis University"</p><p>But for the jury this contest is a very tedious task. They would like to divide the girls into groups in each stage so that the total number of pairwise comparisons of the girls is as few as possible. Let <span class="tex-span"><i>f</i>(<i>n</i>)</span> be the minimal total number of comparisons that should be made to select the most beautiful participant, if we admit <span class="tex-span"><i>n</i></span> girls to the first stage.</p><p>The organizers of the competition are insane. They give Noora three integers <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> and ask the poor girl to calculate the value of the following expression: <span class="tex-span"><i>t</i><sup class="upper-index">0</sup>·<i>f</i>(<i>l</i>) + <i>t</i><sup class="upper-index">1</sup>·<i>f</i>(<i>l</i> + 1) + ... + <i>t</i><sup class="upper-index"><i>r</i> - <i>l</i></sup>·<i>f</i>(<i>r</i>)</span>. However, since the value of this expression can be quite large the organizers ask her to calculate it modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>. If Noora can calculate the value of this expression the organizers promise her to help during the beauty contest. But the poor girl is not strong in mathematics, so she turned for help to Leha and he turned to you.</p></div><div class="input-specification"><p>The first and single line contains three integers <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>t</i> &lt; 10<sup class="upper-index">9</sup> + 7, 2 ≤ <i>l</i> ≤ <i>r</i> ≤ 5·10<sup class="upper-index">6</sup></span>).</p></div><div class="output-specification"><p>In the first line print single integer — the value of the expression modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first and single line contains three integers <span class="tex-span"><i>t</i></span>, <span class="tex-span"><i>l</i></span> and <span class="tex-span"><i>r</i></span> (<span class="tex-span">1 ≤ <i>t</i> &lt; 10<sup class="upper-index">9</sup> + 7, 2 ≤ <i>l</i> ≤ <i>r</i> ≤ 5·10<sup class="upper-index">6</sup></span>).</p>

## Output

<p>In the first line print single integer — the value of the expression modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
2 2 4

```




```output1
19

```



## Note

<p>Consider the sample.</p><p>It is necessary to find the value of <img align="middle" class="tex-formula" src="file://6qyYjmdI.png" style="max-width: 100.0%;max-height: 100.0%;">.</p><p><span class="tex-span"><i>f</i>(2) = 1</span>. From two girls you can form only one group of two people, in which there will be one comparison.</p><p><span class="tex-span"><i>f</i>(3) = 3</span>. From three girls you can form only one group of three people, in which there will be three comparisons.</p><p><span class="tex-span"><i>f</i>(4) = 3</span>. From four girls you can form two groups of two girls each. Then at the first stage there will be two comparisons, one in each of the two groups. In the second stage there will be two girls and there will be one comparison between them. Total <span class="tex-span">2 + 1 = 3</span> comparisons. You can also leave all girls in same group in the first stage. Then <img align="middle" class="tex-formula" src="file://161b2q8b.png" style="max-width: 100.0%;max-height: 100.0%;"> comparisons will occur. Obviously, it's better to split girls into groups in the first way.</p><p>Then the value of the expression is <img align="middle" class="tex-formula" src="file://OhX8Nbm2.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>
