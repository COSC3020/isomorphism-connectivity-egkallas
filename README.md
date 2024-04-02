[![Review Assignment Due Date](https://classroom.github.com/assets/deadline-readme-button-24ddc0f5d75046c5622901739e7c5dd533143b0c8e959d652212380cedb1ea36.svg)](https://classroom.github.com/a/QM7QGF1q)
# Isomorphism

Prove that if two graphs $A$ and $B$ are isomorphic they do *not* have to
be completely connected. I have started with the formal definition of
isomorphism below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

Consider the graph $G_1$:
<br>
$V$  $E$<br>
$A | B$<br>
$B | A$<br>
$C | D$<br>
$D | C$<br>
<br>
Consider the graph $G_2$:<br>
$V$  $E$<br>
$W | X$<br>
$X | W$<br>
$Y | Z$<br>
$Z | Y$<br>
<br>

Lemma: Bijectivity ($V_1 \rightarrow V_2$)<br>
$f(A) = W$<br>
$f(B) = X$<br>
$f(C) = Y$<br>
$f(D) = Z$<br>
This prooves every node in $G_1$ can be mapped to a unique node in $G_2$.

Lemma: Edge correspondence ($(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$)<br>

$(A, B) \in E_1 \rightarrow (W, X) \ E_2$<br>
$(C, D) \in E_1 \rightarrow (Y, Z) \ E_2$<br>
This prooves that for every edge $(u,v)$ in $G_1$ there is a corresponding edge $(f(u),f(v))$ in $G_2$.<br>
$\therefore G_1$ and $G_2$ are isomorphic.<br>

The graphs however are not connected because there is no edge from the $A$ / $B$ nodes to the $C$ / $D$ nodes in $G_1$, and there is no edge from the $W$ / $X$ nodes to the $Y$ / $Z$ nodes in $G_2$.<br>
$QED$
