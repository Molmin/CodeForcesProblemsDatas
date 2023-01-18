## Description

<div><p>Fangy the little walrus, as all the modern walruses, loves to communicate via text messaging. One day he faced the following problem: When he sends large texts, they are split into parts each containing <span class="tex-span"><i>n</i></span> characters (which is the size of one text message). Thus, whole sentences and words get split!</p><p>Fangy did not like it, so he faced the task of breaking the text into minimal messages on his own so that no sentence were broken into pieces when it is sent and the number of text messages to be sent would be minimal. If two consecutive sentences are in different messages, the space between them can be ignored (Fangy does not write this space).</p><p>The little walrus's text looks in the following manner: </p><pre class="verbatim">TEXT ::= SENTENCE | SENTENCE SPACE TEXT<br>SENTENCE ::= WORD SPACE SENTENCE | WORD END<br>END ::= {'.', '?', '!'}<br>WORD ::= LETTER | LETTER WORD<br>LETTER ::= {'a'..'z', 'A'..'Z'}<br>SPACE ::= ' '<br></pre><p>SPACE stands for the symbol of a space.</p><p>So, how many messages did Fangy send?</p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span>, which is the size of one message (<span class="tex-span">2 ≤ <i>n</i> ≤ 255</span>). The second line contains the text. The length of the text does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> characters. It is guaranteed that the text satisfies the above described format. Specifically, this implies that the text is not empty.</p></div><div class="output-specification"><p>On the first and only line print the number of text messages Fangy will need. If it is impossible to split the text, print "<span class="tex-font-style-tt">Impossible</span>" without the quotes.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span>, which is the size of one message (<span class="tex-span">2 ≤ <i>n</i> ≤ 255</span>). The second line contains the text. The length of the text does not exceed <span class="tex-span">10<sup class="upper-index">4</sup></span> characters. It is guaranteed that the text satisfies the above described format. Specifically, this implies that the text is not empty.</p>

## Output

<p>On the first and only line print the number of text messages Fangy will need. If it is impossible to split the text, print "<span class="tex-font-style-tt">Impossible</span>" without the quotes.</p>





```input1
25
Hello. I am a little walrus.

```




```input2
2
How are you?

```




```input3
19
Hello! Do you like fish? Why?

```




```output1
2

```




```output2
Impossible

```




```output3
3

```



## Note

<p>Let's take a look at the third sample. The text will be split into three messages: "<span class="tex-font-style-tt">Hello!</span>", "<span class="tex-font-style-tt">Do you like fish?</span>" and "<span class="tex-font-style-tt">Why?</span>".</p>
