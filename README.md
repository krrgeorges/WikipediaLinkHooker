## Project Description

[![GPLv3 License](https://img.shields.io/badge/License-GPL%20v3-yellow.svg)](https://opensource.org/licenses/) [![Version](https://badge.fury.io/gh/tterb%2FHyde.svg)](https://badge.fury.io/gh/tterb%2FHyde)


### WikipediaLinkHooker

WikipediaLinkHooker is a utility tool thats allows for improvement of content quality through adding wikipedia links to a word(eg: Geology) or group of words(Battle of the Bulge) if an article about a word or a group of words exists


### Why should I use this?

Wikipedia has become a primary source of information for millions across the globe. A person might want to know in detail about a particular topic referred in your content text. This script can help in assisting and satisfying the curiosity of the person.


### Requirements

Requires Python -v > 3.r.0 

### Using WikipediaLinkHooker

Import the script and execute the following

```python
content = 'World War II (often abbreviated as WWII or WW2), also known as the Second World War, was a global war that lasted from 1939 to 1945. The vast majority of the world's countries—including all the great powers—eventually formed two opposing military alliances: the Allies and the Axis. A state of total war emerged, directly involving more than 100 million people from more than 30 countries. The major participants threw their entire economic, industrial, and scientific capabilities behind the war effort, blurring the distinction between civilian and military resources. World War II was the deadliest conflict in human history, marked by 70 to 85 million fatalities, most of whom were civilians in the Soviet Union and China. It included massacres, genocides (including the Holocaust), strategic bombing, premeditated death from starvation and disease, and the only use of nuclear weapons in war.'
window_size = 4
wiki_hooked = WikipediaLinkHooker(content,window_size).hook()
```
window_size is the number of words to be considered for consideration of hooking (4 is optimal).

wiki_hooked will be a dictionary containing the html and the references to the page for the word or group of words.
