---
title: "The Document Title"
author: [Example Author, Another Author]
date: 2017-02-20
tags: [Markdown, Example]
...

1. Level one heading
	- a bullet point
	* another bullet point
	+ yet another... you guessed it... a bullet point
	- pick your poison

#. It is smart enough to figure out the numbering for you.
	- pretty crazy

#. You can just throw math whereever you like
	$$
	\frac{a}{b} = \frac{c}{d} + \frac{e}{f}
	$$

	- Single line $\frac{a}{b}$ why not 

#. Look, an alphabetical sublist:
	a) whoa
	b) trippy

#. Let's put a graph. Hope it works!
\begin{figure}[H]
   \centering
   \begin{tikzpicture}
   \node[vertex] (a) at  (0,0) {};
   \node[vertex] (b) at  (4,3) {};
   \node[vertex] (c) at  (8,0) {};
   \node[vertex] (d) at  (4,-3) {$t$};
   \node[vertex] (a1) at (1.5,0) {};
   \node[vertex] (a2) at (3,0) {};
   \draw[edge] (b) to (a);
   \draw[edge] (b) to (c);
   \draw[edge] (a) to (d);
   \draw[edge] (c) to (d);
   
   \draw[edge] (a)  to[bend left] (a1);
   \draw[edge] (a1) to[bend left] (a);
   
   \draw[edge] (a1) to[bend left] (a2);
   \draw[edge] (a2) to[bend left] (a1);
   
   \path (a2) to node {\dots} (c);
   \node [shape=circle,minimum size=1.5em] (a3) at (4.5,0) {};
   \draw[edge] (a2) to[bend left] (a3);
   \draw[edge] (a3) to[bend left] (a2);
   
   \node [shape=circle,minimum size=1.5em] (c1) at (6.5,0) {};
   \draw[edge] (c) to[bend left] (c1);
   \draw[edge] (c1) to[bend left] (c);
   \end{tikzpicture}
\end{figure}
