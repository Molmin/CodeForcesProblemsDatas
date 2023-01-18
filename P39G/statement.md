## Description

<div><p>Petya wrote a programme on C++ that calculated a very interesting function <span class="tex-span"><i>f</i>(<i>n</i>)</span>. Petya ran the program with a certain value of <span class="tex-span"><i>n</i></span> and went to the kitchen to have some tea. The history has no records concerning how long the program had been working. By the time Petya returned, it had completed the calculations and had the result. However while Petya was drinking tea, a sly virus managed to destroy the input file so that Petya can't figure out for which value of <span class="tex-span"><i>n</i></span> the program was run. Help Petya, carry out the inverse function!</p><p>Mostly, the program consists of a function in C++ with the following simplified syntax:</p><ul> <li> <span class="tex-span"><i>function</i></span> ::= int f(int n) {<span class="tex-span"><i>operatorSequence</i></span>}</li><li> <span class="tex-span"><i>operatorSequence</i></span> ::= <span class="tex-span"><i>operator</i>&nbsp;|&nbsp;<i>operator</i>&nbsp;<i>operatorSequence</i></span></li><li> <span class="tex-span"><i>operator</i></span> ::= return <span class="tex-span"><i>arithmExpr</i></span>; <span class="tex-span">|</span> if (<span class="tex-span"><i>logicalExpr</i></span>) return <span class="tex-span"><i>arithmExpr</i></span>;</li><li> <span class="tex-span"><i>logicalExpr</i></span> ::= <span class="tex-span"><i>arithmExpr</i> &gt; <i>arithmExpr</i></span> <span class="tex-span">|</span> <span class="tex-span"><i>arithmExpr</i> &lt; <i>arithmExpr</i></span> <span class="tex-span">|</span> <span class="tex-span"><i>arithmExpr</i></span> == <span class="tex-span"><i>arithmExpr</i></span></li><li> <span class="tex-span"><i>arithmExpr</i></span> ::= <span class="tex-span"><i>sum</i></span></li><li> <span class="tex-span"><i>sum</i></span> ::= <span class="tex-span"><i>product</i></span> <span class="tex-span">|</span> <span class="tex-span"><i>sum</i> + <i>product</i></span> <span class="tex-span">|</span> <span class="tex-span"><i>sum</i> - <i>product</i></span></li><li> <span class="tex-span"><i>product</i></span> ::= <span class="tex-span"><i>multiplier</i></span> <span class="tex-span">|</span> <span class="tex-span"><i>product</i> * <i>multiplier</i></span> <span class="tex-span">|</span> <span class="tex-span"><i>product</i> / <i>multiplier</i></span></li><li> <span class="tex-span"><i>multiplier</i></span> ::= n <span class="tex-span">|</span> <span class="tex-span"><i>number</i></span> <span class="tex-span">|</span> f(<span class="tex-span"><i>arithmExpr</i></span>)</li><li> <span class="tex-span"><i>number</i></span> ::= <span class="tex-span">0|1|2|... |32767</span> </li></ul><p>The whitespaces in a <span class="tex-span"><i>operatorSequence</i></span> are optional.</p><p>Thus, we have a function, in which body there are two kinds of operators. There is the operator "return <span class="tex-span"><i>arithmExpr</i></span>;" that returns the value of the expression as the value of the function, and there is the conditional operator "if (<span class="tex-span"><i>logicalExpr</i></span>) return <span class="tex-span"><i>arithmExpr</i></span>;" that returns the value of the arithmetical expression when and only when the logical expression is true. Guaranteed that no other constructions of C++ language — cycles, assignment operators, nested conditional operators etc, and other variables except the <span class="tex-span"><i>n</i></span> parameter are used in the function. All the constants are integers in the interval <span class="tex-span">[0..32767]</span>.</p><p>The operators are performed sequentially. After the function has returned a value other operators in the sequence are not performed. Arithmetical expressions are performed taking into consideration the standard priority of the operations. It means that first all the products that are part of the sum are calculated. During the calculation of the products the operations of multiplying and division are performed from the left to the right. Then the summands are summed, and the addition and the subtraction are also performed from the left to the right. Operations "&gt;" (more), "&lt;" (less) and "==" (equals) also have standard meanings.</p><p>Now you've got to pay close attention! The program is compiled with the help of <span class="tex-span">15</span>-bit Berland C++ compiler invented by a Berland company BerSoft, that's why arithmetical operations are performed in a non-standard way. Addition, subtraction and multiplication are performed modulo <span class="tex-span">32768</span> (if the result of subtraction is negative, then <span class="tex-span">32768</span> is added to it until the number belongs to the interval <span class="tex-span">[0..32767]</span>). Division "/" is a usual integer division where the remainder is omitted.</p><p>Examples of arithmetical operations: </p><center class="tex-equation"><img align="middle" class="tex-formula" src="file://YCRclNr3.png" style="max-width: 100.0%;max-height: 100.0%;"></center><p>Guaranteed that for all values of <span class="tex-span"><i>n</i></span> from <span class="tex-span">0</span> to <span class="tex-span">32767</span> the given function is performed correctly. That means that:</p><p>1. Division by <span class="tex-span">0</span> never occures.</p><p>2. When performing a function for the value <span class="tex-span"><i>n</i> = <i>N</i></span> recursive calls of the function <span class="tex-span"><i>f</i></span> may occur only for the parameter value of <span class="tex-span">0, 1, ..., <i>N</i> - 1</span>. Consequently, the program never has an infinite recursion.</p><p>3. As the result of the sequence of the operators, the function always returns a value.</p><p>We have to mention that due to all the limitations the value returned by the function <span class="tex-span"><i>f</i></span> is independent from either global variables or the order of performing the calculations of arithmetical expressions as part of the logical one, or from anything else except the value of <span class="tex-span"><i>n</i></span> parameter. That's why the <span class="tex-span"><i>f</i></span> function can be regarded as a function in its mathematical sense, i.e. as a unique correspondence between any value of <span class="tex-span"><i>n</i></span> from the interval <span class="tex-span">[0..32767]</span> and a value of <span class="tex-span"><i>f</i>(<i>n</i>)</span> from the same interval.</p><p>Given the value of <span class="tex-span"><i>f</i>(<i>n</i>)</span>, and you should find <span class="tex-span"><i>n</i></span>. If the suitable <span class="tex-span"><i>n</i></span> value is not unique, you should find the maximal one (from the interval <span class="tex-span">[0..32767]</span>).</p></div><div class="input-specification"><p>The first line has an integer <span class="tex-span"><i>f</i>(<i>n</i>)</span> from the interval <span class="tex-span">[0..32767]</span>. The next lines have the description of the function <span class="tex-span"><i>f</i></span>. In the description can be found extra spaces and line breaks (see the examples) which, of course, can’t break key words int, if, return and numbers. The size of input data can’t exceed <span class="tex-span">100</span> bytes.</p></div><div class="output-specification"><p>Output a single number — the answer to the problem. If there’s no answer, output "-1" (without quotes).</p></div>

## Input

<p>The first line has an integer <span class="tex-span"><i>f</i>(<i>n</i>)</span> from the interval <span class="tex-span">[0..32767]</span>. The next lines have the description of the function <span class="tex-span"><i>f</i></span>. In the description can be found extra spaces and line breaks (see the examples) which, of course, can’t break key words int, if, return and numbers. The size of input data can’t exceed <span class="tex-span">100</span> bytes.</p>

## Output

<p>Output a single number — the answer to the problem. If there’s no answer, output "-1" (without quotes).</p>





```input1
17
int f(int n)
{
if (n &lt; 100) return 17;
if (n &gt; 99) return 27;
}

```




```input2
13
int f(int n)
{
if (n == 0) return 0;
return f(n - 1) + 1;
}

```




```input3
144
int f(int n)
{
if (n == 0) return 0;
if (n == 1) return n;
return f(n - 1) + f(n - 2);
}
```




```output1
99

```




```output2
13
```




```output3
24588

```


