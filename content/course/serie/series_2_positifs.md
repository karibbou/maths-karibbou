---
title: Séries à termes positifs
summary: Le cas le plus simple dans l'étude des séries ! On établit ici des critères auxquels on va souvent se ramener.
date: '2021-06-04'
type: book
---

On va établir quelques critères de convergence plus evolués que les quelques conditions qu'on à vu précédemment.

Pour cela, on va chercher à se ramener à l'étude la plus simple à mener, celle pour des séries à terme général réel positif.

{{< thm/thm type="proposition" name="" label="" >}}

On suppose que $(u_n)$ est réelle et positive. Alors $\sum u_n$ converge si et seulement si la suite des sommes partielles $s_N = \sum_{n=0}^N u_n$ est bornée.

{{< /thm/thm >}}

## Des critères pour les séries à termes positifs:

{{< thm/thm type="theorem" name="Critère de convergence par comparaison" label="Critère de convergence par comparaison" >}}

Soient $(a_n), (b_n)$ des suites réelles positives. Si $a_n \leq b_n$ pour presque tout n alors : <br>

 * si $\sum b_n$ est convergente, il en est de même pour $\sum a_n$

* Si $\sum a_n$ est divergente, il en est de même pour $\sum b_n$

{{< /thm/thm >}}

{{< thm/thm type="theorem" name="Critère de convergence par équivalence" label="Critère de convergence par équivalence" >}}

Soient $(a_n)$ et $(b_n)$ des suites réelles positives. Si $a_n \sim b_n$, alors $\sum a_n$ et $\sum b_n$ sont de même nature.

{{< /thm/thm >}}

## Comment faire pour des séries quelconques ?

Dans le cas où l'on devrait étudier une série $\sum a_n$ à terme générale complexe ou réelle (positifs ou négatifs), on peut alors se ramener à l'étude de la série $\sum |a_n|$ :

{{< thm/thm type="définition" name="Convergence absolue" label="Convergence absolue" >}}

On dira que  $\sum a_n$  est absolument convergente si  $\sum |a_n|$  est convergente.

{{< /thm/thm >}}

{{< thm/thm type="lemma" name="La convergence absolue implique la convergence" label="La convergence absolue implique la convergence" >}}

Si  $\sum a_n$  est absolument convergente, alors elle converge.

{{< /thm/thm >}}

### Quelques critères liés à l'absolue convergence

{{< thm/thm type="theorem" name="Critère de Cauchy" label="Critère de Cauchy" >}}

On suppose qu'il existe $\rho \in [0, 1[$ tel que pour presque tout $n \in \mathbb{N}, \sqrt[n]{|a_n}| \leq \rho$ alors  $\sum a_n$ converge. <br>
En particulier, si $\lim_{n \rightarrow +\infty} \sqrt[n]{|a_n}| < 1$ alors $\sum a_n$ converge.

{{< /thm/thm >}}

{{< thm/thm type="theorem" name="Critère de D'Alembert" label="Critère de D'Alembert" >}}

On suppose qu'il existe $\rho \in [0, 1[$ tel que pour presque tout $n \in \mathbb{N}, |\frac{a_{n+1}}{a_n}| \leq \rho$, alors  $\sum a_n$ converge. <br>
En particulier, si $\lim_{n \rightarrow +\infty} |\frac{a_{n+1}}{a_n}| < 1$ alors $\sum a_n$ converge.

{{< /thm/thm >}}

## La réponse à une grande question:

L'ordre dans lequel on somme les termes d'une série a-t-il un impact sur la convergence de la série ?<br>Plus formellement, si $\sum a_n$ converge, est-ce que pour chaque bijection $\sigma: \mathbb{N} \longrightarrow \mathbb{N}$ la série $\sum a_{\sigma(n)}$ (qu'on appelle "réarrangement de $\sum a_n$") est convergente ? <br> On pourrait penser que oui puisque l'addition est commutatif mais la réponse est en fait plus complexe.

{{< thm/thm type="theorem" name="Théorème de réarrangement de Dirichlet" label="Théorème de réarrangement de Dirichlet" >}}

Soit $\sum a_n$ une série absolument convergente et a limite $l$. Alors tout réarrangement $\sum a_{\sigma(n)}$ est absolument convergent et a pour limite $l$.

{{< /thm/thm >}}

Sans la condition d'absolue convergence, la convergence des réarrangement n'est plus garantie !

{{< thm/thm type="theorem" name="Théorème de Riemann" label="Théorème de Riemann" >}}

Soit $\sum a_n$ une série à terme réelle et convergente. Alors pour tout $l \in \mathbb{R} \cup \{+\infty\}\cup\{-\infty\}$, il existe un réarrangement $\sum a_{\sigma(n)}$ ayant pour limite $l$.

{{< /thm/thm >}}