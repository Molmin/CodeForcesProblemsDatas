## Description

<div><p>By 2312 there were <span class="tex-span"><i>n</i></span> Large Hadron Colliders in the inhabited part of the universe. Each of them corresponded to a single natural number from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span>. However, scientists did not know what activating several colliders simultaneously could cause, so the colliders were deactivated.</p><p>In 2312 there was a startling discovery: a collider's activity is safe if and only if all numbers of activated colliders are pairwise relatively prime to each other (two numbers are relatively prime if their greatest common divisor equals <span class="tex-span">1</span>)! If two colliders with relatively nonprime numbers are activated, it will cause a global collapse.</p><p>Upon learning this, physicists rushed to turn the colliders on and off and carry out all sorts of experiments. To make sure than the scientists' quickness doesn't end with big trouble, the Large Hadron Colliders' Large Remote Control was created. You are commissioned to write the software for the remote (well, you do not expect anybody to operate it manually, do you?).</p><p>Initially, all colliders are deactivated. Your program receives multiple requests of the form "activate/deactivate the <span class="tex-span"><i>i</i></span>-th collider". The program should handle requests in the order of receiving them. The program should print the processed results in the format described below.</p><p>To the request of "<span class="tex-font-style-tt">+ i</span>" (that is, to activate the <span class="tex-span"><i>i</i></span>-th collider), the program should print exactly one of the following responses: </p><ul> <li> "<span class="tex-font-style-tt">Success</span>" if the activation was successful. </li><li> "<span class="tex-font-style-tt">Already on</span>", if the <span class="tex-span"><i>i</i></span>-th collider was already activated before the request. </li><li> "<span class="tex-font-style-tt">Conflict with j</span>", if there is a conflict with the <span class="tex-span"><i>j</i></span>-th collider (that is, the <span class="tex-span"><i>j</i></span>-th collider is on, and numbers <span class="tex-span"><i>i</i></span> and <span class="tex-span"><i>j</i></span> are not relatively prime). In this case, the <span class="tex-span"><i>i</i></span>-th collider shouldn't be activated. If a conflict occurs with several colliders simultaneously, you should print the number of any of them. </li></ul><p>The request of "<span class="tex-font-style-tt">- i</span>" (that is, to deactivate the <span class="tex-span"><i>i</i></span>-th collider), should receive one of the following responses from the program: </p><ul> <li> "<span class="tex-font-style-tt">Success</span>", if the deactivation was successful. </li><li> "<span class="tex-font-style-tt">Already off</span>", if the <span class="tex-span"><i>i</i></span>-th collider was already deactivated before the request. </li></ul><p>You don't need to print quotes in the output of the responses to the requests.</p></div><div class="input-specification"><p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of colliders and the number of requests, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain numbers of requests, one per line, in the form of either "<span class="tex-font-style-tt">+ i</span>" (without the quotes) — activate the <span class="tex-span"><i>i</i></span>-th collider, or "<span class="tex-font-style-tt">-&nbsp;i</span>" (without the quotes) — deactivate the <span class="tex-span"><i>i</i></span>-th collider (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>m</i></span> lines — the results of executing requests in the above given format. The requests should be processed in the order, in which they are given in the input. Don't forget that the responses to the requests should be printed without quotes.</p></div>

## Input

<p>The first line contains two space-separated integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>n</i>, <i>m</i> ≤ 10<sup class="upper-index">5</sup></span>) — the number of colliders and the number of requests, correspondingly.</p><p>Next <span class="tex-span"><i>m</i></span> lines contain numbers of requests, one per line, in the form of either "<span class="tex-font-style-tt">+ i</span>" (without the quotes) — activate the <span class="tex-span"><i>i</i></span>-th collider, or "<span class="tex-font-style-tt">-&nbsp;i</span>" (without the quotes) — deactivate the <span class="tex-span"><i>i</i></span>-th collider (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>).</p>

## Output

<p>Print <span class="tex-span"><i>m</i></span> lines — the results of executing requests in the above given format. The requests should be processed in the order, in which they are given in the input. Don't forget that the responses to the requests should be printed without quotes.</p>





```input1
10 10
+ 6
+ 10
+ 5
- 10
- 5
- 6
+ 10
+ 3
+ 6
+ 3

```




```output1
Success
Conflict with 6
Success
Already off
Success
Success
Success
Success
Conflict with 10
Already on

```



## Note

<p>Note that in the sample the colliders don't turn on after the second and ninth requests. The ninth request could also receive response "<span class="tex-font-style-tt">Conflict with 3</span>".</p>
