## Description

<div><p>Bizon the Champion isn't just a bison. He also is a favorite of the "Bizons" team.</p><p>At a competition the "Bizons" got the following problem: "You are given two distinct words (strings of English letters), <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span>. You need to transform word <span class="tex-span"><i>s</i></span> into word <span class="tex-span"><i>t</i></span>". The task looked simple to the guys because they know the suffix data structures well. Bizon Senior loves suffix automaton. By applying it once to a string, he can remove from this string any single character. Bizon Middle knows suffix array well. By applying it once to a string, he can swap any two characters of this string. The guys do not know anything about the suffix tree, but it can help them do much more. </p><p>Bizon the Champion wonders whether the "Bizons" can solve the problem. Perhaps, the solution do not require both data structures. Find out whether the guys can solve the problem and if they can, how do they do it? Can they solve it either only with use of suffix automaton or only with use of suffix array or they need both structures? Note that any structure may be used an unlimited number of times, the structures may be used in any order.</p></div><div class="input-specification"><p>The first line contains a non-empty word <span class="tex-span"><i>s</i></span>. The second line contains a non-empty word <span class="tex-span"><i>t</i></span>. Words <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> are different. Each word consists only of lowercase English letters. Each word contains at most 100 letters.</p></div><div class="output-specification"><p>In the single line print the answer to the problem. Print "<span class="tex-font-style-tt">need tree</span>" (without the quotes) if word <span class="tex-span"><i>s</i></span> cannot be transformed into word <span class="tex-span"><i>t</i></span> even with use of both suffix array and suffix automaton. Print "<span class="tex-font-style-tt">automaton</span>" (without the quotes) if you need only the suffix automaton to solve the problem. Print "<span class="tex-font-style-tt">array</span>" (without the quotes) if you need only the suffix array to solve the problem. Print "<span class="tex-font-style-tt">both</span>" (without the quotes), if you need both data structures to solve the problem.</p><p>It's guaranteed that if you can solve the problem only with use of suffix array, then it is impossible to solve it only with use of suffix automaton. This is also true for suffix automaton.</p></div>

## Input

<p>The first line contains a non-empty word <span class="tex-span"><i>s</i></span>. The second line contains a non-empty word <span class="tex-span"><i>t</i></span>. Words <span class="tex-span"><i>s</i></span> and <span class="tex-span"><i>t</i></span> are different. Each word consists only of lowercase English letters. Each word contains at most 100 letters.</p>

## Output

<p>In the single line print the answer to the problem. Print "<span class="tex-font-style-tt">need tree</span>" (without the quotes) if word <span class="tex-span"><i>s</i></span> cannot be transformed into word <span class="tex-span"><i>t</i></span> even with use of both suffix array and suffix automaton. Print "<span class="tex-font-style-tt">automaton</span>" (without the quotes) if you need only the suffix automaton to solve the problem. Print "<span class="tex-font-style-tt">array</span>" (without the quotes) if you need only the suffix array to solve the problem. Print "<span class="tex-font-style-tt">both</span>" (without the quotes), if you need both data structures to solve the problem.</p><p>It's guaranteed that if you can solve the problem only with use of suffix array, then it is impossible to solve it only with use of suffix automaton. This is also true for suffix automaton.</p>





```input1
automaton
tomat

```




```input2
array
arary

```




```input3
both
hot

```




```input4
need
tree

```




```output1
automaton

```




```output2
array

```




```output3
both

```




```output4
need tree

```



## Note

<p>In the third sample you can act like that: first transform "<span class="tex-font-style-tt">both</span>" into "<span class="tex-font-style-tt">oth</span>" by removing the first character using the suffix automaton and then make two swaps of the string using the suffix array and get "<span class="tex-font-style-tt">hot</span>".</p>
