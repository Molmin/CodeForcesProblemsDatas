## Description

<div><p>Constanze is the smartest girl in her village but she has bad eyesight.</p><p>One day, she was able to invent an incredible machine! When you pronounce letters, the machine will inscribe them onto a piece of paper. For example, if you pronounce 'c', 'o', 'd', and 'e' in that order, then the machine will inscribe "<span class="tex-font-style-tt">code</span>" onto the paper. Thanks to this machine, she can finally write messages without using her glasses.</p><p>However, her dumb friend Akko decided to play a prank on her. Akko tinkered with the machine so that if you pronounce 'w', it will inscribe "<span class="tex-font-style-tt">uu</span>" instead of "<span class="tex-font-style-tt">w</span>", and if you pronounce 'm', it will inscribe "<span class="tex-font-style-tt">nn</span>" instead of "<span class="tex-font-style-tt">m</span>"! Since Constanze had bad eyesight, she was not able to realize what Akko did.</p><p>The rest of the letters behave the same as before: if you pronounce any letter besides 'w' and 'm', the machine will just inscribe it onto a piece of paper.</p><p>The next day, I received a letter in my mailbox. I can't understand it so I think it's either just some gibberish from Akko, or Constanze made it using her machine. But since I know what Akko did, I can just list down all possible strings that Constanze's machine would have turned into the message I got and see if anything makes sense.</p><p>But I need to know how much paper I will need, and that's why I'm asking you for help. Tell me the number of strings that Constanze's machine would've turned into the message I got.</p><p>But since this number can be quite large, tell me instead its remainder when divided by $10^9+7$.</p><p>If there are no strings that Constanze's machine would've turned into the message I got, then print $0$.</p></div><div class="input-specification"><p>Input consists of a single line containing a string $s$ ($1 \leq |s| \leq 10^5$) — the received message. $s$ contains only lowercase Latin letters.</p></div><div class="output-specification"><p>Print a single integer — the number of strings that Constanze's machine would've turned into the message $s$, modulo $10^9+7$.</p></div>

## Input

<p>Input consists of a single line containing a string $s$ ($1 \leq |s| \leq 10^5$) — the received message. $s$ contains only lowercase Latin letters.</p>

## Output

<p>Print a single integer — the number of strings that Constanze's machine would've turned into the message $s$, modulo $10^9+7$.</p>





```input1
ouuokarinn
```




```input2
banana
```




```input3
nnn
```




```input4
amanda
```




```output1
4
```




```output2
1
```




```output3
3
```




```output4
0
```



## Note

<p>For the first example, the candidate strings are the following: "<span class="tex-font-style-tt">ouuokarinn</span>", "<span class="tex-font-style-tt">ouuokarim</span>", "<span class="tex-font-style-tt">owokarim</span>", and "<span class="tex-font-style-tt">owokarinn</span>".</p><p>For the second example, there is only one: "<span class="tex-font-style-tt">banana</span>".</p><p>For the third example, the candidate strings are the following: "<span class="tex-font-style-tt">nm</span>", "<span class="tex-font-style-tt">mn</span>" and "<span class="tex-font-style-tt">nnn</span>".</p><p>For the last example, there are no candidate strings that the machine can turn into "<span class="tex-font-style-tt">amanda</span>", since the machine won't inscribe 'm'.</p>
