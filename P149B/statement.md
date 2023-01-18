## Description

<div><p>Having stayed home alone, Petya decided to watch forbidden films on the Net in secret. "What ungentlemanly behavior!" — you can say that, of course, but don't be too harsh on the kid. In his country films about the Martians and other extraterrestrial civilizations are forbidden. It was very unfair to Petya as he adored adventure stories that featured lasers and robots. </p><p>Today Petya is watching a shocking blockbuster about the Martians called "R2:D2". What can "R2:D2" possibly mean? It might be the Martian time represented in the Martian numeral system. Petya knows that time on Mars is counted just like on the Earth (that is, there are <span class="tex-span">24</span> hours and each hour has <span class="tex-span">60</span> minutes). The time is written as "<span class="tex-span"><i>a</i></span><span class="tex-font-style-tt">:</span><span class="tex-span"><i>b</i></span>", where the string <span class="tex-span"><i>a</i></span> stands for the number of hours (from <span class="tex-span">0</span> to <span class="tex-span">23</span> inclusive), and string <span class="tex-span"><i>b</i></span> stands for the number of minutes (from <span class="tex-span">0</span> to <span class="tex-span">59</span> inclusive). The only thing Petya doesn't know is in what numeral system the Martian time is written.</p><p>Your task is to print the radixes of all numeral system which can contain the time "<span class="tex-span"><i>a</i></span><span class="tex-font-style-tt">:</span><span class="tex-span"><i>b</i></span>".</p></div><div class="input-specification"><p>The first line contains a single string as "<span class="tex-span"><i>a</i></span><span class="tex-font-style-tt">:</span><span class="tex-span"><i>b</i></span>" (without the quotes). There <span class="tex-span"><i>a</i></span> is a non-empty string, consisting of numbers and uppercase Latin letters. String <span class="tex-span"><i>a</i></span> shows the number of hours. String <span class="tex-span"><i>b</i></span> is a non-empty string that consists of numbers and uppercase Latin letters. String <span class="tex-span"><i>b</i></span> shows the number of minutes. The lengths of strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are from <span class="tex-span">1</span> to <span class="tex-span">5</span> characters, inclusive. Please note that strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> can have leading zeroes that do not influence the result in any way (for example, string "<span class="tex-font-style-tt">008:1</span>" in decimal notation denotes correctly written time).</p><p>We consider characters <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, ..., <span class="tex-font-style-tt">9</span> as denoting the corresponding digits of the number's representation in some numeral system, and characters <span class="tex-font-style-tt">A</span>, <span class="tex-font-style-tt">B</span>, ..., <span class="tex-font-style-tt">Z</span> correspond to numbers <span class="tex-font-style-tt">10</span>, <span class="tex-font-style-tt">11</span>, ..., <span class="tex-font-style-tt">35</span>.</p></div><div class="output-specification"><p>Print the radixes of the numeral systems that can represent the time "<span class="tex-span"><i>a</i></span><span class="tex-font-style-tt">:</span><span class="tex-span"><i>b</i></span>" in the increasing order. Separate the numbers with spaces or line breaks. If there is no numeral system that can represent time "<span class="tex-span"><i>a</i></span><span class="tex-font-style-tt">:</span><span class="tex-span"><i>b</i></span>", print the single integer <span class="tex-font-style-tt">0</span>. If there are infinitely many numeral systems that can represent the time "<span class="tex-span"><i>a</i></span><span class="tex-font-style-tt">:</span><span class="tex-span"><i>b</i></span>", print the single integer <span class="tex-font-style-tt">-1</span>.</p><p>Note that on Mars any positional numeral systems with positive radix strictly larger than one are possible.</p></div>

## Input

<p>The first line contains a single string as "<span class="tex-span"><i>a</i></span><span class="tex-font-style-tt">:</span><span class="tex-span"><i>b</i></span>" (without the quotes). There <span class="tex-span"><i>a</i></span> is a non-empty string, consisting of numbers and uppercase Latin letters. String <span class="tex-span"><i>a</i></span> shows the number of hours. String <span class="tex-span"><i>b</i></span> is a non-empty string that consists of numbers and uppercase Latin letters. String <span class="tex-span"><i>b</i></span> shows the number of minutes. The lengths of strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> are from <span class="tex-span">1</span> to <span class="tex-span">5</span> characters, inclusive. Please note that strings <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> can have leading zeroes that do not influence the result in any way (for example, string "<span class="tex-font-style-tt">008:1</span>" in decimal notation denotes correctly written time).</p><p>We consider characters <span class="tex-font-style-tt">0</span>, <span class="tex-font-style-tt">1</span>, ..., <span class="tex-font-style-tt">9</span> as denoting the corresponding digits of the number's representation in some numeral system, and characters <span class="tex-font-style-tt">A</span>, <span class="tex-font-style-tt">B</span>, ..., <span class="tex-font-style-tt">Z</span> correspond to numbers <span class="tex-font-style-tt">10</span>, <span class="tex-font-style-tt">11</span>, ..., <span class="tex-font-style-tt">35</span>.</p>

## Output

<p>Print the radixes of the numeral systems that can represent the time "<span class="tex-span"><i>a</i></span><span class="tex-font-style-tt">:</span><span class="tex-span"><i>b</i></span>" in the increasing order. Separate the numbers with spaces or line breaks. If there is no numeral system that can represent time "<span class="tex-span"><i>a</i></span><span class="tex-font-style-tt">:</span><span class="tex-span"><i>b</i></span>", print the single integer <span class="tex-font-style-tt">0</span>. If there are infinitely many numeral systems that can represent the time "<span class="tex-span"><i>a</i></span><span class="tex-font-style-tt">:</span><span class="tex-span"><i>b</i></span>", print the single integer <span class="tex-font-style-tt">-1</span>.</p><p>Note that on Mars any positional numeral systems with positive radix strictly larger than one are possible.</p>





```input1
11:20

```




```input2
2A:13

```




```input3
000B:00001

```




```output1
3 4 5 6 7 8 9 10 11 12 13 14 15 16 17 18 19 20 21 22
```




```output2
0

```




```output3
-1

```



## Note

<p>Let's consider the first sample. String "<span class="tex-font-style-tt">11:20</span>" can be perceived, for example, as time <span class="tex-font-style-tt">4:6</span>, represented in the ternary numeral system or as time <span class="tex-font-style-tt">17:32</span> in hexadecimal system. </p><p>Let's consider the second sample test. String "<span class="tex-font-style-tt">2A:13</span>" can't be perceived as correct time in any notation. For example, let's take the base-11 numeral notation. There the given string represents time <span class="tex-font-style-tt">32:14</span> that isn't a correct time.</p><p>Let's consider the third sample. String "<span class="tex-font-style-tt">000B:00001</span>" can be perceived as a correct time in the infinite number of numeral systems. If you need an example, you can take any numeral system with radix no less than <span class="tex-font-style-tt">12</span>.</p>
