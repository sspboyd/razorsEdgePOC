# Making a quick (and rough) prototype in Processing to test an idea...

I'm working on an(other) idea inspired by a Sol Lewitt wall drawing. This one is inspired by "Ifs Ands or Buts", 1973. Lewitt's drawing uses the simple instruction of "All ifs ands or buts connected by green lines". 

![Ifs Ands or Buts](https://pbs.twimg.com/media/BkkMUT4CQAAB2K8.jpg)

"Ifs Ands or Buts, 1973"

My variant of this idea is as follows:

1. Print the full text of Somerset Maugham's Razor's Edge on a wall. 

2. For each major character, find two mentions of the character's name in the text and connect them with a different coloured line for each.

3. The location of the names and number of connections is left to the choice of the executor (executioner?).

I like to create quick, small prototypes in Processing to see how an idea might look. I start with the most stripped down representation of an idea and build out from there. To figure out what to include in a stripped down version, I ask, "How much can I take away and still convey the idea?" For this drawing I really only need some small font-sized text on the screen and draw lines connecting a number of randomly located nodes. Crude, but quick and hopefully representative of the idea.

The quickest way to get some text was to grab a bit of [Lorem Ipsum online](http://www.lipsum.com/ "Lorem Ipsum generator") and copy paste it multiple times in a sketch that draws it to the screen. Easy. So far.

Next, create an array of randomly selected points on the screen, select two of the points and draw a line between them. Rinse wash and repeat about 100 times (repeat again with different number of lines to see what it looks like).

I liked what I saw so I kept going. Unfortunately, I didn't screenshot anything until later in the process. I wanted to replace the Lorem Ipsum with the real text. Understandably, the text for the book isn't freely available online. As a work around, I decided to use one of Arthur Conan Doyle's Sherlock Holmes stories which is available on Gutenburg (link).

Using a real text, the resulting image didn't look too much different but it had less of a homogenous quality than the Lorem Ipsum text. To improve on the fidelity of the prototype I wanted find the number of mentions and the x and y locations of the main characters, Sherlock and Watson, in the text. There was no immediately obvious/easy way to do this in Processing. Calulating the pixel position of a word-wrapped text is a trick I haven't learned yet. Processing is amazing for many things but in my experience text manipulation isn't one of them. 

In the spirit of creating a rough prototype I decided that a good workaround would be to figure out the number of mentions of "Watson" and "Holmes" in the text and then pick a corresponding number of random points for both characters. Not perfect, but progress. The vertical location of the points was aligned to the baseline of each line of text. 

Here's what it looks like.

!["Tall, thin version"](https://raw.githubusercontent.com/sspboyd/razorsEdgePOC/master/razorsEdgePOC-20150617003940rS47-.jpeg)!["Tall, thin version"](https://raw.githubusercontent.com/sspboyd/razorsEdgePOC/master/razorsEdgePOC-20150806010657rS47-.jpeg)
!["Landscape Version"](https://raw.githubusercontent.com/sspboyd/razorsEdgePOC/master/razorsEdgePOC-20150806011007rS47-.jpeg)
The tall thin versions were the first to be made. The original impetus for this sketch was to see how this idea would look on a wall in my house that is 49" x 92". 

This prototype works well enought to give me some confidence of what the 'real' version would look like. I write this however without knowing what a more fullsome execution based on the actual location of characters in the text would look like. The random selection of character locations looks interesting but I am more curious than ever to see what the real author determined locations would look like. 

The Processing code for this piece can be found [here on GitHub](https://github.com/sspboyd/razorsEdgePOC "Code available on GitHub").

If you look at the code, you'll notice I used character names from The Razor's Edge instead of Watson and Holmes. This was because I'd started the code before switching to using a Sherlock story. There's no need or benefit to switcg

I'll update this post when I figured out a reasonable way to get the x/y locations of the characters names in the text. Meanwhile, I decided that a real world prototype would be interesting to create too, so I printed out the full text of "A Scandal in Bohemia" on 14x11 sheets of paper and I started connecting names with a blue Bic pen and good ruler. I like this way too. It is a very slowly developing prototype but satisfying. (Images of this real world prototype are included too. {eventually})



