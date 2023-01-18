## Description

<div><p>The History of Magic is perhaps the most boring subject in the Hogwarts school of Witchcraft and Wizardry. Harry Potter is usually asleep during history lessons, and his magical quill writes the lectures for him. Professor Binns, the history of magic teacher, lectures in such a boring and monotonous voice, that he has a soporific effect even on the quill. That's why the quill often makes mistakes, especially in dates.</p><p>So, at the end of the semester Professor Binns decided to collect the students' parchments with notes and check them. Ron Weasley is in a panic: Harry's notes may contain errors, but at least he has some notes, whereas Ron does not have any. Ronald also has been sleeping during the lectures and his quill had been eaten by his rat Scabbers. Hermione Granger refused to give Ron her notes, because, in her opinion, everyone should learn on their own. Therefore, Ron has no choice but to copy Harry's notes.</p><p>Due to the quill's errors Harry's dates are absolutely confused: the years of goblin rebellions and other important events for the wizarding world do not follow in order, and sometimes even dates from the future occur. Now Ron wants to change some of the digits while he copies the notes so that the dates were in the chronological (i.e. non-decreasing) order and so that the notes did not have any dates strictly later than <span class="tex-span">2011</span>, or strictly before than <span class="tex-span">1000</span>. To make the resulting sequence as close as possible to the one dictated by Professor Binns, Ron will change no more than one digit in each date into other digit. Help him do it.</p></div><div class="input-specification"><p>The first input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). It represents the number of dates in Harry's notes. Next <span class="tex-span"><i>n</i></span> lines contain the actual dates <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>y</i><sub class="lower-index"><i>n</i></sub></span>, each line contains a date. Each date is a four-digit integer (<span class="tex-span">1000 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 9999</span>).</p></div><div class="output-specification"><p>Print <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>z</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>z</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1000 ≤ <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ 2011</span>). They are Ron's resulting dates. Print each number on a single line. Numbers <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> must form the non-decreasing sequence. Each number <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> should differ from the corresponding date <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> in no more than one digit. It is not allowed to change the first digit of a number into <span class="tex-span">0</span>. If there are several possible solutions, print any of them. If there's no solution, print "No solution" (without the quotes).</p></div>

## Input

<p>The first input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span>). It represents the number of dates in Harry's notes. Next <span class="tex-span"><i>n</i></span> lines contain the actual dates <span class="tex-span"><i>y</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>y</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>y</i><sub class="lower-index"><i>n</i></sub></span>, each line contains a date. Each date is a four-digit integer (<span class="tex-span">1000 ≤ <i>y</i><sub class="lower-index"><i>i</i></sub> ≤ 9999</span>).</p>

## Output

<p>Print <span class="tex-span"><i>n</i></span> numbers <span class="tex-span"><i>z</i><sub class="lower-index">1</sub></span>, <span class="tex-span"><i>z</i><sub class="lower-index">2</sub></span>, ..., <span class="tex-span"><i>z</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1000 ≤ <i>z</i><sub class="lower-index"><i>i</i></sub> ≤ 2011</span>). They are Ron's resulting dates. Print each number on a single line. Numbers <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> must form the non-decreasing sequence. Each number <span class="tex-span"><i>z</i><sub class="lower-index"><i>i</i></sub></span> should differ from the corresponding date <span class="tex-span"><i>y</i><sub class="lower-index"><i>i</i></sub></span> in no more than one digit. It is not allowed to change the first digit of a number into <span class="tex-span">0</span>. If there are several possible solutions, print any of them. If there's no solution, print "No solution" (without the quotes).</p>





```input1
3
1875
1936
1721

```




```input2
4
9999
2000
3000
3011

```




```input3
3
1999
5055
2000

```




```output1
1835
1836
1921

```




```output2
1999
2000
2000
2011

```




```output3
No solution

```


