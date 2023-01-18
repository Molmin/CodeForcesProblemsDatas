## Description

<div><p>Vasya is about to take his first university exam in about several minutes. And it's not just some ordinary exam, it's on mathematical analysis. Of course, right now Vasya can only think of one thing: what the result of his talk with the examiner will be...</p><p>To prepare for the exam, one has to study proofs of <span class="tex-span"><i>n</i></span> theorems. It is known that there will be <span class="tex-span"><i>k</i></span> examination cards on the exam and each card contains <img align="middle" class="tex-formula" src="file://k8XO99N2.png" style="max-width: 100.0%;max-height: 100.0%;"> distinct theorems. Besides, no theorem is mentioned in more than one card (that is, <img align="middle" class="tex-formula" src="file://8i5rMhCf.png" style="max-width: 100.0%;max-height: 100.0%;"> theorems won't be mentioned in any card). During the exam several students may get the same card.</p><p>We do not know the exact way theorems are distributed by cards, however the students that took the exam before Vasya told him what theorems their cards contained. Vasya evaluates his <span class="tex-font-style-underline">level of proficiency in the <span class="tex-span"><i>i</i></span>-th theorem</span> by some number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>. <span class="tex-font-style-underline">The level of proficiency in some card</span> is the average of the levels of proficiency in the theorems that are included in the card. Now Vasya wants to know the minimally and maximally possible levels of his proficiency in the card he gets on the exam. Vasya wants to determine it by the data he has collected from other students. Unfortunately, Vasya has no time left to do the math and he asked you to help him.</p></div><div class="input-specification"><p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100</span>) — the number of theorems and the number of cards correspondingly. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), the <span class="tex-span"><i>i</i></span>-th number (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) corresponds to Vasya's proficiency in the <span class="tex-span"><i>i</i></span>-th theorem.</p><p>The third line contains number <span class="tex-span"><i>q</i></span> (<span class="tex-span">0 ≤ <i>q</i> ≤ 100</span>) — the number of people that have taken the exam before Vasya. Each of the following <span class="tex-span"><i>q</i></span> lines contains the description of a student's card: <img align="middle" class="tex-formula" src="file://z353tjjp.png" style="max-width: 100.0%;max-height: 100.0%;"> integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> inclusive. They are the numbers of theorems included in the card in the order in which they are enumerated in the input data. The numbers are given in an arbitrary order. It is guaranteed that the given cards are valid (that is, that all theorems in one card are different and that different people get cards that either don't contain the same theorems or coincide up to the theorems' permutation).</p></div><div class="output-specification"><p>Print two real numbers, representing Vasya's minimum and maximum proficiency in the card he will get on the exam. The absolute or relative error should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i> ≤ 100</span>) — the number of theorems and the number of cards correspondingly. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>), the <span class="tex-span"><i>i</i></span>-th number (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>) corresponds to Vasya's proficiency in the <span class="tex-span"><i>i</i></span>-th theorem.</p><p>The third line contains number <span class="tex-span"><i>q</i></span> (<span class="tex-span">0 ≤ <i>q</i> ≤ 100</span>) — the number of people that have taken the exam before Vasya. Each of the following <span class="tex-span"><i>q</i></span> lines contains the description of a student's card: <img align="middle" class="tex-formula" src="file://z353tjjp.png" style="max-width: 100.0%;max-height: 100.0%;"> integers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> inclusive. They are the numbers of theorems included in the card in the order in which they are enumerated in the input data. The numbers are given in an arbitrary order. It is guaranteed that the given cards are valid (that is, that all theorems in one card are different and that different people get cards that either don't contain the same theorems or coincide up to the theorems' permutation).</p>

## Output

<p>Print two real numbers, representing Vasya's minimum and maximum proficiency in the card he will get on the exam. The absolute or relative error should not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
7 3
7 15 0 19 10 5 12
2
1 6
7 4

```




```input2
4 2
10 8 1 17
2
2 3
3 2

```




```output1
5.0000000000 15.5000000000
```




```output2
4.5000000000 13.5000000000
```



## Note

<p>Let's analyze the first sample. Vasya's proficiency in the cards whose content he already knows equals <span class="tex-span">6</span> and <span class="tex-span">15.5</span> correspondingly. The three theorems that are left are only enough to make one exam card. If we consider all possible variants of theorems included in the card we can see that in the best case scenario Vasya gets the card that contains theorems <span class="tex-span">4</span> and <span class="tex-span">7</span> (his proficiency would equal <span class="tex-span">15.5</span>) and in the worst case scenario he gets theorems <span class="tex-span">3</span> and <span class="tex-span">5</span> (his proficiency would equal <span class="tex-span">5</span>).</p><p>The <span class="tex-span">⌊ <i>x</i>⌋</span> operation denotes taking integer part of real number <span class="tex-span"><i>x</i></span> (rounding down).</p>
