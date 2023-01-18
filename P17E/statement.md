## Description

<div><p>In an English class Nick had nothing to do at all, and remembered about wonderful strings called <span class="tex-font-style-underline">palindromes</span>. We should remind you that a string is called a palindrome if it can be read the same way both from left to right and from right to left. Here are examples of such strings: «<span class="tex-font-style-tt">eye</span>», «<span class="tex-font-style-tt">pop</span>», «<span class="tex-font-style-tt">level</span>», «<span class="tex-font-style-tt">aba</span>», «<span class="tex-font-style-tt">deed</span>», «<span class="tex-font-style-tt">racecar</span>», «<span class="tex-font-style-tt">rotor</span>», «<span class="tex-font-style-tt">madam</span>». </p><p>Nick started to look carefully for all palindromes in the text that they were reading in the class. For each occurrence of each palindrome in the text he wrote a pair — the position of the beginning and the position of the ending of this occurrence in the text. Nick called each occurrence of each palindrome he found in the text <span class="tex-font-style-underline">subpalindrome</span>. When he found all the subpalindromes, he decided to find out how many different pairs among these subpalindromes cross. Two subpalindromes cross if they cover common positions in the text. No palindrome can cross itself.</p><p>Let's look at the actions, performed by Nick, by the example of text «<span class="tex-font-style-tt">babb</span>». At first he wrote out all subpalindromes:</p><center>• «<span class="tex-font-style-tt">b</span>» — <span class="tex-span">1..1</span> </center><center>• «<span class="tex-font-style-tt">bab</span>» — <span class="tex-span">1..3</span> </center><center>• «<span class="tex-font-style-tt">a</span>» — <span class="tex-span">2..2</span> </center><center>• «<span class="tex-font-style-tt">b</span>» — <span class="tex-span">3..3</span> </center><center>• «<span class="tex-font-style-tt">bb</span>» — <span class="tex-span">3..4</span> </center><center>• «<span class="tex-font-style-tt">b</span>» — <span class="tex-span">4..4</span> </center><p>Then Nick counted the amount of different pairs among these subpalindromes that cross. These pairs were six:</p><center> <span class="tex-font-style-tt">1.</span> <span class="tex-span">1..1</span> cross with <span class="tex-span">1..3</span> </center><center> <span class="tex-font-style-tt">2.</span> <span class="tex-span">1..3</span> cross with <span class="tex-span">2..2</span> </center><center> <span class="tex-font-style-tt">3.</span> <span class="tex-span">1..3</span> cross with <span class="tex-span">3..3</span> </center><center> <span class="tex-font-style-tt">4.</span> <span class="tex-span">1..3</span> cross with <span class="tex-span">3..4</span> </center><center> <span class="tex-font-style-tt">5.</span> <span class="tex-span">3..3</span> cross with <span class="tex-span">3..4</span> </center><center> <span class="tex-font-style-tt">6.</span> <span class="tex-span">3..4</span> cross with <span class="tex-span">4..4</span> </center><p>Since it's very exhausting to perform all the described actions manually, Nick asked you to help him and write a program that can find out the amount of different subpalindrome pairs that cross. Two subpalindrome pairs are regarded as different if one of the pairs contains a subpalindrome that the other does not.</p></div><div class="input-specification"><p>The first input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">6</sup></span>) — length of the text. The following line contains <span class="tex-span"><i>n</i></span> lower-case Latin letters (from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">z</span>).</p></div><div class="output-specification"><p>In the only line output the amount of different pairs of two subpalindromes that cross each other. Output the answer modulo <span class="tex-span">51123987</span>.</p></div>

## Input

<p>The first input line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 2·10<sup class="upper-index">6</sup></span>) — length of the text. The following line contains <span class="tex-span"><i>n</i></span> lower-case Latin letters (from <span class="tex-font-style-tt">a</span> to <span class="tex-font-style-tt">z</span>).</p>

## Output

<p>In the only line output the amount of different pairs of two subpalindromes that cross each other. Output the answer modulo <span class="tex-span">51123987</span>.</p>





```input1
4
babb

```




```input2
2
aa

```




```output1
6

```




```output2
2

```


