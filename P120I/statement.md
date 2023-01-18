## Description

<div><p>Vasya has been collecting transport tickets for quite a while now. His collection contains several thousands of tram, trolleybus and bus tickets. Vasya is already fed up with the traditional definition of what a lucky ticket is. Thus, he's looking for new perspectives on that. Besides, Vasya cannot understand why all tickets are only divided into lucky and unlucky ones. He thinks that all tickets are lucky but in different degrees. Having given the matter some thought, Vasya worked out the definition of a ticket's <span class="tex-font-style-it">degree of luckiness</span>. Let a ticket consist of <span class="tex-span">2<i>n</i></span> digits. Let's regard each digit as written as is shown on the picture:</p><center> <img class="tex-graphics" height="76px" src="file://16fBXurY.png" style="max-width: 100.0%;max-height: 100.0%;" width="378px"> </center><p>You have seen such digits on electronic clocks: seven segments are used to show digits. Each segment can either be colored or not. The colored segments form a digit. Vasya regards the digits as written in this very way and takes the right half of the ticket and puts it one the left one, so that the first digit coincides with the <span class="tex-span"><i>n</i> + 1</span>-th one, the second digit coincides with the <span class="tex-span"><i>n</i> + 2</span>-th one, ..., the <span class="tex-span"><i>n</i></span>-th digit coincides with the <span class="tex-span">2<i>n</i></span>-th one. For each pair of digits, put one on another, he counts the number of segments colored in both digits and summarizes the resulting numbers. The resulting value is called the <span class="tex-font-style-it">degree of luckiness</span> of a ticket. For example, the degree of luckiness of ticket 03 equals four and the degree of luckiness of ticket 2345 equals six.</p><p>You are given the number of a ticket containing <span class="tex-span">2<i>n</i></span> digits. Your task is to find among the tickets whose number exceeds the number of this ticket but also consists of <span class="tex-span">2<i>n</i></span> digits such ticket, whose degree of luckiness exceeds the degrees of luckiness of the given ticket. Moreover, if there are several such tickets, you should only choose the one with the smallest number.</p></div><div class="input-specification"><p>The first line contains the number of the ticket that consists of <span class="tex-span"><i>k</i></span> characters (<span class="tex-span"><i>k</i> = 2<i>n</i>, 1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). </p></div><div class="output-specification"><p>Print the number of the sought ticket or "-1" (without the quotes) if no such ticket exists.</p></div>

## Input

<p>The first line contains the number of the ticket that consists of <span class="tex-span"><i>k</i></span> characters (<span class="tex-span"><i>k</i> = 2<i>n</i>, 1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup></span>). </p>

## Output

<p>Print the number of the sought ticket or "-1" (without the quotes) if no such ticket exists.</p>





```input1
13

```




```input2
2345

```




```input3
88

```




```output1
20

```




```output2
2348

```




```output3
-1

```


