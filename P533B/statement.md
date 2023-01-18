## Description

<div><p>One Big Software Company has <span class="tex-span"><i>n</i></span> employees numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. The director is assigned number <span class="tex-span">1</span>. Every employee of the company except the director has exactly one immediate superior. The director, of course, doesn't have a superior.</p><p>We will call person <span class="tex-span"><i>a</i></span> a subordinates of another person <span class="tex-span"><i>b</i></span>, if either <span class="tex-span"><i>b</i></span> is an immediate supervisor of <span class="tex-span"><i>a</i></span>, or the immediate supervisor of <span class="tex-span"><i>a</i></span> is a subordinate to person <span class="tex-span"><i>b</i></span>. In particular, subordinates of the head are all other employees of the company.</p><p>To solve achieve an Important Goal we need to form a workgroup. Every person has some efficiency, expressed by a positive integer <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span>, where <span class="tex-span"><i>i</i></span> is the person's number. The efficiency of the workgroup is defined as the total efficiency of all the people included in it.</p><p>The employees of the big software company are obsessed with modern ways of work process organization. Today pair programming is at the peak of popularity, so the workgroup should be formed with the following condition. Each person entering the workgroup should be able to sort all of his subordinates who are also in the workgroup into pairs. In other words, for each of the members of the workgroup the number of his subordinates within the workgroup should be even.</p><p>Your task is to determine the maximum possible efficiency of the workgroup formed at observing the given condition. Any person including the director of company can enter the workgroup.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of workers of the Big Software Company. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, describing the company employees. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — the number of the person who is the <span class="tex-span"><i>i</i></span>-th employee's immediate superior and <span class="tex-span"><i>i</i></span>-th employee's efficiency. For the director <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> =  - 1</span>, for all other people the condition <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span> is fulfilled.</p></div><div class="output-specification"><p>Print a single integer — the maximum possible efficiency of the workgroup.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">5</sup></span>) — the number of workers of the Big Software Company. </p><p>Then <span class="tex-span"><i>n</i></span> lines follow, describing the company employees. The <span class="tex-span"><i>i</i></span>-th line contains two integers <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub>, <i>a</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">5</sup></span>) — the number of the person who is the <span class="tex-span"><i>i</i></span>-th employee's immediate superior and <span class="tex-span"><i>i</i></span>-th employee's efficiency. For the director <span class="tex-span"><i>p</i><sub class="lower-index">1</sub> =  - 1</span>, for all other people the condition <span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> &lt; <i>i</i></span> is fulfilled.</p>

## Output

<p>Print a single integer — the maximum possible efficiency of the workgroup.</p>





```input1
7
-1 3
1 2
1 1
1 4
4 5
4 3
5 2

```




```output1
17

```



## Note

<p>In the sample test the most effective way is to make a workgroup from employees number <span class="tex-span">1, 2, 4, 5, 6</span>.</p>
