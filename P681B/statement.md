## Description

<div><p>Kolya is developing an economy simulator game. His most favourite part of the development process is in-game testing. Once he was entertained by the testing so much, that he found out his game-coin score become equal to <span class="tex-span">0</span>.</p><p>Kolya remembers that at the beginning of the game his game-coin score was equal to <span class="tex-span"><i>n</i></span> and that he have bought only some houses (for <span class="tex-span">1 234 567</span> game-coins each), cars (for <span class="tex-span">123 456</span> game-coins each) and computers (for <span class="tex-span">1 234</span> game-coins each).</p><p>Kolya is now interested, whether he could have spent all of his initial <span class="tex-span"><i>n</i></span> game-coins buying only houses, cars and computers or there is a bug in the game. Formally, is there a triple of non-negative integers <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> and <span class="tex-span"><i>c</i></span> such that <span class="tex-span"><i>a</i> × 1 234 567 + <i>b</i> × 123 456 + <i>c</i> × 1 234 = <i>n</i></span>?</p><p>Please help Kolya answer this question.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— Kolya's initial game-coin score.</p></div><div class="output-specification"><p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it's possible that Kolya spent all of his initial <span class="tex-span"><i>n</i></span> coins buying only houses, cars and computers. Otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10<sup class="upper-index">9</sup></span>)&nbsp;— Kolya's initial game-coin score.</p>

## Output

<p>Print "<span class="tex-font-style-tt">YES</span>" (without quotes) if it's possible that Kolya spent all of his initial <span class="tex-span"><i>n</i></span> coins buying only houses, cars and computers. Otherwise print "<span class="tex-font-style-tt">NO</span>" (without quotes).</p>





```input1
1359257

```




```input2
17851817

```




```output1
YES
```




```output2
NO
```



## Note

<p>In the first sample, one of the possible solutions is to buy one house, one car and one computer, spending <span class="tex-span">1 234 567 + 123 456 + 1234 = 1 359 257</span> game-coins in total.</p>
