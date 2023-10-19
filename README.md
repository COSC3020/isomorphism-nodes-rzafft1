[![Open in Visual Studio Code](https://classroom.github.com/assets/open-in-vscode-718a45dd9cf7e7f842a935f5ebbe5719a5e09af4491e668f4dbf3b35d5cca122.svg)](https://classroom.github.com/online_ide?assignment_repo_id=12384029&assignment_repo_type=AssignmentRepo)
# Isomorphism

Prove that if two graphs $A$ and $B$ do not have the same number of nodes, they
cannot be isomorphic. I have started with the formal definition of isomorphism
below. Add your answer to this markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$G_1=(V_1 , E_1)$ is isomorphic to $G_2 = (V_2, E_2)$ if there exists a
one-to-one and onto function (bijection) $f: V_1 \rightarrow V_2$ such that $(u,v)
\in E_1$ iff $(f(u),f(v)) \in E_2$.

Proof

- if $G_1$ and $G_2$ have different numbers of nodes, then there must exists a node such that $(\exists u \in V_1)(\exists v \in V_2)(u \neq f(u))$

- In order for $G_1$ and $G_2$ to be isomorphic the relation between $G_1$ and $G_2$ must also be onto 

- $(\exists u \in V_1)(\exists v \in V_2)(u \neq f(u))$ shows that the required onto relation between $G_1$ and $G_2$ does not exists 

- The Onto function definition says that $(\forall v)(\forall u)$ { $ v \in V \implies v = f(u)$ } showing that if we have a node in $G_1$ and $G_1$ and $G_2$ are isomorphic, then a corresponding node must also exist in $G_2$

- As described above, there does not exist a node in $G_2$ such that  $v \in V \implies v = f(u)$

- Therefore, if $G_1$ has a size $n$ and $G_2$ has a size $m$ and $n \neq m \implies (\exists u \in V_1)(\exists v \in V_2)(u \neq f(u))$. Therefore $G_1$ and $G_2$ are NOT isomorphic
