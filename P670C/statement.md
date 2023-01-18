## Description

<div><p>Moscow is hosting a major international conference, which is attended by <span class="tex-span"><i>n</i></span> scientists from different countries. Each of the scientists knows exactly one language. For convenience, we enumerate all languages of the world with integers from <span class="tex-span">1</span> to <span class="tex-span">10<sup class="upper-index">9</sup></span>.</p><p>In the evening after the conference, all <span class="tex-span"><i>n</i></span> scientists decided to go to the cinema. There are <span class="tex-span"><i>m</i></span> movies in the cinema they came to. Each of the movies is characterized by two <span class="tex-font-style-bf">distinct</span> numbers&nbsp;— the index of audio language and the index of subtitles language. The scientist, who came to the movie, will be <span class="tex-font-style-it">very pleased</span> if he knows the audio language of the movie, will be <span class="tex-font-style-it">almost satisfied</span> if he knows the language of subtitles and will be <span class="tex-font-style-it">not satisfied</span> if he does not know neither one nor the other (note that the audio language and the subtitles language for each movie are always different). </p><p>Scientists decided to go together to the same movie. You have to help them choose the movie, such that the number of very pleased scientists is maximum possible. If there are several such movies, select among them one that will maximize the number of almost satisfied scientists.</p></div><div class="input-specification"><p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of scientists.</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the index of a language, which the <span class="tex-span"><i>i</i></span>-th scientist knows.</p><p>The third line contains a positive integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the number of movies in the cinema. </p><p>The fourth line contains <span class="tex-span"><i>m</i></span> positive integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> is the index of the audio language of the <span class="tex-span"><i>j</i></span>-th movie.</p><p>The fifth line contains <span class="tex-span"><i>m</i></span> positive integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> is the index of subtitles language of the <span class="tex-span"><i>j</i></span>-th movie.</p><p>It is guaranteed that audio languages and subtitles language are different for each movie, that is <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub> ≠ <i>c</i><sub class="lower-index"><i>j</i></sub></span>. </p></div><div class="output-specification"><p>Print the single integer&nbsp;— the index of a movie to which scientists should go. After viewing this movie the number of very pleased scientists should be maximum possible. If in the cinema there are several such movies, you need to choose among them one, after viewing which there will be the maximum possible number of almost satisfied scientists. </p><p>If there are several possible answers print any of them.</p></div>

## Input

<p>The first line of the input contains a positive integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 200 000</span>)&nbsp;— the number of scientists.</p><p>The second line contains <span class="tex-span"><i>n</i></span> positive integers <span class="tex-span"><i>a</i><sub class="lower-index">1</sub>, <i>a</i><sub class="lower-index">2</sub>, ..., <i>a</i><sub class="lower-index"><i>n</i></sub></span> (<span class="tex-span">1 ≤ <i>a</i><sub class="lower-index"><i>i</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the index of a language, which the <span class="tex-span"><i>i</i></span>-th scientist knows.</p><p>The third line contains a positive integer <span class="tex-span"><i>m</i></span> (<span class="tex-span">1 ≤ <i>m</i> ≤ 200 000</span>)&nbsp;— the number of movies in the cinema. </p><p>The fourth line contains <span class="tex-span"><i>m</i></span> positive integers <span class="tex-span"><i>b</i><sub class="lower-index">1</sub>, <i>b</i><sub class="lower-index">2</sub>, ..., <i>b</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>b</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub></span> is the index of the audio language of the <span class="tex-span"><i>j</i></span>-th movie.</p><p>The fifth line contains <span class="tex-span"><i>m</i></span> positive integers <span class="tex-span"><i>c</i><sub class="lower-index">1</sub>, <i>c</i><sub class="lower-index">2</sub>, ..., <i>c</i><sub class="lower-index"><i>m</i></sub></span> (<span class="tex-span">1 ≤ <i>c</i><sub class="lower-index"><i>j</i></sub> ≤ 10<sup class="upper-index">9</sup></span>), where <span class="tex-span"><i>c</i><sub class="lower-index"><i>j</i></sub></span> is the index of subtitles language of the <span class="tex-span"><i>j</i></span>-th movie.</p><p>It is guaranteed that audio languages and subtitles language are different for each movie, that is <span class="tex-span"><i>b</i><sub class="lower-index"><i>j</i></sub> ≠ <i>c</i><sub class="lower-index"><i>j</i></sub></span>. </p>

## Output

<p>Print the single integer&nbsp;— the index of a movie to which scientists should go. After viewing this movie the number of very pleased scientists should be maximum possible. If in the cinema there are several such movies, you need to choose among them one, after viewing which there will be the maximum possible number of almost satisfied scientists. </p><p>If there are several possible answers print any of them.</p>





```input1
3
2 3 2
2
3 2
2 3

```




```input2
6
6 3 1 1 3 7
5
1 2 3 4 5
2 3 4 5 1

```




```output1
2

```




```output2
1

```



## Note

<p>In the first sample, scientists must go to the movie with the index <span class="tex-span">2</span>, as in such case the <span class="tex-span">1</span>-th and the <span class="tex-span">3</span>-rd scientists will be very pleased and the <span class="tex-span">2</span>-nd scientist will be almost satisfied.</p><p>In the second test case scientists can go either to the movie with the index <span class="tex-span">1</span> or the index <span class="tex-span">3</span>. After viewing any of these movies exactly <span class="tex-font-style-bf">two</span> scientists will be very pleased and all the others will be not satisfied. </p>
