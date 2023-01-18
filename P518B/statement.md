## Description

<div><p>Little Tanya decided to present her dad a postcard on his Birthday. She has already created a message — string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span>, consisting of uppercase and lowercase English letters. Tanya can't write yet, so she found a newspaper and decided to cut out the letters and glue them into the postcard to achieve string <span class="tex-span"><i>s</i></span>. The newspaper contains string <span class="tex-span"><i>t</i></span>, consisting of uppercase and lowercase English letters. We know that the length of string <span class="tex-span"><i>t</i></span> greater or equal to the length of the string <span class="tex-span"><i>s</i></span>.</p><p>The newspaper may possibly have too few of some letters needed to make the text and too many of some other letters. That's why Tanya wants to cut some <span class="tex-span"><i>n</i></span> letters out of the newspaper and make a message of length exactly <span class="tex-span"><i>n</i></span>, so that it looked as much as possible like <span class="tex-span"><i>s</i></span>. If the letter in some position has correct value and correct letter case (in the string <span class="tex-span"><i>s</i></span> and in the string that Tanya will make), then she shouts joyfully "<span class="tex-font-style-tt">YAY!</span>", and if the letter in the given position has only the correct value but it is in the wrong case, then the girl says "<span class="tex-font-style-tt">WHOOPS</span>".</p><p>Tanya wants to make such message that lets her shout "<span class="tex-font-style-tt">YAY!</span>" as much as possible. If there are multiple ways to do this, then her second priority is to maximize the number of times she says "<span class="tex-font-style-tt">WHOOPS</span>". Your task is to help Tanya make the message.</p></div><div class="input-specification"><p>The first line contains line <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 2·10<sup class="upper-index">5</sup></span>), consisting of uppercase and lowercase English letters — the text of Tanya's message.</p><p>The second line contains line <span class="tex-span"><i>t</i></span> (<span class="tex-span">|<i>s</i>| ≤ |<i>t</i>| ≤ 2·10<sup class="upper-index">5</sup></span>), consisting of uppercase and lowercase English letters — the text written in the newspaper.</p><p>Here <span class="tex-span">|<i>a</i>|</span> means the length of the string <span class="tex-span"><i>a</i></span>.</p></div><div class="output-specification"><p>Print two integers separated by a space:</p><ul> <li> the first number is the number of times Tanya shouts "<span class="tex-font-style-tt">YAY!</span>" while making the message, </li><li> the second number is the number of times Tanya says "<span class="tex-font-style-tt">WHOOPS</span>" while making the message. </li></ul></div>

## Input

<p>The first line contains line <span class="tex-span"><i>s</i></span> (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 2·10<sup class="upper-index">5</sup></span>), consisting of uppercase and lowercase English letters — the text of Tanya's message.</p><p>The second line contains line <span class="tex-span"><i>t</i></span> (<span class="tex-span">|<i>s</i>| ≤ |<i>t</i>| ≤ 2·10<sup class="upper-index">5</sup></span>), consisting of uppercase and lowercase English letters — the text written in the newspaper.</p><p>Here <span class="tex-span">|<i>a</i>|</span> means the length of the string <span class="tex-span"><i>a</i></span>.</p>

## Output

<p>Print two integers separated by a space:</p><ul> <li> the first number is the number of times Tanya shouts "<span class="tex-font-style-tt">YAY!</span>" while making the message, </li><li> the second number is the number of times Tanya says "<span class="tex-font-style-tt">WHOOPS</span>" while making the message. </li></ul>





```input1
AbC
DCbA

```




```input2
ABC
abc

```




```input3
abacaba
AbaCaBA

```




```output1
3 0

```




```output2
0 3

```




```output3
3 4

```


