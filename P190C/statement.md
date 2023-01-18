## Description

<div><p>Vasya used to be an accountant before the war began and he is one of the few who knows how to operate a computer, so he was assigned as the programmer.</p><p>We all know that programs often store sets of integers. For example, if we have a problem about a weighted directed graph, its edge can be represented by three integers: the number of the starting vertex, the number of the final vertex and the edge's weight. So, as Vasya was trying to represent characteristics of a recently invented robot in his program, he faced the following problem.</p><p>Vasya is not a programmer, so he asked his friend Gena, what the convenient way to store <span class="tex-span"><i>n</i></span> integers is. Gena used to code in language X-<span class="tex-font-style-it"></span>- and so he can use only the types that occur in this language. Let's define, what a "type" is in language X-<span class="tex-font-style-it"></span>-:</p><ul> <li> First, a type is a string "<span class="tex-font-style-tt">int</span>". </li><li> Second, a type is a string that starts with "<span class="tex-font-style-tt">pair</span>", then followed by angle brackets listing <span class="tex-font-style-bf">exactly two</span> comma-separated other types of language X-<span class="tex-font-style-it"></span>-. This record contains no spaces. </li><li> No other strings can be regarded as types. </li></ul><p>More formally: <span class="tex-font-style-tt">type</span> := <span class="tex-font-style-tt">int</span> | <span class="tex-font-style-tt">pair&lt;type,type&gt;</span>. For example, Gena uses the following type for graph edges: <span class="tex-font-style-tt">pair&lt;int,pair&lt;int,int&gt;<span class="tex-font-style-it"></span>&gt;</span>.</p><p>Gena was pleased to help Vasya, he dictated to Vasya a type of language X-<span class="tex-font-style-it"></span>-, that stores <span class="tex-span"><i>n</i></span> integers. Unfortunately, Gena was in a hurry, so he omitted the punctuation. Now Gena has already left and Vasya can't find the correct punctuation, resulting in a type of language X-<span class="tex-font-style-it"></span>-, however hard he tries.</p><p>Help Vasya and add the punctuation marks so as to receive the valid type of language X-<span class="tex-font-style-it"></span>-. Otherwise say that the task is impossible to perform.</p></div><div class="input-specification"><p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, showing how many numbers the type dictated by Gena contains.</p><p>The second line contains space-separated words, said by Gena. Each of them is either "<span class="tex-font-style-tt">pair</span>" or "<span class="tex-font-style-tt">int</span>" (without the quotes).</p><p>It is guaranteed that the total number of words does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> and that among all the words that Gena said, there are exactly <span class="tex-span"><i>n</i></span> words "<span class="tex-font-style-tt">int</span>".</p></div><div class="output-specification"><p>If it is possible to add the punctuation marks so as to get a correct type of language X-<span class="tex-font-style-it"></span>- as a result, print a single line that represents the resulting type. Otherwise, print "<span class="tex-font-style-tt">Error occurred</span>" (without the quotes). <span class="tex-font-style-bf">Inside the record of a type should not be any extra spaces and other characters</span>. </p><p>It is guaranteed that if such type exists, then it is unique.</p><p>Note that you should print the type dictated by Gena (if such type exists) and not any type that can contain <span class="tex-span"><i>n</i></span> values.</p></div>

## Input

<p>The first line contains a single integer <span class="tex-span"><i>n</i></span> <span class="tex-span">(1 ≤ <i>n</i> ≤ 10<sup class="upper-index">5</sup>)</span>, showing how many numbers the type dictated by Gena contains.</p><p>The second line contains space-separated words, said by Gena. Each of them is either "<span class="tex-font-style-tt">pair</span>" or "<span class="tex-font-style-tt">int</span>" (without the quotes).</p><p>It is guaranteed that the total number of words does not exceed <span class="tex-span">10<sup class="upper-index">5</sup></span> and that among all the words that Gena said, there are exactly <span class="tex-span"><i>n</i></span> words "<span class="tex-font-style-tt">int</span>".</p>

## Output

<p>If it is possible to add the punctuation marks so as to get a correct type of language X-<span class="tex-font-style-it"></span>- as a result, print a single line that represents the resulting type. Otherwise, print "<span class="tex-font-style-tt">Error occurred</span>" (without the quotes). <span class="tex-font-style-bf">Inside the record of a type should not be any extra spaces and other characters</span>. </p><p>It is guaranteed that if such type exists, then it is unique.</p><p>Note that you should print the type dictated by Gena (if such type exists) and not any type that can contain <span class="tex-span"><i>n</i></span> values.</p>





```input1
3
pair pair int int int

```




```input2
1
pair int

```




```output1
pair&lt;pair&lt;int,int&gt;,int&gt;
```




```output2
Error occurred
```


