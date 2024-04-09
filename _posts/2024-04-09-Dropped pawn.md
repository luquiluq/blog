---
title: 
date: 2024-04-09
---

Some days ago I was watching a chess game and took note of a nice position that came up. Later that day, I came across my young sister.

"Elva", I said to her, "look at this board from today's game. White to move. How odd it is!"; to which she answered, sharp as always, "It doesn't seem to have lasted long. Mate in one.". Didn't even blink!

Below's the board that I showed Elva. A pawn is missing (but only from the board below, i.e. Elva saw the complete board).

![The board](https://raw.githubusercontent.com/luquiluq/blog/main/docs/assets/comosicion_ajedrez.png)

- Can you determine where the missing pawn was?
- How did Elva spot the mate in one?

<details>
<summary>The solution</summary>
The only possibility is for a white pawn to be on <code>d5</code> and to capture black's pawn on <code>d4</code> <em>en passant</em>. But how did Elva see that such a move was legal? Her only information was the full board and the fact that it came from a true game. Elva must have thought backwards to deduce that black's last move was a 2-square push of the e pawn. Let's then answer this question: <em>what was black's last move?</em>
<ul>
  <li>Clearly black didn't move the bishop.</li>
  <li>They neither moved the king as it would have previously been in a double check.</li>
  <li>The last move must have been <code>...e5</code>, <code>...exf6</code> or <code>...gxf6</code>. In the first case, only a 2-square push would have been possible (note white king's position). Now, the other two moves are impossible: a simple way to see this is that black has already captured exactly two white pieces, because there are 14 white pieces on the board. Moreover, those two captures were accomplished by the pawn on <code>a4</code>. Why? Well, of course that pawn of course must belong to the column <code>c</code> or some posterior one, so it has to have hopped at least twice diagonally. So the last piece to move can't have been the pawn on <code>f6</code>. The only possibility is a 2-square pawn push that allows for <em>en passant</em>.</li>
</ul>
</details>



