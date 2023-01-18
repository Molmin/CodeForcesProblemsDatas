## Description

<div><p>There are two popular keyboard layouts in Berland, they differ only in letters positions. All the other keys are the same. In Berland they use alphabet with <span class="tex-span">26</span> letters which coincides with English alphabet.</p><p>You are given two strings consisting of <span class="tex-span">26</span> distinct letters each: all keys of the first and the second layouts in the same order. </p><p>You are also given some text consisting of small and capital English letters and digits. It is known that it was typed in the first layout, but the writer intended to type it in the second layout. Print the text if the same keys were pressed in the second layout.</p><p>Since all keys but letters are the same in both layouts, the capitalization of the letters should remain the same, as well as all other characters.</p></div><div class="input-specification"><p>The first line contains a string of length <span class="tex-span">26</span> consisting of distinct lowercase English letters. This is the first layout.</p><p>The second line contains a string of length <span class="tex-span">26</span> consisting of distinct lowercase English letters. This is the second layout.</p><p>The third line contains a non-empty string <span class="tex-span"><i>s</i></span> consisting of lowercase and uppercase English letters and digits. This is the text typed in the first layout. The length of <span class="tex-span"><i>s</i></span> does not exceed <span class="tex-span">1000</span>.</p></div><div class="output-specification"><p>Print the text if the same keys were pressed in the second layout.</p></div>

## Input

<p>The first line contains a string of length <span class="tex-span">26</span> consisting of distinct lowercase English letters. This is the first layout.</p><p>The second line contains a string of length <span class="tex-span">26</span> consisting of distinct lowercase English letters. This is the second layout.</p><p>The third line contains a non-empty string <span class="tex-span"><i>s</i></span> consisting of lowercase and uppercase English letters and digits. This is the text typed in the first layout. The length of <span class="tex-span"><i>s</i></span> does not exceed <span class="tex-span">1000</span>.</p>

## Output

<p>Print the text if the same keys were pressed in the second layout.</p>





```input1
qwertyuiopasdfghjklzxcvbnm
veamhjsgqocnrbfxdtwkylupzi
TwccpQZAvb2017

```




```input2
mnbvcxzlkjhgfdsapoiuytrewq
asdfghjklqwertyuiopzxcvbnm
7abaCABAABAcaba7

```




```output1
HelloVKCup2017

```




```output2
7uduGUDUUDUgudu7

```


