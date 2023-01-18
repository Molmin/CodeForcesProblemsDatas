## Description

<div><p>Devu is a dumb guy, his learning curve is very slow. You are supposed to teach him <span class="tex-span"><i>n</i></span> subjects, the <span class="tex-span"><i>i</i><sup class="upper-index"><i>th</i></sup></span> subject has <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> chapters. When you teach him, you are supposed to teach all the chapters of a subject continuously.</p><p>Let us say that his initial per chapter learning power of a subject is <span class="tex-span"><i>x</i></span> hours. In other words he can learn a chapter of a particular subject in <span class="tex-span"><i>x</i></span> hours.</p><p>Well Devu is not complete dumb, there is a good thing about him too. If you teach him a subject, then time required to teach any chapter of the next subject will require exactly 1 hour less than previously required (see the examples to understand it more clearly). Note that his per chapter learning power can not be less than 1 hour.</p><p>You can teach him the <span class="tex-span"><i>n</i></span> subjects in any possible order. Find out minimum amount of time (in hours) Devu will take to understand all the subjects and you will be free to do some enjoying task rather than teaching a dumb guy.</p><p><span class="tex-font-style-it">Please be careful that answer might not fit in 32 bit data type.</span></p></div><div class="input-specification"><p>The first line will contain two space separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>). The next line will contain <span class="tex-span"><i>n</i></span> space separated integers: <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p></div><div class="output-specification"><p>Output a single integer representing the answer to the problem.</p></div>

## Input

<p>The first line will contain two space separated integers <span class="tex-span"><i>n</i></span>, <span class="tex-span"><i>x</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>x</i> ≤ 10<sup class="upper-index">5</sup></span>). The next line will contain <span class="tex-span"><i>n</i></span> space separated integers: <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>).</p>

## Output

<p>Output a single integer representing the answer to the problem.</p>





```input1
2 3
4 1

```




```input2
4 2
5 1 2 1

```




```input3
3 3
1 1 1

```




```output1
11

```




```output2
10

```




```output3
6

```



## Note

<p>Look at the first example. Consider the order of subjects: <span class="tex-span">1</span>, <span class="tex-span">2</span>. When you teach Devu the first subject, it will take him <span class="tex-span">3</span> hours per chapter, so it will take <span class="tex-span">12</span> hours to teach first subject. After teaching first subject, his per chapter learning time will be <span class="tex-span">2</span> hours. Now teaching him second subject will take <span class="tex-span">2 × 1 = 2</span> hours. Hence you will need to spend <span class="tex-span">12 + 2 = 14</span> hours.</p><p>Consider the order of subjects: <span class="tex-span">2</span>, <span class="tex-span">1</span>. When you teach Devu the second subject, then it will take him <span class="tex-span">3</span> hours per chapter, so it will take <span class="tex-span">3 × 1 = 3</span> hours to teach the second subject. After teaching the second subject, his per chapter learning time will be <span class="tex-span">2</span> hours. Now teaching him the first subject will take <span class="tex-span">2 × 4 = 8</span> hours. Hence you will need to spend <span class="tex-span">11</span> hours.</p><p>So overall, minimum of both the cases is <span class="tex-span">11</span> hours.</p><p>Look at the third example. The order in this example doesn't matter. When you teach Devu the first subject, it will take him <span class="tex-span">3</span> hours per chapter. When you teach Devu the second subject, it will take him <span class="tex-span">2</span> hours per chapter. When you teach Devu the third subject, it will take him <span class="tex-span">1</span> hours per chapter. In total it takes <span class="tex-span">6</span> hours.</p>
