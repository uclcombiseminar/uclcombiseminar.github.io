---
layout: post
speaker: Debsoumya Chakraborti
speaker-url: https://sites.google.com/view/debsoumya
speaker-uni: University of Warwick
title: 22 January 2024
subtitle: Bandwidth theorem for graph transversals

excerpt_separator: <!--more-->
---
The bandwidth of a graph is the minimum $b$ such that 
there is a labeling of the vertex set of $H$ by 
the numbers $1,2,\ldots,n$ with $|i-j|\le b$ 
for every edge $ij$ of $H$. The celebrated bandwidth theorem
states that if $H$ is an $n$-vertex graph with chromatic number $r$,
bounded maximum degree, and bandwidth $o(n)$, then every $n$-vertex 
graph with minimum degree at least $\left(1-\frac{1}{r}+o(1)\right)n$ 
contains a copy of $H$. This minimum degree is best possible up to the $o(1)$ term.

Recently, there have been systematic studies extending spanning subgraph problems
to the setting of transversals over a collection of graphs. 
Given a graph-collection $\mathcal{G}=\{G_1,\dots, G_h\}$ with the same vertex set $V$,
an $h$-edge graph $H$ on the vertex set $V$ is a $\mathcal{G}$-transversal 
if there exists a bijection $\lambda : E(H) \rightarrow \{1,\ldots,h\}$ such that 
$e\in E(G_{\lambda(e)})$ for each $e\in E(H)$. 
The minimum degree condition $\delta(\mathcal{G})=\min\{ \delta(G_i)\}$ 
for finding a spanning $\mathcal{G}$-transversal $H$ have been actively 
studied when $H$ is a Hamilton cycle, an $F$-factor, 
a tree with maximum degree $o(n/\log n)$, and power of Hamilton cycles, etc.

Generalizing both these results and the original bandwidth theorem, 
we obtain asymptotically sharp minimum degree conditions for graphs 
with bounded degree and sublinear bandwidth, proving the bandwidth theorem
for graph transversals. This talk is based on joint work 
with Seonghyuk Im, Jaehoon Kim, and Hong Liu.

<!--more-->
