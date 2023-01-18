## Description

<div><p>The king Copa often has been reported about the Codeforces site, which is rapidly getting more and more popular among the brightest minds of the humanity, who are using it for training and competing. Recently Copa understood that to conquer the world he needs to organize the world Codeforces tournament. He hopes that after it the brightest minds will become his subordinates, and the toughest part of conquering the world will be completed.</p><p>The final round of the Codeforces World Finals 20YY is scheduled for <span class="tex-span"><i>DD</i></span>.<span class="tex-span"><i>MM</i></span>.<span class="tex-span"><i>YY</i></span>, where <span class="tex-span"><i>DD</i></span> is the day of the round, <span class="tex-span"><i>MM</i></span> is the month and <span class="tex-span"><i>YY</i></span> are the last two digits of the year. Bob is lucky to be the first finalist form Berland. But there is one problem: according to the rules of the competition, all participants must be at least 18 years old at the moment of the finals. Bob was born on <span class="tex-span"><i>BD</i></span>.<span class="tex-span"><i>BM</i></span>.<span class="tex-span"><i>BY</i></span>. This date is recorded in his passport, the copy of which he has already mailed to the organizers. But Bob learned that in different countries the way, in which the dates are written, differs. For example, in the US the month is written first, then the day and finally the year. Bob wonders if it is possible to rearrange the numbers in his date of birth so that he will be at least 18 years old on the day <span class="tex-span"><i>DD</i></span>.<span class="tex-span"><i>MM</i></span>.<span class="tex-span"><i>YY</i></span>. He can always tell that in his motherland dates are written differently. Help him.</p><p>According to another strange rule, eligible participant must be born in the same century as the date of the finals. If the day of the finals is participant's 18-th birthday, he is allowed to participate. </p><p>As we are considering only the years from <span class="tex-span">2001</span> to <span class="tex-span">2099</span> for the year of the finals, use the following rule: the year is leap if it's number is divisible by four.</p></div><div class="input-specification"><p>The first line contains the date <span class="tex-span"><i>DD</i></span>.<span class="tex-span"><i>MM</i></span>.<span class="tex-span"><i>YY</i></span>, the second line contains the date <span class="tex-span"><i>BD</i></span>.<span class="tex-span"><i>BM</i></span>.<span class="tex-span"><i>BY</i></span>. It is guaranteed that both dates are correct, and <span class="tex-span"><i>YY</i></span> and <span class="tex-span"><i>BY</i></span> are always in <span class="tex-span">[01;99]</span>.</p><p>It could be that by passport Bob was born after the finals. In this case, he can still change the order of numbers in date.</p></div><div class="output-specification"><p>If it is possible to rearrange the numbers in the date of birth so that Bob will be at least 18 years old on the <span class="tex-span"><i>DD</i></span>.<span class="tex-span"><i>MM</i></span>.<span class="tex-span"><i>YY</i></span>, output <span class="tex-font-style-tt">YES</span>. In the other case, output <span class="tex-font-style-tt">NO</span>. </p><p>Each number contains exactly two digits and stands for day, month or year in a date. Note that it is permitted to rearrange only numbers, not digits.</p></div>

## Input

<p>The first line contains the date <span class="tex-span"><i>DD</i></span>.<span class="tex-span"><i>MM</i></span>.<span class="tex-span"><i>YY</i></span>, the second line contains the date <span class="tex-span"><i>BD</i></span>.<span class="tex-span"><i>BM</i></span>.<span class="tex-span"><i>BY</i></span>. It is guaranteed that both dates are correct, and <span class="tex-span"><i>YY</i></span> and <span class="tex-span"><i>BY</i></span> are always in <span class="tex-span">[01;99]</span>.</p><p>It could be that by passport Bob was born after the finals. In this case, he can still change the order of numbers in date.</p>

## Output

<p>If it is possible to rearrange the numbers in the date of birth so that Bob will be at least 18 years old on the <span class="tex-span"><i>DD</i></span>.<span class="tex-span"><i>MM</i></span>.<span class="tex-span"><i>YY</i></span>, output <span class="tex-font-style-tt">YES</span>. In the other case, output <span class="tex-font-style-tt">NO</span>. </p><p>Each number contains exactly two digits and stands for day, month or year in a date. Note that it is permitted to rearrange only numbers, not digits.</p>





```input1
01.01.98
01.01.80

```




```input2
20.10.20
10.02.30

```




```input3
28.02.74
28.02.64

```




```output1
YES

```




```output2
NO

```




```output3
NO

```


