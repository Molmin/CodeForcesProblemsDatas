## Description

<div><p><span class="tex-font-style-it">The only difference from the previous problem is the constraint on the number of requests. In this problem your program should guess the answer doing at most 7 requests.</span></p><p>This problem is a little bit unusual. Here you are to implement an interaction with a testing system. That means that you can make queries and get responses in the online mode. Please be sure to use the stream flushing operation after each query's output in order not to leave part of your output in some buffer. For example, in C++ you've got to use the <span class="tex-font-style-tt">fflush(stdout)</span> function, in Java — call <span class="tex-font-style-tt">System.out.flush()</span>, and in Pascal — <span class="tex-font-style-tt">flush(output)</span>.</p><p>Bulls and Cows (also known as Cows and Bulls or Pigs and Bulls or Bulls and Cleots) is an old code-breaking paper and pencil game for two players, predating the similar commercially marketed board game Mastermind.</p><p>On a sheet of paper, the first player thinks a secret string. This string consists only of digits and has the length <span class="tex-span">4</span>. The digits in the string <span class="tex-font-style-bf">must</span> be all different, no two or more equal digits are allowed.</p><p>Then the second player tries to guess his opponent's string. For every guess the first player gives the number of matches. If the matching digits are on their right positions, they are "bulls", if on different positions, they are "cows". Thus a response is a pair of numbers — the number of "bulls" and the number of "cows". A try can contain equal digits.</p><p>More formally, let's the secret string is <span class="tex-span"><i>s</i></span> and the second player are trying to guess it with a string <span class="tex-span"><i>x</i></span>. The number of "bulls" is a number of such positions <span class="tex-span"><i>i</i></span> (<span class="tex-span">1 ≤ <i>i</i> ≤ 4</span>) where <span class="tex-span"><i>s</i>[<i>i</i>] = <i>x</i>[<i>i</i>]</span>. The number of "cows" is a number of such digits <span class="tex-span"><i>c</i></span> that <span class="tex-span"><i>s</i></span> contains <span class="tex-span"><i>c</i></span> in the position <span class="tex-span"><i>i</i></span> (i.e. <span class="tex-span"><i>s</i>[<i>i</i>] = <i>c</i></span>), <span class="tex-span"><i>x</i></span> contains <span class="tex-span"><i>c</i></span>, but <span class="tex-span"><i>x</i>[<i>i</i>] ≠ <i>c</i></span>.</p><p>For example, the secret string is "<span class="tex-font-style-tt">0427</span>", the opponent's try is "<span class="tex-font-style-tt">0724</span>", then the answer is <span class="tex-span">2</span> bulls and <span class="tex-span">2</span> cows (the bulls are "0" and "2", the cows are "4" and "7"). If the secret string is "<span class="tex-font-style-tt">0123</span>", the opponent's try is "<span class="tex-font-style-tt">0330</span>", then the answer is <span class="tex-span">1</span> bull and <span class="tex-span">1</span> cow.</p><p>In this problem you are to guess the string <span class="tex-span"><i>s</i></span> that the system has chosen. You only know that the chosen string consists of <span class="tex-span">4</span> distinct digits.</p><p>You can make queries to the testing system, each query is the output of a single <span class="tex-span">4</span>-digit string. The answer to the query is the number of bulls and number of cows. If the system's response equals "4 0", that means the interaction with your problem is over and the program must terminate. That is possible for two reasons — the program either guessed the number <span class="tex-span"><i>x</i></span> or made an invalid action (for example, printed letters instead of digits).</p><p><span class="tex-font-style-bf">Your program is allowed to do at most <span class="tex-span">7</span> queries.</span></p><p>You can hack solutions of other participants providing a 4-digit string containing distinct digits — the secret string.</p></div><div class="input-specification"><p>To read answers to the queries, the program must use the standard input.</p><p>The program will receive pairs of non-negative integers in the input, one pair per line. The first number in a pair is a number of bulls and the second one is a number of cows of the string <span class="tex-span"><i>s</i></span> and the string <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> printed by your program. If the system response equals "4 0", then your solution should terminate.</p><p>The testing system will let your program read the <span class="tex-span"><i>i</i></span>-th pair of integers from the input only after your program displays the corresponding system query in the output: prints value <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> in a single line and executes operation <span class="tex-font-style-tt">flush</span>.</p></div><div class="output-specification"><p>The program must use the standard output to print queries.</p><p>Your program must output requests — <span class="tex-span">4</span>-digit strings <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ...</span>, one per line. After the output of each line the program must execute <span class="tex-font-style-tt">flush</span> operation. The program should read the answer to the query from the standard input.</p><p><span class="tex-font-style-bf">Your program is allowed to do at most <span class="tex-span">7</span> queries.</span></p></div>

## Input

<p>To read answers to the queries, the program must use the standard input.</p><p>The program will receive pairs of non-negative integers in the input, one pair per line. The first number in a pair is a number of bulls and the second one is a number of cows of the string <span class="tex-span"><i>s</i></span> and the string <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> printed by your program. If the system response equals "4 0", then your solution should terminate.</p><p>The testing system will let your program read the <span class="tex-span"><i>i</i></span>-th pair of integers from the input only after your program displays the corresponding system query in the output: prints value <span class="tex-span"><i>x</i><sub class="lower-index"><i>i</i></sub></span> in a single line and executes operation <span class="tex-font-style-tt">flush</span>.</p>

## Output

<p>The program must use the standard output to print queries.</p><p>Your program must output requests — <span class="tex-span">4</span>-digit strings <span class="tex-span"><i>x</i><sub class="lower-index">1</sub>, <i>x</i><sub class="lower-index">2</sub>, ...</span>, one per line. After the output of each line the program must execute <span class="tex-font-style-tt">flush</span> operation. The program should read the answer to the query from the standard input.</p><p><span class="tex-font-style-bf">Your program is allowed to do at most <span class="tex-span">7</span> queries.</span></p>





```input1
0 1
2 0
1 1
0 4
2 1
4 0

```




```output1
8000
0179
3159
3210
0112
0123
```



## Note

<p>The secret string <span class="tex-span"><i>s</i></span> in the example is "<span class="tex-font-style-tt">0123</span>".</p>
