## Description

<div><p>Friday is Polycarpus' favourite day of the week. Not because it is followed by the weekend, but because the lessons on Friday are 2 IT lessons, 2 math lessons and 2 literature lessons. Of course, Polycarpus has prepared to all of them, unlike his buddy Innocentius. Innocentius spent all evening playing his favourite game Fur2 and didn't have enough time to do the literature task. As Innocentius didn't want to get an F, he decided to do the task and read the book called "Storm and Calm" during the IT and Math lessons (he never used to have problems with these subjects). When the IT teacher Mr. Watkins saw this, he decided to give Innocentius another task so that the boy concentrated more on the lesson and less — on the staff that has nothing to do with IT. </p><p>Mr. Watkins said that a palindrome is a string that can be read the same way in either direction, from the left to the right and from the right to the left. A concatenation of strings <span class="tex-span"><i>a</i></span>, <span class="tex-span"><i>b</i></span> is a string <span class="tex-span"><i>ab</i></span> that results from consecutive adding of string <span class="tex-span"><i>b</i></span> to string <span class="tex-span"><i>a</i></span>. Of course, Innocentius knew it all but the task was much harder than he could have imagined. Mr. Watkins asked change in the "Storm and Calm" the minimum number of characters so that the text of the book would also be a concatenation of no more than <span class="tex-span"><i>k</i></span> palindromes. Innocentius can't complete the task and therefore asks you to help him.</p></div><div class="input-specification"><p>The first input line contains a non-empty string <span class="tex-span"><i>s</i></span> which is the text of "Storm and Calm" (without spaces). The length of the string <span class="tex-span"><i>s</i></span> does not exceed <span class="tex-span">500</span> characters. String <span class="tex-span"><i>s</i></span> consists of uppercase and lowercase Latin letters. The second line contains a single number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ |<i>s</i>|</span>, where <span class="tex-span">|<i>s</i>|</span> represents the length of the string <span class="tex-span"><i>s</i></span>).</p></div><div class="output-specification"><p>Print on the first line the minimum number of changes that Innocentius will have to make. Print on the second line the string consisting of no more than <span class="tex-span"><i>k</i></span> palindromes. Each palindrome should be non-empty and consist of uppercase and lowercase Latin letters. Use the character "<span class="tex-font-style-tt">+</span>" (ASCII-code 43) to separate consecutive palindromes. If there exist several solutions, print any of them.</p><p>The letters' case does matter, that is an uppercase letter is <span class="tex-font-style-bf">not</span> considered equivalent to the corresponding lowercase letter.</p></div>

## Input

<p>The first input line contains a non-empty string <span class="tex-span"><i>s</i></span> which is the text of "Storm and Calm" (without spaces). The length of the string <span class="tex-span"><i>s</i></span> does not exceed <span class="tex-span">500</span> characters. String <span class="tex-span"><i>s</i></span> consists of uppercase and lowercase Latin letters. The second line contains a single number <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>k</i> ≤ |<i>s</i>|</span>, where <span class="tex-span">|<i>s</i>|</span> represents the length of the string <span class="tex-span"><i>s</i></span>).</p>

## Output

<p>Print on the first line the minimum number of changes that Innocentius will have to make. Print on the second line the string consisting of no more than <span class="tex-span"><i>k</i></span> palindromes. Each palindrome should be non-empty and consist of uppercase and lowercase Latin letters. Use the character "<span class="tex-font-style-tt">+</span>" (ASCII-code 43) to separate consecutive palindromes. If there exist several solutions, print any of them.</p><p>The letters' case does matter, that is an uppercase letter is <span class="tex-font-style-bf">not</span> considered equivalent to the corresponding lowercase letter.</p>





```input1
abacaba
1

```




```input2
abdcaba
2

```




```input3
abdcaba
5

```




```input4
abacababababbcbabcd
3

```




```output1
0
abacaba

```




```output2
1
abdcdba

```




```output3
0
a+b+d+c+aba

```




```output4
1
abacaba+babab+bcbabcb

```


