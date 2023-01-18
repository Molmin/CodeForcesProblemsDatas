## Description

<div><p>To quickly hire highly skilled specialists one of the new IT City companies made an unprecedented move. Every employee was granted a car, and an employee can choose one of four different car makes.</p><p>The parking lot before the office consists of one line of <span class="tex-span">(2<i>n</i> - 2)</span> parking spaces. Unfortunately the total number of cars is greater than the parking lot capacity. Furthermore even amount of cars of each make is greater than the amount of parking spaces! That's why there are no free spaces on the parking lot ever.</p><p>Looking on the straight line of cars the company CEO thought that parking lot would be more beautiful if it contained exactly <span class="tex-span"><i>n</i></span> successive cars of the same make. Help the CEO determine the number of ways to fill the parking lot this way.</p></div><div class="input-specification"><p>The only line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 30</span>) — the amount of successive cars of the same make.</p></div><div class="output-specification"><p>Output one integer — the number of ways to fill the parking lot by cars of four makes using the described way.</p></div>

## Input

<p>The only line of the input contains one integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">3 ≤ <i>n</i> ≤ 30</span>) — the amount of successive cars of the same make.</p>

## Output

<p>Output one integer — the number of ways to fill the parking lot by cars of four makes using the described way.</p>





```input1
3

```




```output1
24
```



## Note

<p>Let's denote car makes in the following way: A — Aston Martin, B —   Bentley, M — Mercedes-Maybach, Z — Zaporozhets. For <span class="tex-span"><i>n</i> = 3</span> there are the following appropriate ways to fill the parking lot: AAAB AAAM AAAZ ABBB AMMM AZZZ BBBA BBBM BBBZ BAAA BMMM BZZZ MMMA MMMB MMMZ MAAA MBBB MZZZ ZZZA ZZZB ZZZM ZAAA ZBBB ZMMM</p><p>Originally it was planned to grant sport cars of Ferrari, Lamborghini, Maserati and Bugatti makes but this idea was renounced because it is impossible to drive these cars having small road clearance on the worn-down roads of IT City.</p>
