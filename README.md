# Asymptotic Equivalences

In the lectures, we said that logarithms with different bases don't affect the
asymptotic complexity of an algorithm. Prove that $O(\log_{2} n)$ is the same as
$O(\log_{5} n)$. Use the mathematical definition of $O$ -- do a formal proof,
not just the intuition.

I have started with the formal definition of $O$ below. Add your answer to this
markdown file. [This
page](https://docs.github.com/en/get-started/writing-on-github/working-with-advanced-formatting/writing-mathematical-expressions)
might help with the notation for mathematical expressions.

$T(n) \in O(f(n)) \iff \exists c, n_0: T(n) \leq c \cdot f(n) \forall n \geq n_0$

1st half:

chnage of base formula:
$$\log_{5}(n) =\frac{\log_{2}(n)}{\log_{2}(5)}$$

$$\log_{2}(n) =\log_{5}(n) * \log_{2}(5)$$

Since $\log_2(5)$ is a positive constant, there exists some $c_1 = \log_2(5)$ such that:

$$\log_{2}(n) =c_1 * \log_{5}(n) $$
$$\equiv \log_{2}(n) \leq c_1 * \log_{5}(n) $$

which is the $T(n) \leq c \cdot f(n)$...

2nd half:
$$\log_{5}(n) =\frac{\log_{2}(n)}{\log_{2}(5)}$$

Since $\frac{1}{\log_2(5)}$ is a positive constant, there exists some $c_2 = \frac{1}{\log_2(5)}$ such that:
$$\log_{5}(n) =c_2 * \log_{2}(n) $$
$$\equiv \log_{5}(n) \leq c_2 * \log_{2}(n) $$
which is the other side of the bi-implication.

I certify that I have listed all sources used to complete this exercise, including the use of any Large Language Models. All of the work is my own, except where stated otherwise. I am aware that plagiarism carries severe penalties and that if plagiarism is suspected, charges may be filed against me without prior notice.