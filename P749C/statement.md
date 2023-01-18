## Description

<div><p>There are <span class="tex-span"><i>n</i></span> employees in Alternative Cake Manufacturing (ACM). They are now voting on some very important question and the leading world media are trying to predict the outcome of the vote.</p><p>Each of the employees belongs to one of two fractions: depublicans or remocrats, and these two fractions have opposite opinions on what should be the outcome of the vote. The voting procedure is rather complicated: </p><ol> <li> Each of <span class="tex-span"><i>n</i></span> employees makes a statement. They make statements one by one starting from employees <span class="tex-span">1</span> and finishing with employee <span class="tex-span"><i>n</i></span>. If at the moment when it's time for the <span class="tex-span"><i>i</i></span>-th employee to make a statement he no longer has the right to vote, he just skips his turn (and no longer takes part in this voting). </li><li> When employee makes a statement, he can do nothing or declare that one of the other employees no longer has a right to vote. It's allowed to deny from voting people who already made the statement or people who are only waiting to do so. If someone is denied from voting he no longer participates in the voting till the very end. </li><li> When all employees are done with their statements, the procedure repeats: again, each employees starting from <span class="tex-span">1</span> and finishing with <span class="tex-span"><i>n</i></span> who are still eligible to vote make their statements. </li><li> The process repeats until there is only one employee eligible to vote remaining and he determines the outcome of the whole voting. Of course, he votes for the decision suitable for his fraction. </li></ol><p>You know the order employees are going to vote and that they behave optimal (and they also know the order and who belongs to which fraction). Predict the outcome of the vote.</p></div><div class="input-specification"><p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of employees. </p><p>The next line contains <span class="tex-span"><i>n</i></span> characters. The <span class="tex-span"><i>i</i></span>-th character is '<span class="tex-font-style-tt">D</span>' if the <span class="tex-span"><i>i</i></span>-th employee is from depublicans fraction or '<span class="tex-font-style-tt">R</span>' if he is from remocrats.</p></div><div class="output-specification"><p>Print '<span class="tex-font-style-tt">D</span>' if the outcome of the vote will be suitable for depublicans and '<span class="tex-font-style-tt">R</span>' if remocrats will win.</p></div>

## Input

<p>The first line of the input contains a single integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of employees. </p><p>The next line contains <span class="tex-span"><i>n</i></span> characters. The <span class="tex-span"><i>i</i></span>-th character is '<span class="tex-font-style-tt">D</span>' if the <span class="tex-span"><i>i</i></span>-th employee is from depublicans fraction or '<span class="tex-font-style-tt">R</span>' if he is from remocrats.</p>

## Output

<p>Print '<span class="tex-font-style-tt">D</span>' if the outcome of the vote will be suitable for depublicans and '<span class="tex-font-style-tt">R</span>' if remocrats will win.</p>





```input1
5
DDRRR

```




```input2
6
DDRRRR

```




```output1
D

```




```output2
R

```



## Note

<p>Consider one of the voting scenarios for the first sample: </p><ol> <li> Employee <span class="tex-span">1</span> denies employee <span class="tex-span">5</span> to vote. </li><li> Employee <span class="tex-span">2</span> denies employee <span class="tex-span">3</span> to vote. </li><li> Employee <span class="tex-span">3</span> has no right to vote and skips his turn (he was denied by employee <span class="tex-span">2</span>). </li><li> Employee <span class="tex-span">4</span> denies employee <span class="tex-span">2</span> to vote. </li><li> Employee <span class="tex-span">5</span> has no right to vote and skips his turn (he was denied by employee <span class="tex-span">1</span>). </li><li> Employee <span class="tex-span">1</span> denies employee <span class="tex-span">4</span>. </li><li> Only employee <span class="tex-span">1</span> now has the right to vote so the voting ends with the victory of depublicans. </li></ol>
