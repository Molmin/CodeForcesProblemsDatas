## Description

<div><p>A kindergarten teacher Natalia Pavlovna has invented a new ball game. This game not only develops the children's physique, but also teaches them how to count. </p><p>The game goes as follows. Kids stand in circle. Let's agree to think of the children as numbered with numbers from <span class="tex-span">1</span> to <span class="tex-span"><i>n</i></span> clockwise and the child number <span class="tex-span">1</span> is holding the ball. First the first child throws the ball to the next one clockwise, i.e. to the child number <span class="tex-span">2</span>. Then the child number <span class="tex-span">2</span> throws the ball to the next but one child, i.e. to the child number <span class="tex-span">4</span>, then the fourth child throws the ball to the child that stands two children away from him, i.e. to the child number <span class="tex-span">7</span>, then the ball is thrown to the child who stands <span class="tex-span">3</span> children away from the child number <span class="tex-span">7</span>, then the ball is thrown to the child who stands <span class="tex-span">4</span> children away from the last one, and so on. It should be mentioned that when a ball is thrown it may pass the beginning of the circle. For example, if <span class="tex-span"><i>n</i> = 5</span>, then after the third throw the child number <span class="tex-span">2</span> has the ball again. Overall, <span class="tex-span"><i>n</i> - 1</span> throws are made, and the game ends.</p><p>The problem is that not all the children get the ball during the game. If a child doesn't get the ball, he gets very upset and cries until Natalia Pavlovna gives him a candy. That's why Natalia Pavlovna asks you to help her to identify the numbers of the children who will get the ball after each throw.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) which indicates the number of kids in the circle.</p></div><div class="output-specification"><p>In the single line print <span class="tex-span"><i>n</i> - 1</span> numbers which are the numbers of children who will get the ball after each throw. Separate the numbers by spaces.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">2 ≤ <i>n</i> ≤ 100</span>) which indicates the number of kids in the circle.</p>

## Output

<p>In the single line print <span class="tex-span"><i>n</i> - 1</span> numbers which are the numbers of children who will get the ball after each throw. Separate the numbers by spaces.</p>





```input1
10

```




```input2
3

```




```output1
2 4 7 1 6 2 9 7 6

```




```output2
2 1

```


