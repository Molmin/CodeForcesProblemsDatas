## Description

<div><p>The protection of a popular program developed by one of IT City companies is organized the following way. After installation it outputs a random five digit number which should be sent in SMS to a particular phone number. In response an SMS activation code arrives.</p><p>A young hacker Vasya disassembled the program and found the algorithm that transforms the shown number into the activation code. <span class="tex-font-style-it">Note: it is clear that Vasya is a law-abiding hacker, and made it for a noble purpose — to show the developer the imperfection of their protection.</span></p><p>The found algorithm looks the following way. At first the digits of the number are shuffled in the following order &lt;first digit&gt;&lt;third digit&gt;&lt;fifth digit&gt;&lt;fourth digit&gt;&lt;second digit&gt;. For example the shuffle of <span class="tex-span">12345</span> should lead to <span class="tex-span">13542</span>. On the second stage the number is raised to the fifth power. The result of the shuffle and exponentiation of the number <span class="tex-span">12345</span> is <span class="tex-span">455&nbsp;422&nbsp;043&nbsp;125&nbsp;550&nbsp;171&nbsp;232</span>. The answer is the <span class="tex-span">5</span> last digits of this result. For the number <span class="tex-span">12345</span> the answer should be <span class="tex-span">71232</span>.</p><p>Vasya is going to write a keygen program implementing this algorithm. Can you do the same?</p></div><div class="input-specification"><p>The only line of the input contains a positive integer five digit number for which the activation code should be found.</p></div><div class="output-specification"><p>Output exactly <span class="tex-span">5</span> digits without spaces between them — the found activation code of the program.</p></div>

## Input

<p>The only line of the input contains a positive integer five digit number for which the activation code should be found.</p>

## Output

<p>Output exactly <span class="tex-span">5</span> digits without spaces between them — the found activation code of the program.</p>





```input1
12345

```




```output1
71232
```


