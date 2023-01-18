## Description

<div><p>Om Nom is the main character of a game "Cut the Rope". He is a bright little monster who likes visiting friends living at the other side of the park. However the dark old parks can scare even somebody as fearless as Om Nom, so he asks you to help him.</p><center> <img class="tex-graphics" src="file://uyIFLlWD.png" style="max-width: 100.0%;max-height: 100.0%;"> </center><p>The park consists of <span class="tex-span">2<sup class="upper-index"><i>n</i> + 1</sup> - 1</span> squares connected by roads so that the scheme of the park is a full binary tree of depth <span class="tex-span"><i>n</i></span>. More formally, the entrance to the park is located at the square <span class="tex-span">1</span>. The exits out of the park are located at squares <span class="tex-span">2<sup class="upper-index"><i>n</i></sup>, 2<sup class="upper-index"><i>n</i></sup> + 1, ..., 2<sup class="upper-index"><i>n</i> + 1</sup> - 1</span> and these exits lead straight to the Om Nom friends' houses. From each square <span class="tex-span"><i>i</i></span> (<span class="tex-span">2 ≤ <i>i</i> &lt; 2<sup class="upper-index"><i>n</i> + 1</sup></span>) there is a road to the square <img align="middle" class="tex-formula" src="file://f7gZ5vYG.png" style="max-width: 100.0%;max-height: 100.0%;">. Thus, it is possible to go from the park entrance to each of the exits by walking along exactly <span class="tex-span"><i>n</i></span> roads. </p><center> <img class="tex-graphics" src="file://dqFUk1Hp.png" style="max-width: 100.0%;max-height: 100.0%;"> </center> To light the path roads in the evening, the park keeper installed street lights along each road. The road that leads from square <span class="tex-span"><i>i</i></span> to square <img align="middle" class="tex-formula" src="file://Yo9mAeWE.png" style="max-width: 100.0%;max-height: 100.0%;"> has <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> lights.<p>Om Nom loves counting lights on the way to his friend. Om Nom is afraid of spiders who live in the park, so he doesn't like to walk along roads that are not enough lit. What he wants is that the way to any of his friends should have in total the same number of lights. That will make him feel safe. </p><p>He asked you to help him install additional lights. Determine what minimum number of lights it is needed to additionally place on the park roads so that a path from the entrance to any exit of the park contains the same number of street lights. You may add an arbitrary number of street lights to each of the roads.</p></div><div class="input-specification"><p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>) — the number of roads on the path from the entrance to any exit.</p><p>The next line contains <span class="tex-span">2<sup class="upper-index"><i>n</i> + 1</sup> - 2</span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ... <i>a</i><sub class="lower-index">2<sup class="upper-index"><i>n</i> + 1</sup> - 1</sub></span> — the initial numbers of street lights on each road of the park. Here <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of street lights on the road between squares <span class="tex-span"><i>i</i></span> and <img align="middle" class="tex-formula" src="file://3xBNmu7b.png" style="max-width: 100.0%;max-height: 100.0%;">. All numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are positive integers, not exceeding <span class="tex-span">100</span>.</p></div><div class="output-specification"><p>Print the minimum number of street lights that we should add to the roads of the park to make Om Nom feel safe.</p></div>

## Input

<p>The first line contains integer <span class="tex-span"><i>n</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 10</span>) — the number of roads on the path from the entrance to any exit.</p><p>The next line contains <span class="tex-span">2<sup class="upper-index"><i>n</i> + 1</sup> - 2</span> numbers <span class="tex-span"><i>a</i><sub class="lower-index">2</sub>, <i>a</i><sub class="lower-index">3</sub>, ... <i>a</i><sub class="lower-index">2<sup class="upper-index"><i>n</i> + 1</sup> - 1</sub></span> — the initial numbers of street lights on each road of the park. Here <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> is the number of street lights on the road between squares <span class="tex-span"><i>i</i></span> and <img align="middle" class="tex-formula" src="file://3xBNmu7b.png" style="max-width: 100.0%;max-height: 100.0%;">. All numbers <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub></span> are positive integers, not exceeding <span class="tex-span">100</span>.</p>

## Output

<p>Print the minimum number of street lights that we should add to the roads of the park to make Om Nom feel safe.</p>





```input1
2
1 2 3 4 5 6

```




```output1
5

```



## Note

<p>Picture for the sample test. Green color denotes the additional street lights.</p><center> <img class="tex-graphics" src="file://nA933DXq.png" style="max-width: 100.0%;max-height: 100.0%;"> </center>
