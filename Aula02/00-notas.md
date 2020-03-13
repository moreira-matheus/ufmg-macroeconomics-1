## Modelo de Solow (1956)

**Características**:

1. Modelo com agregações (sem micro-fundamentação);
2. Baseado em uma função de produção;
3. Remuneração dos fatores equivale a sua produtividade marginal;
4. Rendimentos marginais decrescentes.

> Característica 3 se dá em um contexto de concorrência perfeita (em que as firmas não têm lucro).
>
> Características 3 e 4 estão relacionadas com a homogeneidade da função de produção.

**Crescimento do produto**:

- Acumulação dos fatores de produção:
  - $K$: capital (físico ou humano);
  - $L$: trabalho.
- Progresso tecnológico. 

> O progresso tecnológico em Solow é exógeno.

**Hipóteses do modelo**:

- Função de produção: $Y(t) = f\big[K(t), A(t)L(t) \big] \quad \textbf{(1)}$.

  - $A \cdot L$: trabalho efetivo (progresso técnico incorporado ao trabalho).

  - Função com retornos constantes de escala.

  - Função homogênea de grau 1: $f(cK, cAL) = c \cdot f(K, AL),\ c\geq 0 \quad\textbf{(2)}$.

    - Exemplo: [Cobb-Douglas](https://en.wikipedia.org/wiki/Cobb%E2%80%93Douglas_production_function).
      $$
      Y = f(K,AL) = K^{\alpha}(AL)^{1-\alpha}, \ \ 0 < \alpha < 1 \quad\textbf{(3)}
      $$
      Homogeneidade:
      $$
      \begin{align}
      f(cK,cAL) = &\ (cK)^{\alpha} (cAL)^{1-\alpha} \\
      = &\ c^{\alpha} K^{\alpha} c^{1-\alpha}(AL)^{1-\alpha} \\
      = &\ c K^{\alpha}(AL)^{1-\alpha}
      \end{align}
      $$

    - Na forma intensiva: seja $c = \displaystyle\frac{1}{AL}$, subst. em $\textbf{(2)}$:
      $$
      f\bigg(\displaystyle\frac{K}{AL},1\bigg) = \frac{1}{AL} f(K,AL) \quad\textbf{(5)}
      $$
      Subst. em $\textbf{(1)}$:
      $$
      \begin{align}
      \displaystyle\frac{1}{AL}Y &= \frac{1}{AL}f(K,AL) \\
      \displaystyle\frac{Y}{AL} &= f\bigg(\frac{K}{AL},1\bigg)
      \end{align}
      $$
      definam-se: $\displaystyle\frac{Y}{AL} = y;\ k = \frac{K}{AL}$.

      Na forma intensiva: $y = f(k,1) \Leftrightarrow y = f(k) \quad \textbf{(6)}$.

    - Propriedades de $\textbf{(6)}$:

      1. $f(0) = 0$ (começa na origem).
      2. $f'(k) > 0$ (sempre crescente).
      3. $f''(k) < 0$ (cresce a taxas decrescentes).

      > As propriedades 2 e 3 garantem a existência de um ponto máximo.

    - Limites de variações do estoque de capital na forma intensiva:

      1. $\displaystyle\lim_{k \rightarrow 0} f'(k) = \infty$.
      2. $\displaystyle\lim_{k\rightarrow \infty} f'(k) = 0$.

      > São chamadas condições de [Inada](https://en.wikipedia.org/wiki/Inada_conditions).

    - Exemplo: Cobb-Douglas.

      Forma intensiva: 
      $$
      \begin{align}
      Y = &\ K^{\alpha}(AL)^{1-\alpha} \\
      \displaystyle\frac{Y}{AL} = &\ y = f(k) = \bigg(\frac{K}{AL}\bigg)^{\alpha} \bigg(\frac{AL}{AL}\bigg)^{1-\alpha} 
      \Leftrightarrow y = k^\alpha \quad\textbf{(7)}
      \end{align}
      $$

      1. $y(k=0) = 0 \quad\checkmark$
      2. $y'(k) = \alpha k^{\alpha-1} > 0 \quad\checkmark$
      3. $y''(k) = -\alpha (1-\alpha) k^{\alpha-2} < 0 \quad\checkmark$
      4. $\displaystyle\lim_{k\rightarrow 0} y'(k) = \lim_{k\rightarrow 0} \alpha k^{\alpha-1} = \infty\ (\because 0 < \alpha < 1) \quad\checkmark$
      5. $\displaystyle\lim_{k\rightarrow \infty} y'(k) = \lim_{k\rightarrow \infty} \alpha k^{\alpha-1} = 0 \quad\checkmark$

**Fatores de produção**:

<u>Trabalho + tecnologia</u>: cresce a uma taxa constante.

- $\displaystyle\frac{d}{dt} L(t) = \dot{L}(t) = nL(t) \quad\textbf{(8)}$

  - "A força de trabalho é determinada por uma taxa constante e exógena": $n$.

- $\displaystyle\frac{d}{dt} A(t) = \dot{A}(t) = gA(t) \quad\textbf{(9)}$

  - $g$: taxa de "crescimento" do progresso tecnológico (constante e exógena).

- Podemos calcular essas taxas a partir dos logaritmos:
  $$
  \begin{align}
  \displaystyle\frac{d}{dt}\big(\ln L(t)\big) = &\ \frac{d}{d L(t)}\big(\ln L(t)\big) \cdot \frac{d}{dt}L(t) \\
  = &\ \frac{1}{L(t)} \dot{L}(t) \Rightarrow \frac{\dot{L}(t)}{L(t)} = n \quad\textbf{(10)}
  \end{align}
  $$
  ou seja: $d \ln L(t) = n\ dt$.

  Se a diferença do log natural é igual à taxa de crescimento $\bigg(\ln L(1) - \ln L(0) = n\bigg)$, podemos aplicar isso para qualquer período:
  $$
  \begin{align}
  &\ln L(1) = \ln L(0) + n \\
  &\ln L(2) = \ln L(1) + n = \ln L(0) + 2n \\
  &\dots \\
  &\ln L(t) = \ln L(0) + n\cdot t \quad \textbf{(11)} \\ \\
  &\ln A(t) = \ln A(0) + g\cdot t \quad \textbf{(12)}
  \end{align}
  $$
  Voltando aos valores em nível de variáveis:
  $$
  L(t) = L(0)\cdot\exp\{nt\} \quad\textbf{(13)} \\
  A(t) = A(0)\cdot\exp\{gt\} \quad\textbf{(14)}
  $$
  Conclusão: trabalho e conhecimento crescem exponencialmente a partir de valores iniciais.

<u>Capital</u>: depende do investimento e da depreciação.

- Poupança: $S = sY(t)$.

  - $s$: taxa de poupança (exógena e constante).

- Vale a [lei de Say](https://en.wikipedia.org/wiki/Say%27s_law): $S=I$ (poupança é iguala investimento).

  - Modelo de Solow pressupõe causalidade: *investimento depende de poupança prévia*.

- Taxa de depreciação $\delta$: constante e exógena.

  - $n + g +\delta > 0$.

- Dinâmica do modelo:
  $$
  \displaystyle\frac{d}{dt}K(t) = \dot{K}(t) = sY(t) - \delta K(t) \quad\textbf{(15)}
  $$
  Na forma intensiva $k = \displaystyle\frac{K}{AL}$:
  $$
  \begin{align}
  \displaystyle\frac{d}{dt}\bigg(\frac{K}{AL}\bigg) = \dot{k}(t) = &\ \frac{K'(t)\big(A(t)L(t)\big) - K(t)\big(A(t)L(t)\big)'}{\big(A(t)L(t)\big)^2} \\
  = &\ \frac{\dot K(t)}{A(t)L(t)} - \frac{K(t)}{\big(A(t)L(t)\big)^2} \big[A(t) \dot L(t) + \dot A(t) L(t)\big] \\
  = &\ \frac{\dot K(t)}{A(t)L(t)} - \frac{K(t)}{A(t)L(t)}\cdot \frac{\dot L(t)}{L(t)} - \frac{K(t)}{A(t)L(t)}\cdot \frac{\dot A(t)}{A(t)} \quad\textbf{(16)}
  \end{align}
  $$
  Subst. $\textbf{(8)}$, $\textbf{(9)}$ e $\textbf{(10)}$ em $\textbf{(16)}$:
  $$
  \begin{align}
  \dot k(t) = &\ \displaystyle\frac{sY(t) - \delta K(t)}{A(t)L(t)} - k(t) \cdot n - k(t) \cdot g \\
  = &\ \frac{sY(t)}{A(t)L(t)} - \delta k(t) - n k(t) - g k(t) \\
  = &\ sy(t) - (n + g + \delta) k(t) \quad\textbf{(18)}
  \end{align}
  $$
  onde $y(t) = f\big(k(t)\big) = \displaystyle\frac{Y}{AL}$.

***

### Leituras complementares:

- ACEMOGLU, Daron. Economic Growth and Economic Development: The Questions. In: ____. "**Introduction to Modern Economic Growth**“. Department of Economics, Massachusetts Institute of Technology, 2007. p. 3-25.
- SIMON, Carl P. et al. Homogeneous and Homothetic Functions. In: ____. **Mathematics for economists**. New York: Norton, 1994. p. 483-504.