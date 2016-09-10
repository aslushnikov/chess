# Chess.js [[play]](https://aslushnikov.github.io/chess/)

![chess.js](/screenshot.png?raw=true "Chess.js")

In 2011 I was suggested to write a web version of chess with AI, from scratch and in two days.
The AI had to be strong enough to overcome an average player. 
In case of success, a reward of $1000 was promised.

I didn't know much of js, but managed to fit in the deadlines and got the reward.

Today, the money are long gone, but I'm still proud of the AI which won over
a lot of my friends. \m/

### AI

To make a move, AI traverses the tree of all possible moves. The deeper traversal goes,
the more powerful AI is, and the more time it takes to make a move.

The maximum traversal depth is defined by the `AI.oa` variable (the code is minified; unfotunately, I lost
the sources). The default value is 3 (which means, it will go 3 half-moves deep).

To increase AI power, open DevTools console and run the following snippet:
```
AI.oa = 4
```

This is not very convenient, but I didn't make the complexity switch back in the days. Today, I'd like to keep this code untouched as a memory :)
