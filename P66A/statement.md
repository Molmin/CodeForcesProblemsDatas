## Description

<div><p>Little Petya has recently started attending a programming club. Naturally he is facing the problem of choosing a programming language. After long considerations he realized that Java is the best choice. The main argument in favor of choosing Java was that it has a very large integer data type, called BigInteger.</p><p>But having attended several classes of the club, Petya realized that not all tasks require using the BigInteger type. It turned out that in some tasks it is much easier to use small data types. That's why a question arises: "Which integer type to use if one wants to store a positive integer <span class="tex-span"><i>n</i></span>?"</p><p>Petya knows only 5 integer types:</p><p>1) <span class="tex-font-style-bf">byte</span> occupies 1 byte and allows you to store numbers from <span class="tex-span"> - 128</span> to <span class="tex-span">127</span></p><p>2) <span class="tex-font-style-bf">short</span> occupies 2 bytes and allows you to store numbers from <span class="tex-span"> - 32768</span> to <span class="tex-span">32767</span></p><p>3) <span class="tex-font-style-bf">int</span> occupies 4 bytes and allows you to store numbers from <span class="tex-span"> - 2147483648</span> to <span class="tex-span">2147483647</span></p><p>4) <span class="tex-font-style-bf">long</span> occupies 8 bytes and allows you to store numbers from <span class="tex-span"> - 9223372036854775808</span> to <span class="tex-span">9223372036854775807</span></p><p>5) <span class="tex-font-style-bf">BigInteger</span> can store any integer number, but at that it is not a primitive type, and operations with it are much slower.</p><p>For all the types given above the boundary values are included in the value range.</p><p>From this list, Petya wants to choose the smallest type that can store a positive integer <span class="tex-span"><i>n</i></span>. Since BigInteger works much slower, Peter regards it last. Help him.</p></div><div class="input-specification"><p>The first line contains a positive number <span class="tex-span"><i>n</i></span>. It consists of no more than <span class="tex-span">100</span> digits and doesn't contain any leading zeros. The number <span class="tex-span"><i>n</i></span> can't be represented as an empty string.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p></div><div class="output-specification"><p>Print the first type from the list "<span class="tex-font-style-tt">byte</span>, <span class="tex-font-style-tt">short</span>, <span class="tex-font-style-tt">int</span>, <span class="tex-font-style-tt">long</span>, <span class="tex-font-style-tt">BigInteger</span>", that can store the natural number <span class="tex-span"><i>n</i></span>, in accordance with the data given above.</p></div>

## Input

<p>The first line contains a positive number <span class="tex-span"><i>n</i></span>. It consists of no more than <span class="tex-span">100</span> digits and doesn't contain any leading zeros. The number <span class="tex-span"><i>n</i></span> can't be represented as an empty string.</p><p>Please, do not use <span class="tex-font-style-tt">%lld</span> specificator to read or write 64-bit integers in C++. It is preffered to use <span class="tex-font-style-tt">cout</span> (also you may use <span class="tex-font-style-tt">%I64d</span>).</p>

## Output

<p>Print the first type from the list "<span class="tex-font-style-tt">byte</span>, <span class="tex-font-style-tt">short</span>, <span class="tex-font-style-tt">int</span>, <span class="tex-font-style-tt">long</span>, <span class="tex-font-style-tt">BigInteger</span>", that can store the natural number <span class="tex-span"><i>n</i></span>, in accordance with the data given above.</p>





```input1
127

```




```input2
130

```




```input3
123456789101112131415161718192021222324

```




```output1
byte

```




```output2
short

```




```output3
BigInteger

```


