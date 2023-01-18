## Description

<div><p>One must train much to do well on wizardry contests. So, there are numerous wizardry schools and magic fees.</p><p>One of such magic schools consists of <span class="tex-span"><i>n</i></span> tours. A winner of each tour gets a huge prize. The school is organised quite far away, so one will have to take all the prizes home in one go. And the bags that you've brought with you have space for no more than <span class="tex-span"><i>k</i></span> huge prizes.</p><p>Besides the fact that you want to take all the prizes home, you also want to perform well. You will consider your performance good if you win at least <span class="tex-span"><i>l</i></span> tours.</p><p>In fact, years of organizing contests proved to the organizers that transporting huge prizes is an issue for the participants. Alas, no one has ever invented a spell that would shrink the prizes... So, here's the solution: for some tours the winner gets a bag instead of a huge prize. Each bag is characterized by number <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> — the number of huge prizes that will fit into it.</p><p>You already know the subject of all tours, so you can estimate the probability <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> of winning the <span class="tex-span"><i>i</i></span>-th tour. You cannot skip the tour under any circumstances.</p><p>Find the probability that you will perform well on the contest and will be able to take all won prizes home (that is, that you will be able to fit all the huge prizes that you won into the bags that you either won or brought from home).</p></div><div class="input-specification"><p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200, 0 ≤ <i>l</i>, <i>k</i> ≤ 200</span>) — the number of tours, the minimum number of tours to win, and the number of prizes that you can fit in the bags brought from home, correspondingly.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the probability to win the <span class="tex-span"><i>i</i></span>-th tour, in percents.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 200</span>) — the capacity of the bag that will be awarded to you for winning the <span class="tex-span"><i>i</i></span>-th tour, or else -1, if the prize for the <span class="tex-span"><i>i</i></span>-th tour is a huge prize and not a bag.</p></div><div class="output-specification"><p>Print a single real number — the answer to the problem. The answer will be accepted if the absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p></div>

## Input

<p>The first line contains three integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>l</i></span>, <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200, 0 ≤ <i>l</i>, <i>k</i> ≤ 200</span>) — the number of tours, the minimum number of tours to win, and the number of prizes that you can fit in the bags brought from home, correspondingly.</p><p>The second line contains <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 100</span>) — the probability to win the <span class="tex-span"><i>i</i></span>-th tour, in percents.</p><p>The third line contains <span class="tex-span"><i>n</i></span> space-separated integers, <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 200</span>) — the capacity of the bag that will be awarded to you for winning the <span class="tex-span"><i>i</i></span>-th tour, or else -1, if the prize for the <span class="tex-span"><i>i</i></span>-th tour is a huge prize and not a bag.</p>

## Output

<p>Print a single real number — the answer to the problem. The answer will be accepted if the absolute or relative error does not exceed <span class="tex-span">10<sup class="upper-index"> - 6</sup></span>.</p>





```input1
3 1 0
10 20 30
-1 -1 2

```




```input2
1 1 1
100
123

```




```output1
0.300000000000

```




```output2
1.000000000000

```



## Note

<p>In the first sample we need either win no tour or win the third one. If we win nothing we wouldn't perform well. So, we must to win the third tour. Other conditions will be satisfied in this case. Probability of wining the third tour is 0.3.</p><p>In the second sample we win the only tour with probability 1.0, and go back home with bag for it.</p>
