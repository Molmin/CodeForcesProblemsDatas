## Description

<div><p>Seryozha has a very changeable character. This time he refused to leave the room to Dima and his girlfriend (her hame is Inna, by the way). However, the two lovebirds can always find a way to communicate. Today they are writing text messages to each other.</p><p>Dima and Inna are using a secret code in their text messages. When Dima wants to send Inna some sentence, he writes out all words, inserting a heart before each word and after the last word. A heart is a sequence of two characters: the "less" characters (<span class="tex-font-style-tt">&lt;</span>) and the digit three (<span class="tex-font-style-tt">3</span>). After applying the code, a test message looks like that: &lt;3<span class="tex-span"><i>word</i><sub class="lower-index">1</sub></span>&lt;3<span class="tex-span"><i>word</i><sub class="lower-index">2</sub></span>&lt;3 ... <span class="tex-span"><i>word</i><sub class="lower-index"><i>n</i></sub></span>&lt;3.</p><p>Encoding doesn't end here. Then Dima inserts a random number of small English characters, digits, signs "more" and "less" into any places of the message.</p><p>Inna knows Dima perfectly well, so she knows what phrase Dima is going to send her beforehand. Inna has just got a text message. Help her find out if Dima encoded the message correctly. In other words, find out if a text message could have been received by encoding in the manner that is described above.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of words in Dima's message. Next <span class="tex-span"><i>n</i></span> lines contain non-empty words, one word per line. The words only consist of small English letters. The total length of all words doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. </p><p>The last line contains non-empty text message that Inna has got. The number of characters in the text message doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. A text message can contain only small English letters, digits and signs more and less.</p></div><div class="output-specification"><p>In a single line, print "<span class="tex-font-style-tt">yes</span>" (without the quotes), if Dima decoded the text message correctly, and "<span class="tex-font-style-tt">no</span>" (without the quotes) otherwise.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span> — the number of words in Dima's message. Next <span class="tex-span"><i>n</i></span> lines contain non-empty words, one word per line. The words only consist of small English letters. The total length of all words doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. </p><p>The last line contains non-empty text message that Inna has got. The number of characters in the text message doesn't exceed <span class="tex-span">10<sup class="upper-index">5</sup></span>. A text message can contain only small English letters, digits and signs more and less.</p>

## Output

<p>In a single line, print "<span class="tex-font-style-tt">yes</span>" (without the quotes), if Dima decoded the text message correctly, and "<span class="tex-font-style-tt">no</span>" (without the quotes) otherwise.</p>





```input1
3
i
love
you
&lt;3i&lt;3love&lt;23you&lt;3

```




```input2
7
i
am
not
main
in
the
family
&lt;3i&lt;&gt;3am&lt;3the&lt;3&lt;main&lt;3in&lt;3the&lt;3&gt;&lt;3family&lt;3

```




```output1
yes

```




```output2
no

```



## Note

<p>Please note that Dima got a good old kick in the pants for the second sample from the statement.</p>
