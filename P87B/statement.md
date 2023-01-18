## Description

<div><p>Programmer Vasya is studying a new programming language &amp;K*. The &amp;K* language resembles the languages of the C family in its syntax. However, it is more powerful, which is why the rules of the actual C-like languages are unapplicable to it. To fully understand the statement, please read the language's description below carefully and follow it and not the similar rules in real programming languages.</p><p>There is a very powerful system of pointers on &amp;K* — you can add an asterisk to the right of the existing type <span class="tex-span"><i>X</i></span> — that will result in new type <span class="tex-span"><i>X</i> * </span>. That is called pointer-definition operation. Also, there is the operation that does the opposite — to any type of <span class="tex-span"><i>X</i></span>, which is a pointer, you can add an ampersand — that will result in a type <span class="tex-span">&amp;<i>X</i></span>, to which refers <span class="tex-span"><i>X</i></span>. That is called a dereference operation.</p><p>The &amp;K* language has only two basic data types — <span class="tex-font-style-tt">void</span> and <span class="tex-font-style-tt">errtype</span>. Also, the language has operators <span class="tex-font-style-tt">typedef</span> and <span class="tex-font-style-tt">typeof</span>.</p><ul><li> The operator "<span class="tex-font-style-tt">typedef <span class="tex-span"><i>A</i></span> <span class="tex-span"><i>B</i></span></span>" defines a new data type <span class="tex-span"><i>B</i></span>, which is equivalent to <span class="tex-span"><i>A</i></span>. <span class="tex-span"><i>A</i></span> can have asterisks and ampersands, and <span class="tex-span"><i>B</i></span> cannot have them. For example, the operator <span class="tex-font-style-tt">typedef void** ptptvoid</span> will create a new type <span class="tex-font-style-tt">ptptvoid</span>, that can be used as <span class="tex-font-style-tt">void**</span>.</li><li> The operator "<span class="tex-font-style-tt">typeof <span class="tex-span"><i>A</i></span></span>" returns type of <span class="tex-span"><i>A</i></span>, brought to <span class="tex-font-style-tt">void</span>, that is, returns the type <span class="tex-font-style-tt">void**...*</span>, equivalent to it with the necessary number of asterisks (the number can possibly be zero). That is, having defined the <span class="tex-font-style-tt">ptptvoid</span> type, as shown above, the <span class="tex-font-style-tt">typeof ptptvoid</span> operator will return <span class="tex-font-style-tt">void**</span>.</li></ul><p>An attempt of dereferencing of the <span class="tex-font-style-tt">void</span> type will lead to an error: to a special data type <span class="tex-font-style-tt">errtype</span>. For <span class="tex-font-style-tt">errtype</span> the following equation holds true: <span class="tex-font-style-tt">errtype*</span><span class="tex-span"> = </span><span class="tex-font-style-tt">&amp;errtype</span><span class="tex-span"> = </span><span class="tex-font-style-tt">errtype</span>. An attempt to use the data type that hasn't been defined before that will also lead to the <span class="tex-font-style-tt">errtype</span>.</p><p>Using <span class="tex-font-style-tt">typedef</span>, we can define one type several times. Of all the definitions only the last one is valid. However, all the types that have been defined earlier using this type do not change.</p><p>Let us also note that the dereference operation has the lower priority that the pointer operation, in other words <span class="tex-span">&amp;<i>T</i> * </span> is always equal to <span class="tex-span"><i>T</i></span>.</p><p>Note, that the operators are executed consecutively one by one. If we have two operators "<span class="tex-font-style-tt">typedef &amp;void a</span>" and "<span class="tex-font-style-tt">typedef a* b</span>", then at first <span class="tex-font-style-tt">a</span> becomes <span class="tex-font-style-tt">errtype</span>, and after that <span class="tex-font-style-tt">b</span> becomes <span class="tex-font-style-tt">errtype* = errtype</span>, but <span class="tex-font-style-bf">not</span> <span class="tex-font-style-tt">&amp;void* = void</span> (see sample 2).</p><p>Vasya does not yet fully understand this powerful technology, that's why he asked you to help him. Write a program that analyzes these operators. </p></div><div class="input-specification"><p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of operators. Then follow <span class="tex-span"><i>n</i></span> lines with operators. Each operator is of one of two types: either "<span class="tex-font-style-tt">typedef <span class="tex-span"><i>A</i></span> <span class="tex-span"><i>B</i></span></span>", or "<span class="tex-font-style-tt">typeof <span class="tex-span"><i>A</i></span></span>". In the first case the <span class="tex-span"><i>B</i></span> type differs from <span class="tex-font-style-tt">void</span> and <span class="tex-font-style-tt">errtype</span> types, and besides, doesn't have any asterisks and ampersands.</p><p>All the data type names are non-empty lines of no more than 20 lowercase Latin letters. The number of asterisks and ampersands separately in one type in any operator does not exceed 10, however if we bring some types to <span class="tex-font-style-tt">void</span> with several asterisks, their number may exceed 10.</p></div><div class="output-specification"><p>For every <span class="tex-font-style-tt">typeof</span> operator print on the single line the answer to that operator — the type that the given operator returned.</p></div>

## Input

<p>The first line contains an integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 100</span>) — the number of operators. Then follow <span class="tex-span"><i>n</i></span> lines with operators. Each operator is of one of two types: either "<span class="tex-font-style-tt">typedef <span class="tex-span"><i>A</i></span> <span class="tex-span"><i>B</i></span></span>", or "<span class="tex-font-style-tt">typeof <span class="tex-span"><i>A</i></span></span>". In the first case the <span class="tex-span"><i>B</i></span> type differs from <span class="tex-font-style-tt">void</span> and <span class="tex-font-style-tt">errtype</span> types, and besides, doesn't have any asterisks and ampersands.</p><p>All the data type names are non-empty lines of no more than 20 lowercase Latin letters. The number of asterisks and ampersands separately in one type in any operator does not exceed 10, however if we bring some types to <span class="tex-font-style-tt">void</span> with several asterisks, their number may exceed 10.</p>

## Output

<p>For every <span class="tex-font-style-tt">typeof</span> operator print on the single line the answer to that operator — the type that the given operator returned.</p>





```input1
5
typedef void* ptv
typeof ptv
typedef &amp;&amp;ptv node
typeof node
typeof &amp;ptv

```




```input2
17
typedef void* b
typedef b* c
typeof b
typeof c
typedef &amp;b b
typeof b
typeof c
typedef &amp;&amp;b* c
typeof c
typedef &amp;b* c
typeof c
typedef &amp;void b
typeof b
typedef b******* c
typeof c
typedef &amp;&amp;b* c
typeof c

```




```output1
void*
errtype
void

```




```output2
void*
void**
void
void**
errtype
void
errtype
errtype
errtype

```



## Note

<p>Let's look at the second sample.</p><p>After the first two queries <span class="tex-font-style-tt">typedef</span> the <span class="tex-font-style-tt">b</span> type is equivalent to <span class="tex-font-style-tt">void*</span>, and <span class="tex-font-style-tt">с</span> — to <span class="tex-font-style-tt">void**</span>.</p><p>The next query <span class="tex-font-style-tt">typedef</span> redefines <span class="tex-font-style-tt">b</span> — it is now equal to <span class="tex-font-style-tt">&amp;b = &amp;void* = void</span>. At that, the <span class="tex-font-style-tt">с</span> type doesn't change.</p><p>After that the <span class="tex-font-style-tt">с</span> type is defined as <span class="tex-font-style-tt">&amp;&amp;b* = &amp;&amp;void* = &amp;void = errtype</span>. It doesn't influence the <span class="tex-font-style-tt">b</span> type, that's why the next <span class="tex-font-style-tt">typedef</span> defines <span class="tex-font-style-tt">c</span> as <span class="tex-font-style-tt">&amp;void* = void</span>.</p><p>Then the <span class="tex-font-style-tt">b</span> type is again redefined as <span class="tex-font-style-tt">&amp;void = errtype</span>. </p><p>Please note that the <span class="tex-font-style-tt">c</span> type in the next query is defined exactly as <span class="tex-font-style-tt">errtype******* = errtype</span>, and not <span class="tex-font-style-tt">&amp;void******* = void******</span>. The same happens in the last <span class="tex-font-style-tt">typedef</span>.</p>
