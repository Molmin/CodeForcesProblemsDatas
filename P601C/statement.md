## Description

<div><p>Kleofáš is participating in an <span class="tex-span"><i>n</i></span>-thlon - a tournament consisting of <span class="tex-span"><i>n</i></span> different competitions in <span class="tex-span"><i>n</i></span> different disciplines (numbered <span class="tex-span">1</span> through <span class="tex-span"><i>n</i></span>). There are <span class="tex-span"><i>m</i></span> participants in the <span class="tex-span"><i>n</i></span>-thlon and each of them participates in all competitions.</p><p>In each of these <span class="tex-span"><i>n</i></span> competitions, the participants are given <span class="tex-font-style-underline">ranks</span> from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span> in such a way that no two participants are given the same rank - in other words, the ranks in each competition form a permutation of numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>m</i></span>. The <span class="tex-font-style-underline">score</span> of a participant in a competition is equal to his/her rank in it.</p><p>The <span class="tex-font-style-underline">overall score</span> of each participant is computed as the sum of that participant's scores in all competitions.</p><p>The <span class="tex-font-style-underline">overall rank</span> of each participant is equal to <span class="tex-span">1 + <i>k</i></span>, where <span class="tex-span"><i>k</i></span> is the number of participants with <span class="tex-font-style-bf">strictly smaller</span> overall score.</p><p>The <span class="tex-span"><i>n</i></span>-thlon is over now, but the results haven't been published yet. Kleofáš still remembers his ranks in each particular competition; however, he doesn't remember anything about how well the other participants did. Therefore, Kleofáš would like to know his expected overall rank.</p><p>All competitors are equally good at each discipline, so all rankings (permutations of ranks of everyone except Kleofáš) in each competition are equiprobable.</p></div><div class="input-specification"><p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>)&nbsp;— the number of competitions and the number of participants respectively.</p><p>Then, <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains one integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— the rank of Kleofáš in the <span class="tex-span"><i>i</i></span>-th competition.</p></div><div class="output-specification"><p>Output a single real number – the expected overall rank of Kleofáš. Your answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://sVwbFa4M.png" style="max-width: 100.0%;max-height: 100.0%;">.</p></div>

## Input

<p>The first line of the input contains two space-separated integers <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 1000</span>)&nbsp;— the number of competitions and the number of participants respectively.</p><p>Then, <span class="tex-span"><i>n</i></span> lines follow. The <span class="tex-span"><i>i</i></span>-th of them contains one integer <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>x</i><sub class="lower-index"><i>i</i></sub> ≤ <i>m</i></span>)&nbsp;— the rank of Kleofáš in the <span class="tex-span"><i>i</i></span>-th competition.</p>

## Output

<p>Output a single real number – the expected overall rank of Kleofáš. Your answer will be considered correct if its relative or absolute error doesn't exceed <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p><p>Namely: let's assume that your answer is <span class="tex-span"><i>a</i></span>, and the answer of the jury is <span class="tex-span"><i>b</i></span>. The checker program will consider your answer correct, if <img align="middle" class="tex-formula" src="file://sVwbFa4M.png" style="max-width: 100.0%;max-height: 100.0%;">.</p>





```input1
4 10
2
1
2
1

```




```input2
5 5
1
2
3
4
5

```




```input3
3 6
2
4
2

```




```output1
1.0000000000000000

```




```output2
2.7500000000000000

```




```output3
1.6799999999999999

```



## Note

<p>In the first sample, Kleofáš has overall score <span class="tex-span">6</span>. Nobody else can have overall score less than <span class="tex-span">6</span> (but it's possible for one other person to have overall score <span class="tex-span">6</span> as well), so his overall rank must be <span class="tex-span">1</span>.</p>
