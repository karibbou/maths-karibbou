---
date: 2021-06-05
title: Définitions et premiers résultats
type: book
---



{{< thm/thm type="definition" name="Somme partielle, série, série convergente" label="" >}} 

Soit $(u_n)$ une suite. <br>On appelle "somme partielle " la suite $S_n = \sum_{k=0}^n u_k$. La série associée est la suite $(S_n)$, qu'on note alors  $\sum_{n \geq 0}u_n$ ou encore  $\sum u_n$. 

On dit que la série converge si $(S_n)$ converge. Dans ce cas, on pourra écrire $\lim_{n \rightarrow +\infty} S_n = \sum^{\infty}_{k=0}u_k$.<br>

Dans le cas où elle ne convergerait pas, on dira qu'elle diverge.

{{< /thm/thm >}}

{{< thm/thm type="theoreme" name="critère de Cauchy" label="" >}} 

La série $\sum u_n$ converge si et seulement si : $\forall \varepsilon > 0, \exists N \in \mathbb{N}$ tel que $\forall n \geq m \geq N$ on a $|{\sum_{k=m}^n u_k} |\leq \varepsilon$

{{< /thm/thm >}}



{{< thm/thm type="theoreme" name="condition nécessaire de convergence" label=" >}} 

Si la série $\sum u_n$ converge, alors $\lim_{n \rightarrow +\infty}u_n  = 0$ 

{{< /thm/thm >}}





