## Description

<div><p>Greg is a beginner bodybuilder. Today the gym coach gave him the training plan. All it had was <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span>. These numbers mean that Greg needs to do exactly <span class="tex-span"><i>n</i></span> exercises today. Besides, Greg should repeat the <span class="tex-span"><i>i</i></span>-th in order exercise <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> times.</p><p>Greg now only does three types of exercises: "chest" exercises, "biceps" exercises and "back" exercises. Besides, his training is cyclic, that is, the first exercise he does is a "chest" one, the second one is "biceps", the third one is "back", the fourth one is "chest", the fifth one is "biceps", and so on to the <span class="tex-span"><i>n</i></span>-th exercise.</p><p>Now Greg wonders, which muscle will get the most exercise during his training. We know that the exercise Greg repeats the maximum number of times, trains the corresponding muscle the most. Help Greg, determine which muscle will get the most training.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 20)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 25)</span> — the number of times Greg repeats the exercises.</p></div><div class="output-specification"><p>Print word "<span class="tex-font-style-tt">chest</span>" (without the quotes), if the chest gets the most exercise, "<span class="tex-font-style-tt">biceps</span>" (without the quotes), if the biceps gets the most exercise and print "<span class="tex-font-style-tt">back</span>" (without the quotes) if the back gets the most exercise.</p><p>It is guaranteed that the input is such that the answer to the problem is <span class="tex-font-style-bf">unambiguous</span>.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 20)</span>. The second line contains <span class="tex-span"><i>n</i></span> integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> <span class="tex-span">(1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 25)</span> — the number of times Greg repeats the exercises.</p>

## Output

<p>Print word "<span class="tex-font-style-tt">chest</span>" (without the quotes), if the chest gets the most exercise, "<span class="tex-font-style-tt">biceps</span>" (without the quotes), if the biceps gets the most exercise and print "<span class="tex-font-style-tt">back</span>" (without the quotes) if the back gets the most exercise.</p><p>It is guaranteed that the input is such that the answer to the problem is <span class="tex-font-style-bf">unambiguous</span>.</p>





```input1
2
2 8

```




```input2
3
5 1 10

```




```input3
7
3 3 2 7 9 6 8

```




```output1
biceps

```




```output2
back

```




```output3
chest

```



## Note

<p>In the first sample Greg does 2 chest, 8 biceps and zero back exercises, so the biceps gets the most exercises.</p><p>In the second sample Greg does 5 chest, 1 biceps and 10 back exercises, so the back gets the most exercises.</p><p>In the third sample Greg does 18 chest, 12 biceps and 8 back exercises, so the chest gets the most exercise.</p>
