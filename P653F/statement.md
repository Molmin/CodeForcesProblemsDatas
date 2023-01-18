## Description

<div><p>Alex was programming while Valentina (his toddler daughter) got there and started asking many questions about the round brackets (or parenthesis) in the code. He explained her a bit and when she got it he gave her a task in order to finish his code on time.</p><p>For the purpose of this problem we consider only strings consisting of opening and closing round brackets, that is characters '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>'.</p><p>The sequence of brackets is called <span class="tex-font-style-it">correct</span> if: </p><ol> <li> it's empty; </li><li> it's a correct sequence of brackets, enclosed in a pair of opening and closing brackets; </li><li> it's a concatenation of two correct sequences of brackets. </li></ol><p>For example, the sequences "<span class="tex-font-style-tt">()()</span>" and "<span class="tex-font-style-tt">((()))(())</span>" are correct, while "<span class="tex-font-style-tt">)(()</span>", "<span class="tex-font-style-tt">(((((</span>" and "<span class="tex-font-style-tt">())</span>" are not.</p><p>Alex took a piece of paper, wrote a string <span class="tex-span"><i>s</i></span> consisting of brackets and asked Valentina to count the number of <span class="tex-font-style-bf">distinct</span> non-empty substrings of <span class="tex-span"><i>s</i></span> that are correct sequences of brackets. In other words, her task is to count the number of non-empty correct sequences of brackets that occur in a string <span class="tex-span"><i>s</i></span> as a <span class="tex-font-style-bf">substring</span> (don't mix up with subsequences).</p><p>When Valentina finished the task, Alex noticed he doesn't know the answer. Help him don't loose face in front of Valentina and solve the problem!</p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000</span>)&nbsp;— the length of the string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> consisting of only '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>'.</p></div><div class="output-specification"><p>Print the number of <span class="tex-font-style-bf">distinct</span> non-empty correct sequences that occur in <span class="tex-span"><i>s</i></span> as substring.</p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 500 000</span>)&nbsp;— the length of the string <span class="tex-span"><i>s</i></span>.</p><p>The second line contains a string <span class="tex-span"><i>s</i></span> of length <span class="tex-span"><i>n</i></span> consisting of only '<span class="tex-font-style-tt">(</span>' and '<span class="tex-font-style-tt">)</span>'.</p>

## Output

<p>Print the number of <span class="tex-font-style-bf">distinct</span> non-empty correct sequences that occur in <span class="tex-span"><i>s</i></span> as substring.</p>





```input1
10
()()()()()

```




```input2
7
)(())()

```




```output1
5

```




```output2
3

```



## Note

<p>In the first sample, there are <span class="tex-span">5</span> distinct substrings we should count: "<span class="tex-font-style-tt">()</span>", "<span class="tex-font-style-tt">()()</span>", "<span class="tex-font-style-tt">()()()</span>", "<span class="tex-font-style-tt">()()()()</span>" and "<span class="tex-font-style-tt">()()()()()</span>".</p><p>In the second sample, there are <span class="tex-span">3</span> distinct substrings we should count: "<span class="tex-font-style-tt">()</span>", "<span class="tex-font-style-tt">(())</span>" and "<span class="tex-font-style-tt">(())()</span>".</p>
