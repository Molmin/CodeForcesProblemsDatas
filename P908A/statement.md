## Description

<div><p>Your friend has <span class="tex-span"><i>n</i></span> cards.</p><p>You know that each card has a lowercase English letter on one side and a digit on the other.</p><p>Currently, your friend has laid out the cards on a table so only one side of each card is visible.</p><p>You would like to know if the following statement is true for cards that your friend owns: "If a card has a vowel on one side, then it has an even digit on the other side." More specifically, a vowel is one of '<span class="tex-font-style-tt">a</span>', '<span class="tex-font-style-tt">e</span>', '<span class="tex-font-style-tt">i</span>', '<span class="tex-font-style-tt">o</span>' or '<span class="tex-font-style-tt">u</span>', and even digit is one of '<span class="tex-font-style-tt">0</span>', '<span class="tex-font-style-tt">2</span>', '<span class="tex-font-style-tt">4</span>', '<span class="tex-font-style-tt">6</span>' or '<span class="tex-font-style-tt">8</span>'.</p><p>For example, if a card has '<span class="tex-font-style-tt">a</span>' on one side, and '<span class="tex-font-style-tt">6</span>' on the other side, then this statement is true for it. Also, the statement is true, for example, for a card with '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">4</span>', and for a card with '<span class="tex-font-style-tt">b</span>' and '<span class="tex-font-style-tt">3</span>' (since the letter is not a vowel). The statement is false, for example, for card with '<span class="tex-font-style-tt">e</span>' and '<span class="tex-font-style-tt">5</span>'. You are interested if the statement is true for all cards. In particular, if no card has a vowel, the statement is true.</p><p>To determine this, you can flip over some cards to reveal the other side. You would like to know what is the minimum number of cards you need to flip in the worst case in order to verify that the statement is true.</p></div><div class="input-specification"><p>The first and only line of input will contain a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 50</span>), denoting the sides of the cards that you can see on the table currently. Each character of <span class="tex-span"><i>s</i></span> is either a lowercase English letter or a digit.</p></div><div class="output-specification"><p>Print a single integer, the minimum number of cards you must turn over to verify your claim.</p></div>

## Input

<p>The first and only line of input will contain a string <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 50</span>), denoting the sides of the cards that you can see on the table currently. Each character of <span class="tex-span"><i>s</i></span> is either a lowercase English letter or a digit.</p>

## Output

<p>Print a single integer, the minimum number of cards you must turn over to verify your claim.</p>





```input1
ee

```




```input2
z

```




```input3
0ay1

```




```output1
2

```




```output2
0

```




```output3
2

```



## Note

<p>In the first sample, we must turn over both cards. Note that even though both cards have the same letter, they could possibly have different numbers on the other side.</p><p>In the second sample, we don't need to turn over any cards. The statement is vacuously true, since you know your friend has no cards with a vowel on them.</p><p>In the third sample, we need to flip the second and fourth cards.</p>
