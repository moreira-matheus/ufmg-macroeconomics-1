SIMON, Carl P. et al. **Mathematics for economists**. New York: Norton, 1994.

### **Chapter 20: Homogeneous and Homothetic Functions**

**Definition and Examples**

<u>Definition</u>: For any scalar $k$, a real-valued function $f(x_1, ..., x_n)$ is **homogeneous of degree** $k$ if:
$$
f(tx_1, \dots, tx_n) = t^k f(x_1, \dots, x_n),\quad \forall x_1, \dots, x_n;\ \forall t>0 \quad\textbf{(1)}
$$

- Examples:

1. $x_1^{2} x_2 + 3x_1 x_2^{2} + x_{2}^{3}$ is homogeneous of degree three, since each term is homogeneous of degree three.

   - Replacing $x_1, x_2, x_3$ by $tx_1, tx_2,tx_3$:
     $$
     \begin{align}
     (tx_1)^2(tx_2) + 3(tx_1)(tx_2)^2 + (tx_2)^3 = &\ t^2 x_1^{2} t x_2 + 3 tx_1 t^2x_{2}^{2} + t^3x_{2}^{3} \\
     = &\ t^3 \big( x_1^2 x_2 + 3x_1x_2^2 +x_2^3 \big) \quad\blacksquare
     \end{align}
     $$

2. $x_1^{7}x_2 x_3^2 + 5x_1^6 - x_2^5 x_3^5$ is homogeneous of degree ten, since each term is homogeneous of degree ten.

   - Replacing $x_1, x_2, x_3$ by $tx_1, tx_2,tx_3$:
     $$
     \begin{align}
     (tx_1)^7 (tx_2) (tx_3)^2 + (tx_1)^6(tx_2)^4 + (tx_2)^5(tx_3)^5 & \\
     = &\ t^{10}\big( x_1^{7}x_2 x_3^2 + 5x_1^6 - x_2^5 x_3^5 \big) \quad\blacksquare
     \end{align}
     $$

3. $4x_1^2 - 5x_1x_2^2$ is *not* homogeneous since the first term has degree five and the second has degree three.

4. A linear function $z = \displaystyle\sum_i a_i x_i$ is homogeneous of degree one.

5. A quadratic form $z = \displaystyle\sum_{i,j} a_{ij} x_i x_j$ is homogeneous of degree two.

6. The function $f_1(x_1,x_2) = 30x_1^{1/2}x_2^{3/2} - 2x_1^3 x_2^{-1}$ is homogeneous of degree two.

7. The function $f_2(x_1,x_2) = x_{1}^{1/2} x_2^{1/4} + x_1^{2}x_2^{-5/4}$ is homogeneous of degree three-quarters.

8. The function $f_3(x_1,x_2) = \displaystyle\frac{x_1^7 - 3x_1^2 x_2^5}{x_1^4 + 2x_1^2 x_2^2 + x_2^4}$ is homogeneous of degree three.

- However, the only homogeneous functions of one variable are the functions of the form $z = ax^k,\ \forall k\in\R$.
  - To prove this statement, let $z=f(x)$ be an arbitrary homogeneous function of one variable.
  - Let $a \equiv f(1)$ and let $x$ be arbitrary.
  - Then, $f(x) = f(x\cdot 1) = x^k f(1) = ax^k$.

**Homogeneous Functions in Economics**

Economists often find it convenient to work with homogeneous functions as production functions.

- For example, if $q = f(x_1, \dots, x_n)$ is production function which is homogeneous fo degree one, then:
  $$
  f(tx_1, \dots, tx_n) = t f(x_1, \dots, x_n) \quad\textbf{(2)}
  $$
  for all input bundles $(x_1, \dots, x_n)$ and all $t > 0$.

  - Taking $t=2$, eq. $\textbf{(2)}$ says that if the firm doubles all inputs, it doubles its output too.
    - For $t=3$, if it triples each input, it triples the corresponding output.
    - Such a firm is said to exhibit **constant returns to scale**.
  - Suppose, on the other hand, the production function is homogeneous of degree $k>1$.
    - If such a firm were to double the amount of each input, its output would rise by a factor of $2^k$.
    - Since $k>1$, its output would more than double.
    - Such a firm is said to exhibit **increasing returns to scale**.
  - Finally, a firm which has a production function that is homogeneous of degree $k<1$, will have its output increase by a factor less than two when it doubles all its inputs.
    - Such a firm exhibits **decreasing returns to scale**.

A specific homogeneous functional form which economists frequently use as a production or utility function is the **Cobb-Douglas function**:
$$
q = A x_{1}^{a_1} x_{2}^{a_2} \cdots x_{n}^{a_n}, \quad\textbf{(3)}
$$
a monomial with exponents $a_1, \dots, a_n$ that are usually positive fractions.

- Economists interested in estimating the production function of a specific firm or industry will often try to find the Cobb-Douglas production function which best fits the firm's input-output data.
  - They can often use linear ordinary least squares techniques since by taking the logarithm of both sides of function $\textbf{(3)}$, they can work with the log of the output as linear function of the logs of the inputs: $\log q = \log A + a_1 \log x_1 + \cdots + a_n \log x_n$.
- Notice that a Cobb Douglas production function exhibits decreasing, constant, or increasing returns to scale according to whether the sum of its exponents is less than, equal to, or greater than $1$.
  - Economists have usually found in their empirical studies that this sum is very close to $1$.

While production functions are often homogeneous *by assumption*, demand functions are homogeneous *by nature* (at least if we ignore the "[money illusion](https://www.investopedia.com/terms/m/money_illusion.asp)").

- Recall that a demand function $\mathbf{x} = D(\mathbf{p}, I)$ associates to each price vector $\mathbf{p} = (p_1, \dots, p_n)$ and income level $I$, an individual's most-preferred consumption bundle $\mathbf x$ at those prices and income.
  - It is the solution of the basic consumer maximization problem: $\mathbf{x} = D(\mathbf p, I)$ maximizes $U(\mathbf x)$ subject to the constraints $x_i \geq 0,\ \forall i$ and $\mathbf p \cdot \mathbf x \leq I \ \textbf{(4)}$.
  - Notice that if all the prices and the consumer's income tripled, constraint $\textbf{(4)}$ would not change.
    - We could just divide the new inequality through by $3$ to return to the original inequality.
- In terms of demand function: $D(t\mathbf{p}, tI) = D(\mathbf p, I),\ \forall \mathbf p, I \ \textbf{(5)}$.
  - Since $t^0 = 1$, eq. $\textbf{(5)}$ states that demand is homogeneous of degree $0$ in $\mathbf p$ and $I$.
  - Since each individual demand function is homogeneous of degree zero, the sum of these individual demands, aggregate demand, is also homogeneous of degree zero.

Finally, a similar, straightforward calculation shows that for a firm in a competitive market, the (minimal) cost function is a homogeneous function of input prices and the optimal function is a homogeneous function of output price.

***