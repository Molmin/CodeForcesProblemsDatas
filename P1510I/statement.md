## Description

<div><p>The popular improv website <span class="tex-font-style-underline">Interpretation Impetus</span> hosts regular improv contests and maintains a rating of the best performers. However, since improv can often go horribly wrong, the website is notorious for declaring improv contests <span class="tex-font-style-underline">unrated</span>. It now holds a wager before each improv contest where the participants try to predict whether it will be rated or unrated, and they are now more popular than the improv itself.</p><p>Izzy and $n$ other participants take part in each wager. First, they each make their prediction, expressed as <span class="tex-font-style-tt">1</span> ("rated") or <span class="tex-font-style-tt">0</span> ("unrated"). Izzy always goes last, so she knows the predictions of the other participants when making her own. Then, the actual competition takes place and it is declared either rated or unrated.</p><p>You need to write a program that will interactively play as Izzy. There will be $m$ wagers held in 2021, and Izzy's goal is to have at most $1.3\cdot b + 100$ wrong predictions after all those wagers, where $b$ is the <span class="tex-font-style-underline">smallest</span> number of wrong predictions that any other wager participant will have after all those wagers. </p><p>The number $b$ is not known in advance. Izzy also knows nothing about the other participants&nbsp;— they might somehow always guess correctly, or their predictions might be correlated. Izzy's predictions, though, do not affect the predictions of the other participants and the decision on the contest being rated or not&nbsp;— in other words, in each test case, your program always receives the same inputs, no matter what it outputs.</p></div><div><h2>Interaction</h2><p>First, a solution must read two integers $n$ ($1 \le n \le 1000$) and $m$ ($1 \le m \le 10\,000$). Then, the solution must process $m$ wagers. For each of them, the solution must first read a string consisting of $n$ <span class="tex-font-style-tt">0</span>s and <span class="tex-font-style-tt">1</span>s, in which the $i$-th character denotes the guess of the $i$-th participant. Then, the solution must print Izzy's guess as <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>. Don't forget to flush the output after printing it! Then, the solution must read the actual outcome, also as <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span>, and then proceed to the next wager, if this wasn't the last one. </p><p>Your solution will be considered correct if it makes at most $1.3\cdot b + 100$ mistakes, where $b$ is the smallest number of mistakes made by any other participant. Note that if a solution outputs anything except <span class="tex-font-style-tt">0</span> or <span class="tex-font-style-tt">1</span> for a wager, it will be considered incorrect even if it made no other mistakes. </p><p>There are 200 test cases in this problem.</p></div>





```input1
3 4
000

1
100

1
001

0
111

1
```




```output1
0


0


1


1
```



## Note

<p>In the example, the participants made 1, 2, and 3 mistakes respectively, therefore $b=1$ (the smallest of these numbers). Izzy made 3 mistakes, which were not more than $1.3\cdot b + 100=101.3$, so these outputs are good enough to pass this test case (as are any other valid outputs).</p>
