## Description

<div><p>One day, liouzhou_101 got a chat record of Freda and Rainbow. Out of curiosity, he wanted to know which sentences were said by Freda, and which were said by Rainbow. According to his experience, he thought that Freda always said "<span class="tex-font-style-tt">lala.</span>" at the end of her sentences, while Rainbow always said "<span class="tex-font-style-tt">miao.</span>" at the beginning of his sentences. For each sentence in the chat record, help liouzhou_101 find whose sentence it is. </p></div><div class="input-specification"><p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>), number of sentences in the chat record. Each of the next <span class="tex-span"><i>n</i></span> lines contains a sentence. A sentence is a string that contains only Latin letters (<span class="tex-font-style-tt">A-Z</span>, <span class="tex-font-style-tt">a-z</span>), underline (<span class="tex-font-style-tt">_</span>), comma (<span class="tex-font-style-tt">,</span>), point (<span class="tex-font-style-tt">.</span>) and space (<span class="tex-font-style-tt"> </span>). Its length doesn’t exceed 100.</p></div><div class="output-specification"><p>For each sentence, output "<span class="tex-font-style-tt">Freda's</span>" if the sentence was said by Freda, "<span class="tex-font-style-tt">Rainbow's</span>" if the sentence was said by Rainbow, or "<span class="tex-font-style-tt">OMG&gt;.&lt; I don't know!</span>" if liouzhou_101 can’t recognize whose sentence it is. He can’t recognize a sentence if it begins with "<span class="tex-font-style-tt">miao.</span>" and ends with "<span class="tex-font-style-tt">lala.</span>", or satisfies neither of the conditions. </p></div>

## Input

<p>The first line of the input contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>), number of sentences in the chat record. Each of the next <span class="tex-span"><i>n</i></span> lines contains a sentence. A sentence is a string that contains only Latin letters (<span class="tex-font-style-tt">A-Z</span>, <span class="tex-font-style-tt">a-z</span>), underline (<span class="tex-font-style-tt">_</span>), comma (<span class="tex-font-style-tt">,</span>), point (<span class="tex-font-style-tt">.</span>) and space (<span class="tex-font-style-tt"> </span>). Its length doesn’t exceed 100.</p>

## Output

<p>For each sentence, output "<span class="tex-font-style-tt">Freda's</span>" if the sentence was said by Freda, "<span class="tex-font-style-tt">Rainbow's</span>" if the sentence was said by Rainbow, or "<span class="tex-font-style-tt">OMG&gt;.&lt; I don't know!</span>" if liouzhou_101 can’t recognize whose sentence it is. He can’t recognize a sentence if it begins with "<span class="tex-font-style-tt">miao.</span>" and ends with "<span class="tex-font-style-tt">lala.</span>", or satisfies neither of the conditions. </p>





```input1
5
I will go to play with you lala.
wow, welcome.
miao.lala.
miao.
miao .

```




```output1
Freda's
OMG&gt;.&lt; I don't know!
OMG&gt;.&lt; I don't know!
Rainbow's
OMG&gt;.&lt; I don't know!

```


