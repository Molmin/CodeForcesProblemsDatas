## Description

<div><p>Each of you probably has your personal experience of riding public transportation and buying tickets. After a person buys a ticket (which traditionally has an <span class="tex-font-style-bf">even</span> number of digits), he usually checks whether the ticket is lucky. Let us remind you that a ticket is lucky if the sum of digits in its first half matches the sum of digits in its second half.</p><p>But of course, not every ticket can be lucky. Far from it! Moreover, sometimes one look at a ticket can be enough to say right away that the ticket is not lucky. So, let's consider the following <span class="tex-font-style-underline">unluckiness criterion</span> that can definitely determine an unlucky ticket. We'll say that a ticket is definitely unlucky if each digit from the first half corresponds to some digit from the second half so that each digit from the first half is <span class="tex-font-style-bf">strictly less</span> than the corresponding digit from the second one or each digit from the first half is <span class="tex-font-style-bf">strictly more</span> than the corresponding digit from the second one. Each digit should be used exactly once in the comparisons. In other words, there is such <span class="tex-font-style-underline">bijective correspondence</span> between the digits of the first and the second half of the ticket, that either each digit of the first half turns out <span class="tex-font-style-bf">strictly less</span> than the corresponding digit of the second half or each digit of the first half turns out <span class="tex-font-style-bf">strictly more</span> than the corresponding digit from the second half.</p><p>For example, ticket <span class="tex-span">2421</span> meets the following unluckiness criterion and will not be considered lucky (the sought correspondence is <span class="tex-span">2 &gt; 1</span> and <span class="tex-span">4 &gt; 2</span>), ticket <span class="tex-span">0135</span> also meets the criterion (the sought correspondence is <span class="tex-span">0 &lt; 3</span> and <span class="tex-span">1 &lt; 5</span>), and ticket <span class="tex-span">3754</span> does not meet the criterion. </p><p>You have a ticket in your hands, it contains <span class="tex-span">2<i>n</i></span> digits. Your task is to check whether it meets the unluckiness criterion.</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). The second line contains a string that consists of <span class="tex-span">2<i>n</i></span> digits and defines your ticket.</p></div><div class="output-specification"><p>In the first line print "<span class="tex-font-style-tt">YES</span>" if the ticket meets the unluckiness criterion. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>). The second line contains a string that consists of <span class="tex-span">2<i>n</i></span> digits and defines your ticket.</p>

## Output

<p>In the first line print "<span class="tex-font-style-tt">YES</span>" if the ticket meets the unluckiness criterion. Otherwise, print "<span class="tex-font-style-tt">NO</span>" (without the quotes).</p>





```input1
2
2421

```




```input2
2
0135

```




```input3
2
3754

```




```output1
YES

```




```output2
YES

```




```output3
NO

```


