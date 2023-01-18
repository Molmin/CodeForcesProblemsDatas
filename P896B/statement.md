## Description

<div><p><span class="tex-font-style-it">This is an interactive problem. Refer to the Interaction section below for better understanding.</span></p><p>Ithea and Chtholly want to play a game in order to determine who can use the kitchen tonight.</p><center><p><img class="tex-graphics" src="file://hs7m8A6U.png" style="max-width: 100.0%;max-height: 100.0%;"></p></center><p>Initially, Ithea puts <span class="tex-span"><i>n</i></span> clear sheets of paper in a line. They are numbered from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> from left to right.</p><p>This game will go on for <span class="tex-span"><i>m</i></span> rounds. In each round, Ithea will give Chtholly an integer between <span class="tex-span">1</span> and <span class="tex-span"><i>c</i></span>, and Chtholly needs to choose one of the sheets to write down this number (if there is already a number before, she will erase the original one and replace it with the new one).</p><p>Chtholly wins if, at any time, all the sheets are filled with a number and the <span class="tex-span"><i>n</i></span> numbers are in non-decreasing order looking from left to right from sheet <span class="tex-span">1</span> to sheet <span class="tex-span"><i>n</i></span>, and if after <span class="tex-span"><i>m</i></span> rounds she still doesn't win, she loses the game.</p><p>Chtholly really wants to win the game as she wants to cook something for Willem. But she doesn't know how to win the game. So Chtholly finds you, and your task is to write a program to receive numbers that Ithea gives Chtholly and help her make the decision on which sheet of paper write this number.</p></div><div class="input-specification"><p>The first line contains 3 integers <span class="tex-span"><i>n</i>, <i>m</i></span> and <span class="tex-span"><i>c</i></span> (<img align="middle" class="tex-formula" src="file://rKdBgqS0.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://BWyW9Ami.png" style="max-width: 100.0%;max-height: 100.0%;"> means <img align="middle" class="tex-formula" src="file://qbv53gsB.png" style="max-width: 100.0%;max-height: 100.0%;"> rounded up)&nbsp;— the number of sheets, the number of rounds and the largest possible number Ithea can give to Chtholly respectively. The remaining parts of input are given throughout the interaction process.</p></div><div><h2>Interaction</h2><p>In each round, your program needs to read one line containing a single integer <span class="tex-span"><i>p</i><sub class="lower-index"><i>i</i></sub></span> (<span class="tex-span">1 ≤ <i>p</i><sub class="lower-index"><i>i</i></sub> ≤ <i>c</i></span>), indicating the number given to Chtholly.</p><p>Your program should then output a line containing an integer between <span class="tex-span">1</span> and <span class="tex-span"><i>n</i></span>, indicating the number of sheet to write down this number in.</p><p><span class="tex-font-style-bf">After outputting each line, don't forget to flush the output.</span> For example: </p><ul> <li> <span class="tex-font-style-tt">fflush(stdout)</span> in C/C++; </li><li> <span class="tex-font-style-tt">System.out.flush()</span> in Java; </li><li> <span class="tex-font-style-tt">sys.stdout.flush()</span> in Python; </li><li> <span class="tex-font-style-tt">flush(output)</span> in Pascal; </li><li> See the documentation for other languages. </li></ul><p><span class="tex-font-style-bf">If Chtholly wins at the end of a round, no more input will become available and your program should terminate normally.</span> It can be shown that under the constraints, it's always possible for Chtholly to win the game.</p></div>

## Input

<p>The first line contains 3 integers <span class="tex-span"><i>n</i>, <i>m</i></span> and <span class="tex-span"><i>c</i></span> (<img align="middle" class="tex-formula" src="file://rKdBgqS0.png" style="max-width: 100.0%;max-height: 100.0%;">, <img align="middle" class="tex-formula" src="file://BWyW9Ami.png" style="max-width: 100.0%;max-height: 100.0%;"> means <img align="middle" class="tex-formula" src="file://qbv53gsB.png" style="max-width: 100.0%;max-height: 100.0%;"> rounded up)&nbsp;— the number of sheets, the number of rounds and the largest possible number Ithea can give to Chtholly respectively. The remaining parts of input are given throughout the interaction process.</p>





```input1
2 4 4
2
1
3

```




```output1
1
2
2

```



## Note

<p>In the example, Chtholly initially knew there were <span class="tex-span">2</span> sheets, <span class="tex-span">4</span> rounds and each number was between <span class="tex-span">1</span> and <span class="tex-span">4</span>. She then received a <span class="tex-span">2</span> and decided to write it in the <span class="tex-span">1</span>st sheet. Then she received a <span class="tex-span">1</span> and wrote it in the <span class="tex-span">2</span>nd sheet. At last, she received a <span class="tex-span">3</span> and replaced <span class="tex-span">1</span> with <span class="tex-span">3</span> in the <span class="tex-span">2</span>nd sheet. At this time all the sheets were filled with a number and they were non-decreasing, so she won the game. </p><p><span class="tex-font-style-bf">Note that it is required that your program terminate immediately after Chtholly wins and do not read numbers from the input for the remaining rounds. If not, undefined behaviour may arise and it won't be sure whether your program will be accepted or rejected. Also because of this, please be careful when hacking others' codes.</span> In the sample, Chtholly won the game after the <span class="tex-span">3</span>rd round, so it is required that your program doesn't read the number of the remaining <span class="tex-span">4</span>th round.</p><p>The input format for hacking: </p><ul> <li> The first line contains 3 integers <span class="tex-span"><i>n</i>, <i>m</i></span> and <span class="tex-span"><i>c</i></span>; </li><li> The following <span class="tex-span"><i>m</i></span> lines each contains an integer between <span class="tex-span">1</span> and <span class="tex-span"><i>c</i></span>, indicating the number given to Chtholly in each round. </li></ul>
