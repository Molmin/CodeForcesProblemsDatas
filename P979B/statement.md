## Description

<div><p>After the big birthday party, Katie still wanted Shiro to have some more fun. Later, she came up with a game called <span class="tex-font-style-it">treasure hunt</span>. Of course, she invited her best friends Kuro and Shiro to play with her.</p><p>The three friends are very smart so they passed all the challenges very quickly and finally reached the destination. But the treasure can only belong to one cat so they started to think of something which can determine who is worthy of the treasure. Instantly, Kuro came up with some ribbons.</p><p>A random colorful ribbon is given to each of the cats. Each color of the ribbon can be represented as an uppercase or lowercase Latin letter. Let's call a consecutive subsequence of colors that appears in the ribbon a <span class="tex-font-style-it">subribbon</span>. The <span class="tex-font-style-it">beauty</span> of a ribbon is defined as the maximum number of times one of its subribbon appears in the ribbon. The more the subribbon appears, the more beautiful is the ribbon. For example, the ribbon <span class="tex-font-style-tt">aaaaaaa</span> has the beauty of $7$ because its subribbon <span class="tex-font-style-tt">a</span> appears $7$ times, and the ribbon <span class="tex-font-style-tt">abcdabc</span> has the beauty of $2$ because its subribbon <span class="tex-font-style-tt">abc</span> appears twice.</p><p>The rules are simple. The game will have $n$ turns. Every turn, each of the cats must change strictly <span class="tex-font-style-bf">one</span> color (at one position) in his/her ribbon to an arbitrary color which is <span class="tex-font-style-bf">different</span> from the unchanged one. For example, a ribbon <span class="tex-font-style-tt">aaab</span> can be changed into <span class="tex-font-style-tt">acab</span> in one turn. The one having the most beautiful ribbon after $n$ turns wins the treasure.</p><p>Could you find out who is going to be the winner if they all play optimally?</p></div><div class="input-specification"><p>The first line contains an integer $n$ ($0 \leq n \leq 10^{9}$)&nbsp;— the number of turns.</p><p>Next 3 lines contain 3 ribbons of Kuro, Shiro and Katie one per line, respectively. Each ribbon is a string which contains no more than $10^{5}$ uppercase and lowercase Latin letters and is not empty. It is guaranteed that the length of all ribbons are equal for the purpose of fairness. Note that uppercase and lowercase letters are considered different colors.</p></div><div class="output-specification"><p>Print the name of the winner ("<span class="tex-font-style-tt">Kuro</span>", "<span class="tex-font-style-tt">Shiro</span>" or "<span class="tex-font-style-tt">Katie</span>"). If there are at least two cats that share the maximum beauty, print "<span class="tex-font-style-tt">Draw</span>".</p></div>

## Input

<p>The first line contains an integer $n$ ($0 \leq n \leq 10^{9}$)&nbsp;— the number of turns.</p><p>Next 3 lines contain 3 ribbons of Kuro, Shiro and Katie one per line, respectively. Each ribbon is a string which contains no more than $10^{5}$ uppercase and lowercase Latin letters and is not empty. It is guaranteed that the length of all ribbons are equal for the purpose of fairness. Note that uppercase and lowercase letters are considered different colors.</p>

## Output

<p>Print the name of the winner ("<span class="tex-font-style-tt">Kuro</span>", "<span class="tex-font-style-tt">Shiro</span>" or "<span class="tex-font-style-tt">Katie</span>"). If there are at least two cats that share the maximum beauty, print "<span class="tex-font-style-tt">Draw</span>".</p>





```input1
3
Kuroo
Shiro
Katie

```




```input2
7
treasurehunt
threefriends
hiCodeforces

```




```input3
1
abcabc
cbabac
ababca

```




```input4
15
foPaErcvJ
mZaxowpbt
mkuOlaHRE

```




```output1
Kuro

```




```output2
Shiro

```




```output3
Katie

```




```output4
Draw

```



## Note

<p>In the first example, after $3$ turns, Kuro can change his ribbon into <span class="tex-font-style-tt">ooooo</span>, which has the beauty of $5$, while reaching such beauty for Shiro and Katie is impossible (both Shiro and Katie can reach the beauty of at most $4$, for example by changing Shiro's ribbon into <span class="tex-font-style-tt">SSiSS</span> and changing Katie's ribbon into <span class="tex-font-style-tt">Kaaaa</span>). Therefore, the winner is Kuro.</p><p>In the fourth example, since the length of each of the string is $9$ and the number of turn is $15$, everyone can change their ribbons in some way to reach the maximal beauty of $9$ by changing their strings into <span class="tex-font-style-tt">zzzzzzzzz</span> after 9 turns, and repeatedly change their strings into <span class="tex-font-style-tt">azzzzzzzz</span> and then into <span class="tex-font-style-tt">zzzzzzzzz</span> thrice. Therefore, the game ends in a draw.</p>
