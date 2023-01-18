## Description

<div><p>Vasya studies divisibility rules at school. Here are some of them:</p><ul><li> <span class="tex-font-style-it">Divisibility by <span class="tex-span">2</span>.</span> A number is divisible by <span class="tex-span">2</span> if and only if its last digit is divisible by <span class="tex-span">2</span> or in other words, is even.</li><li> <span class="tex-font-style-it">Divisibility by <span class="tex-span">3</span>.</span> A number is divisible by <span class="tex-span">3</span> if and only if the sum of its digits is divisible by <span class="tex-span">3</span>.</li><li> <span class="tex-font-style-it">Divisibility by <span class="tex-span">4</span>.</span> A number is divisible by <span class="tex-span">4</span> if and only if its last two digits form a number that is divisible by <span class="tex-span">4</span>.</li><li> <span class="tex-font-style-it">Divisibility by <span class="tex-span">5</span>.</span> A number is divisible by <span class="tex-span">5</span> if and only if its last digit equals <span class="tex-span">5</span> or <span class="tex-span">0</span>.</li><li> <span class="tex-font-style-it">Divisibility by <span class="tex-span">6</span>.</span> A number is divisible by <span class="tex-span">6</span> if and only if it is divisible by <span class="tex-span">2</span> and <span class="tex-span">3</span> simultaneously (that is, if the last digit is even and the sum of all digits is divisible by <span class="tex-span">3</span>).</li><li> <span class="tex-font-style-it">Divisibility by <span class="tex-span">7</span>.</span> Vasya doesn't know such divisibility rule.</li><li> <span class="tex-font-style-it">Divisibility by <span class="tex-span">8</span>.</span> A number is divisible by <span class="tex-span">8</span> if and only if its last three digits form a number that is divisible by <span class="tex-span">8</span>.</li><li> <span class="tex-font-style-it">Divisibility by <span class="tex-span">9</span>.</span> A number is divisible by <span class="tex-span">9</span> if and only if the sum of its digits is divisible by <span class="tex-span">9</span>.</li><li> <span class="tex-font-style-it">Divisibility by <span class="tex-span">10</span>.</span> A number is divisible by <span class="tex-span">10</span> if and only if its last digit is a zero.</li><li> <span class="tex-font-style-it">Divisibility by <span class="tex-span">11</span>.</span> A number is divisible by <span class="tex-span">11</span> if and only if the sum of digits on its odd positions either equals to the sum of digits on the even positions, or they differ in a number that is divisible by <span class="tex-span">11</span>.</li></ul><p>Vasya got interested by the fact that some divisibility rules resemble each other. In fact, to check a number's divisibility by <span class="tex-span">2</span>, <span class="tex-span">4</span>, <span class="tex-span">5</span>, <span class="tex-span">8</span> and <span class="tex-span">10</span> it is enough to check fulfiling some condition for one or several last digits. Vasya calls such rules the <span class="tex-font-style-bf"><span class="tex-span">2</span>-type</span> rules.</p><p>If checking divisibility means finding a sum of digits and checking whether the sum is divisible by the given number, then Vasya calls this rule the <span class="tex-font-style-bf"><span class="tex-span">3</span>-type</span> rule (because it works for numbers <span class="tex-span">3</span> and <span class="tex-span">9</span>).</p><p>If we need to find the difference between the sum of digits on odd and even positions and check whether the difference is divisible by the given divisor, this rule is called the <span class="tex-font-style-bf"><span class="tex-span">11</span>-type</span> rule (it works for number <span class="tex-span">11</span>).</p><p>In some cases we should divide the divisor into several factors and check whether rules of different types (<span class="tex-span">2</span>-type, <span class="tex-span">3</span>-type or <span class="tex-span">11</span>-type) work there. For example, for number <span class="tex-span">6</span> we check <span class="tex-span">2</span>-type and <span class="tex-span">3</span>-type rules, for number <span class="tex-span">66</span> we check all three types. Such mixed divisibility rules are called <span class="tex-font-style-bf"><span class="tex-span">6</span>-type</span> rules. </p><p>And finally, there are some numbers for which no rule works: neither <span class="tex-span">2</span>-type, nor <span class="tex-span">3</span>-type, nor <span class="tex-span">11</span>-type, nor <span class="tex-span">6</span>-type. The least such number is number <span class="tex-span">7</span>, so we'll say that in such cases the mysterious <span class="tex-font-style-bf"><span class="tex-span">7</span>-type</span> rule works, the one that Vasya hasn't discovered yet. </p><p>Vasya's dream is finding divisibility rules for all possible numbers. He isn't going to stop on the decimal numbers only. As there are quite many numbers, ha can't do it all by himself. Vasya asked you to write a program that determines the divisibility rule type in the <span class="tex-span"><i>b</i></span>-based notation for the given divisor <span class="tex-span"><i>d</i></span>.</p></div><div class="input-specification"><p>The first input line contains two integers <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">2 ≤ <i>b</i>, <i>d</i> ≤ 100</span>) — the notation system base and the divisor. Both numbers are given in the decimal notation.</p></div><div class="output-specification"><p>On the first output line print the type of the rule in the <span class="tex-span"><i>b</i></span>-based notation system, where the divisor is <span class="tex-span"><i>d</i></span>: "<span class="tex-font-style-tt">2-type</span>", "<span class="tex-font-style-tt">3-type</span>", "<span class="tex-font-style-tt">11-type</span>", "<span class="tex-font-style-tt">6-type</span>" or "<span class="tex-font-style-tt">7-type</span>". If there are several such types, print the one that goes earlier in the given sequence. If a number belongs to the <span class="tex-span">2</span>-type, print on the second line the least number of the last <span class="tex-span"><i>b</i></span>-based digits that we will need to use to check the divisibility.</p></div>

## Input

<p>The first input line contains two integers <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>d</i></span> (<span class="tex-span">2 ≤ <i>b</i>, <i>d</i> ≤ 100</span>) — the notation system base and the divisor. Both numbers are given in the decimal notation.</p>

## Output

<p>On the first output line print the type of the rule in the <span class="tex-span"><i>b</i></span>-based notation system, where the divisor is <span class="tex-span"><i>d</i></span>: "<span class="tex-font-style-tt">2-type</span>", "<span class="tex-font-style-tt">3-type</span>", "<span class="tex-font-style-tt">11-type</span>", "<span class="tex-font-style-tt">6-type</span>" or "<span class="tex-font-style-tt">7-type</span>". If there are several such types, print the one that goes earlier in the given sequence. If a number belongs to the <span class="tex-span">2</span>-type, print on the second line the least number of the last <span class="tex-span"><i>b</i></span>-based digits that we will need to use to check the divisibility.</p>





```input1
10 10

```




```input2
2 3

```




```output1
2-type
1

```




```output2
11-type

```



## Note

<p>The divisibility rule for number <span class="tex-span">3</span> in binary notation looks as follows: "A number is divisible by <span class="tex-span">3</span> if and only if the sum of its digits that occupy the even places differs from the sum of digits that occupy the odd places, in a number that is divisible by <span class="tex-span">3</span>". That's an <span class="tex-span">11</span>-type rule. For example, <span class="tex-span">21<sub class="lower-index">10</sub> = 10101<sub class="lower-index">2</sub></span>. For it the sum of digits on odd positions equals <span class="tex-span">1 + 1 + 1 = 3</span>, an on even positions — <span class="tex-span">0 + 0 = 0</span>. The rule works and the number is divisible by <span class="tex-span">3</span>. </p><p>In some notations a number can fit into the <span class="tex-span">3</span>-type rule and the <span class="tex-span">11</span>-type rule. In this case the correct answer is "<span class="tex-font-style-tt">3-type</span>".</p>
