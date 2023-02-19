## Description

<div><p>Tenten runs a weapon shop for ninjas. Today she is willing to sell $n$ shurikens which cost $1$, $2$, ..., $n$ ryo (local currency). During a day, Tenten will place the shurikens onto the showcase, which is empty at the beginning of the day. Her job is fairly simple: sometimes Tenten places another shuriken (from the available shurikens) on the showcase, and sometimes a ninja comes in and buys a shuriken from the showcase. Since ninjas are thrifty, they always buy the <span class="tex-font-style-bf">cheapest</span> shuriken from the showcase.</p><p>Tenten keeps a record for all events, and she ends up with a list of the following types of records:</p><ul> <li> <span class="tex-font-style-tt">+</span> means that she placed another shuriken on the showcase; </li><li> <span class="tex-font-style-tt">- x</span> means that the shuriken of price $x$ was bought. </li></ul><p>Today was a lucky day, and all shurikens were bought. Now Tenten wonders if her list is consistent, and what could be a possible order of placing the shurikens on the showcase. Help her to find this out!</p></div><div class="input-specification"><p>The first line contains the only integer $n$ ($1\leq n\leq 10^5$) standing for the number of shurikens. </p><p>The following $2n$ lines describe the events in the format described above. It's guaranteed that there are exactly $n$ events of the first type, and each price from $1$ to $n$ occurs exactly once in the events of the second type.</p></div><div class="output-specification"><p>If the list is consistent, print "<span class="tex-font-style-tt">YES</span>". Otherwise (that is, if the list is contradictory and there is no valid order of shurikens placement), print "<span class="tex-font-style-tt">NO</span>".</p><p>In the first case the second line must contain $n$ space-separated integers denoting the prices of shurikens in order they were placed. If there are multiple answers, print any.</p></div>

## Input

<p>The first line contains the only integer $n$ ($1\leq n\leq 10^5$) standing for the number of shurikens. </p><p>The following $2n$ lines describe the events in the format described above. It's guaranteed that there are exactly $n$ events of the first type, and each price from $1$ to $n$ occurs exactly once in the events of the second type.</p>

## Output

<p>If the list is consistent, print "<span class="tex-font-style-tt">YES</span>". Otherwise (that is, if the list is contradictory and there is no valid order of shurikens placement), print "<span class="tex-font-style-tt">NO</span>".</p><p>In the first case the second line must contain $n$ space-separated integers denoting the prices of shurikens in order they were placed. If there are multiple answers, print any.</p>





```input1
4
+
+
- 2
+
- 3
+
- 1
- 4
```




```input2
1
- 1
+
```




```input3
3
+
+
+
- 2
- 1
- 3
```




```output1
YES
4 2 3 1
```




```output2
NO
```




```output3
NO
```



## Note

<p>In the first example Tenten first placed shurikens with prices $4$ and $2$. After this a customer came in and bought the cheapest shuriken which costed $2$. Next, Tenten added a shuriken with price $3$ on the showcase to the already placed $4$-ryo. Then a new customer bought this $3$-ryo shuriken. After this she added a $1$-ryo shuriken. Finally, the last two customers bought shurikens $1$ and $4$, respectively. Note that the order $[2, 4, 3, 1]$ is also valid.</p><p>In the second example the first customer bought a shuriken before anything was placed, which is clearly impossible.</p><p>In the third example Tenten put all her shurikens onto the showcase, after which a customer came in and bought a shuriken with price $2$. This is impossible since the shuriken was not the cheapest, we know that the $1$-ryo shuriken was also there.</p>
