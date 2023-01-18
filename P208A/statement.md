## Description

<div><p>Vasya works as a DJ in the best Berland nightclub, and he often uses dubstep music in his performance. Recently, he has decided to take a couple of old songs and make dubstep remixes from them.</p><p>Let's assume that a song consists of some number of words. To make the dubstep remix of this song, Vasya inserts a certain number of words "<span class="tex-font-style-tt">WUB</span>" before the first word of the song (the number may be zero), after the last word (the number may be zero), and between words (at least one between any pair of neighbouring words), and then the boy glues together all the words, including "<span class="tex-font-style-tt">WUB</span>", in one string and plays the song at the club.</p><p>For example, a song with words "<span class="tex-font-style-tt">I AM X</span>" can transform into a dubstep remix as "<span class="tex-font-style-tt">WUBWUBIWUBAMWUBWUBX</span>" and cannot transform into "<span class="tex-font-style-tt">WUBWUBIAMWUBX</span>".</p><p>Recently, Petya has heard Vasya's new dubstep track, but since he isn't into modern music, he decided to find out what was the initial song that Vasya remixed. Help Petya restore the original song.</p></div><div class="input-specification"><p>The input consists of a single non-empty string, consisting only of uppercase English letters, the string's length doesn't exceed <span class="tex-span">200</span> characters. It is guaranteed that before Vasya remixed the song, no word contained substring "<span class="tex-font-style-tt">WUB</span>" in it; Vasya didn't change the word order. It is also guaranteed that initially the song had at least one word.</p></div><div class="output-specification"><p>Print the words of the initial song that Vasya used to make a dubsteb remix. Separate the words with a space.</p></div>

## Input

<p>The input consists of a single non-empty string, consisting only of uppercase English letters, the string's length doesn't exceed <span class="tex-span">200</span> characters. It is guaranteed that before Vasya remixed the song, no word contained substring "<span class="tex-font-style-tt">WUB</span>" in it; Vasya didn't change the word order. It is also guaranteed that initially the song had at least one word.</p>

## Output

<p>Print the words of the initial song that Vasya used to make a dubsteb remix. Separate the words with a space.</p>





```input1
WUBWUBABCWUB

```




```input2
WUBWEWUBAREWUBWUBTHEWUBCHAMPIONSWUBMYWUBFRIENDWUB

```




```output1
ABC
```




```output2
WE ARE THE CHAMPIONS MY FRIEND
```



## Note

<p>In the first sample: "<span class="tex-font-style-tt">WUBWUBABCWUB</span>" = "<span class="tex-font-style-tt">WUB</span>" + "<span class="tex-font-style-tt">WUB</span>" + "<span class="tex-font-style-tt">ABC</span>" + "<span class="tex-font-style-tt">WUB</span>". That means that the song originally consisted of a single word "<span class="tex-font-style-tt">ABC</span>", and all words "<span class="tex-font-style-tt">WUB</span>" were added by Vasya.</p><p>In the second sample Vasya added a single word "<span class="tex-font-style-tt">WUB</span>" between all neighbouring words, in the beginning and in the end, except for words "<span class="tex-font-style-tt">ARE</span>" and "<span class="tex-font-style-tt">THE</span>" — between them Vasya added two "<span class="tex-font-style-tt">WUB</span>".</p>
