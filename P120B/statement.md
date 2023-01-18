## Description

<div><p>A team quiz game called "What? Where? When?" is very popular in Berland. The game is centered on two teams competing. They are the team of six Experts versus the team of the Audience. A person from the audience asks a question and the experts are allowed a minute on brainstorming and finding the right answer to the question. All it takes to answer a typical question is general knowledge and common logic. The question sent be the audience are in envelops lain out in a circle on a round table. Each envelop is marked by the name of the asker's town. Each question is positioned in a separate sector. In the centre of the table is a spinning arrow. Thus, the table rather resembles a roulette table with no ball but with a spinning arrow instead. The host sets off the spinning arrow to choose a question for the experts: when the arrow stops spinning, the question it is pointing at is chosen. If the arrow points at the question that has already been asked, the host chooses the next unanswered question in the clockwise direction. Your task is to determine which will be the number of the next asked question if the arrow points at sector number <span class="tex-span"><i>k</i></span>.</p></div><div class="input-specification"><p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span> and <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>) — the numbers of sectors on the table and the number of the sector where the arrow is pointing. The second line contains <span class="tex-span"><i>n</i></span> numbers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span> if the question from sector <span class="tex-span"><i>i</i></span> has already been asked and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 1</span> if the question from sector <span class="tex-span"><i>i</i></span> hasn't been asked yet (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). The sectors are given in the clockwise order, the first sector follows after the <span class="tex-span"><i>n</i></span>-th one.</p></div><div class="output-specification"><p>Print the single number — the number of the sector containing the question the experts will be asked. It is guaranteed that the answer exists, that is that not all the questions have already been asked.</p></div>

## Input

<p>The first line contains two positive integers <span class="tex-span"><i>n</i></span> and <span class="tex-span"><i>k</i></span> (<span class="tex-span">1 ≤ <i>n</i> ≤ 1000</span> and <span class="tex-span">1 ≤ <i>k</i> ≤ <i>n</i></span>) — the numbers of sectors on the table and the number of the sector where the arrow is pointing. The second line contains <span class="tex-span"><i>n</i></span> numbers: <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 0</span> if the question from sector <span class="tex-span"><i>i</i></span> has already been asked and <span class="tex-span"><i>a</i><sub class="lower-index"><i>i</i></sub> = 1</span> if the question from sector <span class="tex-span"><i>i</i></span> hasn't been asked yet (<span class="tex-span">1 ≤ <i>i</i> ≤ <i>n</i></span>). The sectors are given in the clockwise order, the first sector follows after the <span class="tex-span"><i>n</i></span>-th one.</p>

## Output

<p>Print the single number — the number of the sector containing the question the experts will be asked. It is guaranteed that the answer exists, that is that not all the questions have already been asked.</p>





```input1
5 5
0 1 0 1 0

```




```input2
2 1
1 1

```




```output1
2

```




```output2
1

```


