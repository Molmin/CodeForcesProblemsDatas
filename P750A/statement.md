## Description

<div><p>Limak is going to participate in a contest on the last day of the 2016. The contest will start at 20:00 and will last four hours, exactly until midnight. There will be <span class="tex-span"><i>n</i></span> problems, sorted by difficulty, i.e. problem <span class="tex-span">1</span> is the easiest and problem <span class="tex-span"><i>n</i></span> is the hardest. Limak knows it will take him <span class="tex-span">5·<i>i</i></span> minutes to solve the <span class="tex-span"><i>i</i></span>-th problem.</p><p>Limak's friends organize a New Year's Eve party and Limak wants to be there at midnight or earlier. He needs <span class="tex-span"><i>k</i></span> minutes to get there from his house, where he will participate in the contest first.</p><p>How many problems can Limak solve if he wants to make it to the party?</p></div><div class="input-specification"><p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 240</span>)&nbsp;— the number of the problems in the contest and the number of minutes Limak needs to get to the party from his house.</p></div><div class="output-specification"><p>Print one integer, denoting the maximum possible number of problems Limak can solve so that he could get to the party at midnight or earlier.</p></div>

## Input

<p>The only line of the input contains two integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>, <span class="tex-span">1 ≤ <i>k</i> ≤ 240</span>)&nbsp;— the number of the problems in the contest and the number of minutes Limak needs to get to the party from his house.</p>

## Output

<p>Print one integer, denoting the maximum possible number of problems Limak can solve so that he could get to the party at midnight or earlier.</p>





```input1
3 222

```




```input2
4 190

```




```input3
7 1

```




```output1
2

```




```output2
4

```




```output3
7

```



## Note

<p>In the first sample, there are <span class="tex-span">3</span> problems and Limak needs <span class="tex-span">222</span> minutes to get to the party. The three problems require <span class="tex-span">5</span>, <span class="tex-span">10</span> and <span class="tex-span">15</span> minutes respectively. Limak can spend <span class="tex-span">5 + 10 = 15</span> minutes to solve first two problems. Then, at 20:15 he can leave his house to get to the party at 23:57 (after <span class="tex-span">222</span> minutes). In this scenario Limak would solve <span class="tex-span">2</span> problems. He doesn't have enough time to solve <span class="tex-span">3</span> problems so the answer is <span class="tex-span">2</span>.</p><p>In the second sample, Limak can solve all <span class="tex-span">4</span> problems in <span class="tex-span">5 + 10 + 15 + 20 = 50</span> minutes. At 20:50 he will leave the house and go to the party. He will get there exactly at midnight.</p><p>In the third sample, Limak needs only <span class="tex-span">1</span> minute to get to the party. He has enough time to solve all <span class="tex-span">7</span> problems.</p>
