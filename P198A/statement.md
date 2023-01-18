## Description

<div><p>Qwerty the Ranger took up a government job and arrived on planet Mars. He should stay in the secret lab and conduct some experiments on bacteria that have funny and abnormal properties. The job isn't difficult, but the salary is high.</p><p>At the beginning of the first experiment there is a single bacterium in the test tube. Every second each bacterium in the test tube divides itself into <span class="tex-span"><i>k</i></span> bacteria. After that some abnormal effects create <span class="tex-span"><i>b</i></span> more bacteria in the test tube. Thus, if at the beginning of some second the test tube had <span class="tex-span"><i>x</i></span> bacteria, then at the end of the second it will have <span class="tex-span"><i>kx</i> + <i>b</i></span> bacteria.</p><p>The experiment showed that after <span class="tex-span"><i>n</i></span> seconds there were exactly <span class="tex-span"><i>z</i></span> bacteria and the experiment ended at this point.</p><p>For the second experiment Qwerty is going to sterilize the test tube and put there <span class="tex-span"><i>t</i></span> bacteria. He hasn't started the experiment yet but he already wonders, how many seconds he will need to grow at least <span class="tex-span"><i>z</i></span> bacteria. The ranger thinks that the bacteria will divide by the same rule as in the first experiment. </p><p>Help Qwerty and find the minimum number of seconds needed to get a tube with at least <span class="tex-span"><i>z</i></span> bacteria in the second experiment.</p></div><div class="input-specification"><p>The first line contains four space-separated integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>k</i>, <i>b</i>, <i>n</i>, <i>t</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the parameters of bacterial growth, the time Qwerty needed to grow <span class="tex-span"><i>z</i></span> bacteria in the first experiment and the initial number of bacteria in the second experiment, correspondingly.</p></div><div class="output-specification"><p>Print a single number — the minimum number of seconds Qwerty needs to grow at least <span class="tex-span"><i>z</i></span> bacteria in the tube.</p></div>

## Input

<p>The first line contains four space-separated integers <span class="tex-span"><i>k</i></span>, <span class="tex-span"><i>b</i></span>, <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>k</i>, <i>b</i>, <i>n</i>, <i>t</i> ≤ 10<sup class="upper-index">6</sup>)</span> — the parameters of bacterial growth, the time Qwerty needed to grow <span class="tex-span"><i>z</i></span> bacteria in the first experiment and the initial number of bacteria in the second experiment, correspondingly.</p>

## Output

<p>Print a single number — the minimum number of seconds Qwerty needs to grow at least <span class="tex-span"><i>z</i></span> bacteria in the tube.</p>





```input1
3 1 3 5

```




```input2
1 4 4 7

```




```input3
2 2 4 100

```




```output1
2
```




```output2
3
```




```output3
0
```


