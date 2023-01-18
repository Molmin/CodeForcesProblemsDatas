## Description

<div><p>Polycarp has a cat and his cat is a real gourmet! Dependent on a day of the week he eats certain type of food:</p><ul> <li> on Mondays, Thursdays and Sundays he eats <span class="tex-font-style-it">fish food</span>; </li><li> on Tuesdays and Saturdays he eats <span class="tex-font-style-it">rabbit stew</span>; </li><li> on other days of week he eats <span class="tex-font-style-it">chicken stake</span>. </li></ul><p>Polycarp plans to go on a trip and already packed his backpack. His backpack contains:</p><ul> <li> $a$ daily rations of <span class="tex-font-style-it">fish food</span>; </li><li> $b$ daily rations of <span class="tex-font-style-it">rabbit stew</span>; </li><li> $c$ daily rations of <span class="tex-font-style-it">chicken stakes</span>. </li></ul><p>Polycarp has to choose such day of the week to start his trip that his cat can eat without additional food purchases as long as possible. Print the maximum number of days the cat can eat in a trip without additional food purchases, if Polycarp chooses the day of the week to start his trip optimally.</p></div><div class="input-specification"><p>The first line of the input contains three positive integers $a$, $b$ and $c$ ($1 \le a, b, c \le 7\cdot10^8$) — the number of daily rations of <span class="tex-font-style-it">fish food</span>, <span class="tex-font-style-it">rabbit stew</span> and <span class="tex-font-style-it">chicken stakes</span> in Polycarps backpack correspondingly.</p></div><div class="output-specification"><p>Print the maximum number of days the cat can eat in a trip without additional food purchases, if Polycarp chooses the day of the week to start his trip optimally.</p></div>

## Input

<p>The first line of the input contains three positive integers $a$, $b$ and $c$ ($1 \le a, b, c \le 7\cdot10^8$) — the number of daily rations of <span class="tex-font-style-it">fish food</span>, <span class="tex-font-style-it">rabbit stew</span> and <span class="tex-font-style-it">chicken stakes</span> in Polycarps backpack correspondingly.</p>

## Output

<p>Print the maximum number of days the cat can eat in a trip without additional food purchases, if Polycarp chooses the day of the week to start his trip optimally.</p>





```input1
2 1 1
```




```input2
3 2 2
```




```input3
1 100 1
```




```input4
30 20 10
```




```output1
4
```




```output2
7
```




```output3
3
```




```output4
39
```



## Note

<p>In the first example the best day for start of the trip is Sunday. In this case, during Sunday and Monday the cat will eat <span class="tex-font-style-it">fish food</span>, during Tuesday — <span class="tex-font-style-it">rabbit stew</span> and during Wednesday — <span class="tex-font-style-it">chicken stake</span>. So, after four days of the trip all food will be eaten.</p><p>In the second example Polycarp can start his trip in any day of the week. In any case there are food supplies only for one week in Polycarps backpack.</p><p>In the third example Polycarp can start his trip in any day, excluding Wednesday, Saturday and Sunday. In this case, the cat will eat three different dishes in three days. Nevertheless that after three days of a trip there will be $99$ portions of <span class="tex-font-style-it">rabbit stew</span> in a backpack, can cannot eat anything in fourth day of a trip.</p>
