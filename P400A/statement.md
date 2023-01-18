## Description

<div><p>There always is something to choose from! And now, instead of "Noughts and Crosses", Inna choose a very unusual upgrade of this game. The rules of the game are given below:</p><p>There is one person playing the game. Before the beginning of the game he puts 12 cards in a row on the table. Each card contains a character: "<span class="tex-font-style-tt">X</span>" or "<span class="tex-font-style-tt">O</span>". Then the player chooses two positive integers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> <span class="tex-span">(<i>a</i>·<i>b</i> = 12)</span>, after that he makes a table of size <span class="tex-span"><i>a</i> × <i>b</i></span> from the cards he put on the table as follows: the first <span class="tex-span"><i>b</i></span> cards form the first row of the table, the second <span class="tex-span"><i>b</i></span> cards form the second row of the table and so on, the last <span class="tex-span"><i>b</i></span> cards form the last (number <span class="tex-span"><i>a</i></span>) row of the table. The player wins if some column of the table contain characters "<span class="tex-font-style-tt">X</span>" on all cards. Otherwise, the player loses.</p><p>Inna has already put 12 cards on the table in a row. But unfortunately, she doesn't know what numbers <span class="tex-span"><i>a</i></span> and <span class="tex-span"><i>b</i></span> to choose. Help her win the game: print to her all the possible ways of numbers <span class="tex-span"><i>a</i>, <i>b</i></span> that she can choose and win.</p></div><div class="input-specification"><p>The first line of the input contains integer <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 100)</span>. This value shows the number of sets of test data in the input. Next follows the description of each of the <span class="tex-span"><i>t</i></span> tests on a separate line.</p><p>The description of each test is a string consisting of 12 characters, each character is either "<span class="tex-font-style-tt">X</span>", or "<span class="tex-font-style-tt">O</span>". The <span class="tex-span"><i>i</i></span>-th character of the string shows the character that is written on the <span class="tex-span"><i>i</i></span>-th card from the start.</p></div><div class="output-specification"><p>For each test, print the answer to the test on a single line. The first number in the line must represent the number of distinct ways to choose the pair <span class="tex-span"><i>a</i>, <i>b</i></span>. Next, print on this line the pairs in the format <span class="tex-font-style-tt"><span class="tex-span"><i>a</i></span>x<span class="tex-span"><i>b</i></span></span>. Print the pairs in the order of increasing first parameter (<span class="tex-span"><i>a</i></span>). Separate the pairs in the line by whitespaces.</p></div>

## Input

<p>The first line of the input contains integer <span class="tex-span"><i>t</i></span> <span class="tex-span">(1 ≤ <i>t</i> ≤ 100)</span>. This value shows the number of sets of test data in the input. Next follows the description of each of the <span class="tex-span"><i>t</i></span> tests on a separate line.</p><p>The description of each test is a string consisting of 12 characters, each character is either "<span class="tex-font-style-tt">X</span>", or "<span class="tex-font-style-tt">O</span>". The <span class="tex-span"><i>i</i></span>-th character of the string shows the character that is written on the <span class="tex-span"><i>i</i></span>-th card from the start.</p>

## Output

<p>For each test, print the answer to the test on a single line. The first number in the line must represent the number of distinct ways to choose the pair <span class="tex-span"><i>a</i>, <i>b</i></span>. Next, print on this line the pairs in the format <span class="tex-font-style-tt"><span class="tex-span"><i>a</i></span>x<span class="tex-span"><i>b</i></span></span>. Print the pairs in the order of increasing first parameter (<span class="tex-span"><i>a</i></span>). Separate the pairs in the line by whitespaces.</p>





```input1
4
OXXXOXOOXOOX
OXOXOXOXOXOX
XXXXXXXXXXXX
OOOOOOOOOOOO

```




```output1
3 1x12 2x6 4x3
4 1x12 2x6 3x4 6x2
6 1x12 2x6 3x4 4x3 6x2 12x1
0

```


