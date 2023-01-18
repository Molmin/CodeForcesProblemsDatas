## Description

<div><p>Andrey needs one more problem to conduct a programming contest. He has <span class="tex-span"><i>n</i></span> friends who are always willing to help. He can ask some of them to come up with a contest problem. Andrey knows one value for each of his fiends — the probability that this friend will come up with a problem if Andrey asks him.</p><p>Help Andrey choose people to ask. As he needs only one problem, Andrey is going to be really upset if no one comes up with a problem or if he gets more than one problem from his friends. You need to choose such a set of people that maximizes the chances of Andrey not getting upset.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of Andrey's friends. The second line contains <span class="tex-span"><i>n</i></span> real numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0.0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1.0)</span> — the probability that the <span class="tex-span"><i>i</i></span>-th friend can come up with a problem. The probabilities are given with at most 6 digits after decimal point.</p></div><div class="output-specification"><p>Print a single real number — the probability that Andrey won't get upset at the optimal choice of friends. The answer will be considered valid if it differs from the correct one by at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 100)</span> — the number of Andrey's friends. The second line contains <span class="tex-span"><i>n</i></span> real numbers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span">(0.0 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ 1.0)</span> — the probability that the <span class="tex-span"><i>i</i></span>-th friend can come up with a problem. The probabilities are given with at most 6 digits after decimal point.</p>

## Output

<p>Print a single real number — the probability that Andrey won't get upset at the optimal choice of friends. The answer will be considered valid if it differs from the correct one by at most <span class="tex-span">10<sup class="upper-index"> - 9</sup></span>.</p>





```input1
4
0.1 0.2 0.3 0.8

```




```input2
2
0.1 0.2

```




```output1
0.800000000000

```




```output2
0.260000000000

```



## Note

<p>In the first sample the best strategy for Andrey is to ask only one of his friends, the most reliable one.</p><p>In the second sample the best strategy for Andrey is to ask all of his friends to come up with a problem. Then the probability that he will get exactly one problem is <span class="tex-span">0.1·0.8 + 0.9·0.2 = 0.26</span>.</p>
