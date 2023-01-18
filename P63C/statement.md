## Description

<div><p>The "Bulls and Cows" game needs two people to play. The thinker thinks of a number and the guesser tries to guess it.</p><p>The thinker thinks of a four-digit number in the decimal system. All the digits in the number are different and the number may have a leading zero. It can't have more than one leading zero, because all it's digits should be different. The guesser tries to guess the number. He makes a series of guesses, trying experimental numbers and receives answers from the first person in the format "<span class="tex-span"><i>x</i></span> bulls <span class="tex-span"><i>y</i></span> cows". <span class="tex-span"><i>x</i></span> represents the number of digits in the experimental number that occupy the same positions as in the sought number. <span class="tex-span"><i>y</i></span> represents the number of digits of the experimental number that present in the sought number, but occupy different positions. Naturally, the experimental numbers, as well as the sought number, are represented by four-digit numbers where all digits are different and a leading zero can be present.</p><p>For example, let's suppose that the thinker thought of the number <span class="tex-font-style-tt">0123</span>. Then the guessers' experimental number <span class="tex-font-style-tt">1263</span> will receive a reply "1 bull 2 cows" (3 occupies the same positions in both numbers and 1 and 2 are present in both numbers but they occupy different positions). Also, the answer to number <span class="tex-font-style-tt">8103</span> will be "2 bulls 1 cow" (analogically, 1 and 3 occupy the same positions and 0 occupies a different one). </p><p>When the guesser is answered "4 bulls 0 cows", the game is over.</p><p>Now the guesser has already made several guesses and wants to know whether his next guess can possibly be the last one.</p></div><div class="input-specification"><p>The first input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>) which represents the number of already made guesses. Then follow <span class="tex-span"><i>n</i></span> lines in the form of "<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th experimental number, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number of bulls, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the number of cows (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> + <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 4</span>). The experimental numbers are correct, i.e., each of them contains exactly four digits, in each of them all the four digits are different, and there can be a leading zero. All the experimental numbers are different. As the guesser hasn't guessed the number yet, the answer "4 bulls 0 cows" is not present.</p></div><div class="output-specification"><p>If the input data is enough to determine the sought number, print the number with four digits on a single line. If it has less than four digits, add leading zero. If the data is not enough, print "<span class="tex-font-style-tt">Need more data</span>" without the quotes. If the thinker happens to have made a mistake in his replies, print "<span class="tex-font-style-tt">Incorrect data</span>" without the quotes.</p></div>

## Input

<p>The first input line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>) which represents the number of already made guesses. Then follow <span class="tex-span"><i>n</i></span> lines in the form of "<span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span>", where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the <span class="tex-span"><i>i</i></span>-th experimental number, <span class="tex-span"><i>b</i><sub class="lower-index"><i>i</i></sub></span> is the number of bulls, <span class="tex-span"><i>c</i><sub class="lower-index"><i>i</i></sub></span> is the number of cows (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>, <span class="tex-span">0 ≤ <i>b</i><sub class="lower-index"><i>i</i></sub>, <i>c</i><sub class="lower-index"><i>i</i></sub>, <i>b</i><sub class="lower-index"><i>i</i></sub> + <i>c</i><sub class="lower-index"><i>i</i></sub> ≤ 4</span>). The experimental numbers are correct, i.e., each of them contains exactly four digits, in each of them all the four digits are different, and there can be a leading zero. All the experimental numbers are different. As the guesser hasn't guessed the number yet, the answer "4 bulls 0 cows" is not present.</p>

## Output

<p>If the input data is enough to determine the sought number, print the number with four digits on a single line. If it has less than four digits, add leading zero. If the data is not enough, print "<span class="tex-font-style-tt">Need more data</span>" without the quotes. If the thinker happens to have made a mistake in his replies, print "<span class="tex-font-style-tt">Incorrect data</span>" without the quotes.</p>





```input1
2
1263 1 2
8103 2 1

```




```input2
2
1234 2 2
1256 0 2

```




```input3
2
0123 1 1
4567 1 2

```




```output1
Need more data
```




```output2
2134
```




```output3
Incorrect data
```


