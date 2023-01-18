## Description

<div><p>Vasily has recently learned about the amazing properties of number <span class="tex-span">π</span>. In one of the articles it has been hypothesized that, whatever the sequence of numbers we have, in some position, this sequence is found among the digits of number <span class="tex-span">π</span>. Thus, if you take, for example, the epic novel "War and Peace" of famous Russian author Leo Tolstoy, and encode it with numbers, then we will find the novel among the characters of number <span class="tex-span">π</span>.</p><p>Vasily was absolutely delighted with this, because it means that all the books, songs and programs have already been written and encoded in the digits of <span class="tex-span">π</span>. Vasily is, of course, a bit wary that this is only a hypothesis and it hasn't been proved, so he decided to check it out.</p><p>To do this, Vasily downloaded from the Internet the archive with the sequence of digits of number <span class="tex-span">π</span>, starting with a certain position, and began to check the different strings of digits on the presence in the downloaded archive. Vasily quickly found short strings of digits, but each time he took a longer string, it turned out that it is not in the archive. Vasily came up with a definition that a string of length <span class="tex-span"><i>d</i></span> is a <span class="tex-font-style-it">half-occurrence</span> if it contains a substring of length of at least <img align="middle" class="tex-formula" src="file://oUyY8hb6.png" style="max-width: 100.0%;max-height: 100.0%;">, which occurs in the archive.</p><p>To complete the investigation, Vasily took <span class="tex-span">2</span> large numbers <span class="tex-span"><i>x</i>, <i>y</i></span> (<span class="tex-span"><i>x</i> ≤ <i>y</i></span>) with the same number of digits and now he wants to find the number of numbers in the interval from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span>, which are <span class="tex-font-style-it">half-occurrences</span> in the archive. Help Vasily calculate this value modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div><div class="input-specification"><p>The first line contains string <span class="tex-span"><i>s</i></span> consisting of decimal digits (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 1000</span>) that Vasily will use to search substrings in. According to hypothesis, this sequence of digis indeed occurs in the decimal representation of <span class="tex-span">π</span>, although we can't guarantee that.</p><p>The second and third lines contain two positive integers <span class="tex-span"><i>x</i>, <i>y</i></span> of the same length <span class="tex-span"><i>d</i></span> (<span class="tex-span"><i>x</i> ≤ <i>y</i></span>, <span class="tex-span">2 ≤ <i>d</i> ≤ 50</span>). Numbers <span class="tex-span"><i>x</i>, <i>y</i></span> do not contain leading zeroes.</p></div><div class="output-specification"><p>Print how many numbers in the segment from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span> that are half-occurrences in <span class="tex-span"><i>s</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p></div>

## Input

<p>The first line contains string <span class="tex-span"><i>s</i></span> consisting of decimal digits (<span class="tex-span">1 ≤ |<i>s</i>| ≤ 1000</span>) that Vasily will use to search substrings in. According to hypothesis, this sequence of digis indeed occurs in the decimal representation of <span class="tex-span">π</span>, although we can't guarantee that.</p><p>The second and third lines contain two positive integers <span class="tex-span"><i>x</i>, <i>y</i></span> of the same length <span class="tex-span"><i>d</i></span> (<span class="tex-span"><i>x</i> ≤ <i>y</i></span>, <span class="tex-span">2 ≤ <i>d</i> ≤ 50</span>). Numbers <span class="tex-span"><i>x</i>, <i>y</i></span> do not contain leading zeroes.</p>

## Output

<p>Print how many numbers in the segment from <span class="tex-span"><i>x</i></span> to <span class="tex-span"><i>y</i></span> that are half-occurrences in <span class="tex-span"><i>s</i></span> modulo <span class="tex-span">10<sup class="upper-index">9</sup> + 7</span>.</p>





```input1
02
10
19

```




```input2
023456789
10
19

```




```input3
31415926535
10
29

```




```output1
2

```




```output2
9

```




```output3
20

```


