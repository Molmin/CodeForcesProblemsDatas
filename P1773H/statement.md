## Description

<div><p>This is an interactive problem.</p><p>After emigrating to another country, little Hanna came across the fact that playing "Hot and cold" became more difficult: she does not understand the hint phrases! You are to write a helping program for her.</p><p>The playground where the game happens is a rectangle, and the treasure is hidden in some point with integer coordinates between 0&nbsp;and&nbsp;$10^6$, inclusive. Hanna visits several points with valid coordinates. If&nbsp;the visited point contains the hidden treasure, she receives the phrase "Found!" in the local language. Fortunately, the intonations allow her to recognize this phrase&nbsp;— in this problem it will be denoted by an exclamation mark.</p><p>Otherwise, for each visited point except for the first one, Hanna receives a phrase in the local language stating whether she is now "Closer", "Further", or "At the same distance" from the treasure, compared to the previous point. The distances are measured in Euclidean metric. After the first visited point, in case of no treasure there, Hanna receives the phrase "Not found" in the local language.</p><p>Your program must help Hanna find the treasure by visiting <span class="tex-font-style-bf">at most 64 points</span>.</p></div><div><h2>Interaction</h2><p>Your program should print each visited point in a line with two coordinates between 0&nbsp;and&nbsp;$10^6$, inclusive, and flush the output after each one.</p><p>For each visited point, the testing system writes one of the phrases: "Found!", "Closer", "Further", "At the same distance", or "Not found" in some language, consistent throughout the game. The first phrase ends with an exclamation mark, all other phrases do not contain exclamation marks. All phrases contain only Latin letters, spaces and exclamation marks, have lengths between 2 and 30, inclusive, don't start or end with a space, and are pairwise distinct. The phrases are not necessarily coming from any real human language. </p><p>After receiving a phrase with an exclamation mark, your program must halt without printing anything else. Visiting points more than once is allowed, and each such visit counts towards the limit of 64 queries.</p></div>





```input1
Tabilmadi

Daha yakin

Daha yakin

Sama distanco

Dalej

Znaydeno!
```




```input2
You are lucky today!
```




```output1
500 200

560 230

566 240

566 238

30 239

566 239
```




```output2
777777 777777
```


