---
layout: page
title: Various
publish: true
---

- Heisenberg operators:

    $$ \begin{equation*}
          
            \begin{array} {rcl}
              \displaystyle \hat{x}_H (t)
                  & = & \displaystyle \hat{x} \cos \omega t + \frac{\hat{p}}{m \omega} \sin \omega t \\
                \displaystyle \hat{p}_H (t) 
                    & = & \displaystyle \hat{p} \cos \omega t - m \omega \hat{x} \sin \omega t  \\ 
                \displaystyle A_H (t) 
                    & = & \displaystyle \mathcal{U}^\dagger (t, 0) A_S \mathcal{U} (t, 0) \\
                    & = & \displaystyle e^{\frac{i}{\hbar} \hat{H} t} A_S e^{-\frac{i}{\hbar} \hat{H} t} \\
                \displaystyle \hat{a}(t) = \hat{a}_H(t) 
                    & = & \displaystyle e^{-i \omega t} \hat{a} \\
                \displaystyle \hat{a}^\dagger(t) = \hat{a}_H^\dagger(t) 
                    & = & \displaystyle e^{i \omega t} \hat{a}^\dagger \\
                \displaystyle \hat{x}
                    & = & \displaystyle \sqrt{\frac{\hbar}{2 m \omega}} (\hat{a} + \hat{a}^\dagger) \\
                \displaystyle \hat{p}
                    & = & \displaystyle i \sqrt{\frac{m \hbar \omega}{2}} (\hat{a}^\dagger - \hat{a}) \\
            \end{array}
          
        \end{equation*}
    $$

- Identity:

    $$ \begin{equation*}
          \braket{x | p} = \frac{e^{ipx}}{\sqrt{2\pi \hbar}}
        \end{equation*}
    $$

- Translation (unitary) operator $T_{x_0}$:

    $$ \begin{equation*}
        T_{x_0} \equiv e^{-\frac{i}{\hbar} \hat{p} x_0}
        \end{equation*}
    $$

    $$ \begin{equation*}
          \braket{x}_{T_{x_0}\psi} = \bra{\psi}T_{x_0}^\dagger \hat{x} T_{x_0} \ket{\psi} = \bra{\psi} \hat{x} + x_0 \ket{\psi} = \braket{x} + x_0
        \end{equation*}
    $$

    $$ \begin{equation*}
          
            \begin{array} {rcl}
              \displaystyle T_{x_0} \ket{x_1} 
                  & = & \displaystyle \ket{x_1 + x_0} \\
                \displaystyle T_{x_0}^\dagger \ket{x_1} 
                    & = & \displaystyle \ket{x_1 - x_0} \\
                \displaystyle \bra{x_1 | T_{x_0}} 
                    & = & \displaystyle \bra{x_1 - x_0} \\
            \end{array}
          
        \end{equation*}
    $$

    $$ \begin{equation*}
          
            \begin{array} {rcl}
              \displaystyle T_{x_0} \braket{x| T_{x_0}|\psi} 
                  & = & \displaystyle \braket{x - x_0 | \psi} \\
                  & = & \displaystyle \psi(x - x_0) \\
            \end{array}
          
        \end{equation*}
    $$

- Coherent state:

    $$ \begin{equation*}
          \ket{x_0}_c \equiv T_{x_0} \ket{0} = e^{-\frac{i}{\hbar} \hat{p} x_0} \ket{0}
        \end{equation*}
    $$

    where $\ket{0}$ denotes the ground state of the oscillator.

    The wave function $\psi_{x_0}$ associated to the coherent state is easily obtained:

    $$ \begin{equation*}
          \psi_{x_0}(x) = \braket{x | x_0}_c = \braket{x|T_{x_0}|0} = \braket{x - x_0 | 0} = \varphi_0(x - x_0)
        \end{equation*}
    $$

    where we used $\braket{x|0} = \varphi_0(x)$ is the ground state wave
function.

    Expectations in a coherent state:

    $$ \begin{equation*}
          
            \begin{array} {rcl}
              \displaystyle {}_{c}\braket{x_0|\hat{x}|x_0}_c 
                  & = & \displaystyle x_0 \\
              \displaystyle {}_{c}\braket{x_0|\hat{p}|x_0}_c 
                  & = & 0 \\
              \displaystyle {}_{c}\braket{x_0|\hat{H}|x_0}_c
                  & = & \displaystyle \frac{1}{2} \hbar \omega + \frac{1}{2} m \omega^2 x_0^2 \\
              \displaystyle {}_{c}\braket{x_0|\hat{x}^2|x_0}_c
                  & = & \displaystyle x_0^2 + \frac{\hbar}{2 m \omega}  \\
              \displaystyle {}_{c}\braket{x_0|\hat{p}^2|x_0}_c
                  & = & \displaystyle  \frac{m\hbar\omega}{2}  \\
              \displaystyle {}_{c}\braket{x_0|\hat{x}\hat{p}+\hat{p}\hat{x}|x_0}_c
                  & = & 0  \\
                  

            \end{array}
          
        \end{equation*}
    $$

- Time-dependent expectation values:

    $$ \begin{equation*}
          
            \begin{array} {rcl}
              \displaystyle \braket{\hat{x}}_{x_0}(t) 
                  & = & \displaystyle {}_{c}\braket{x_0, t | \hat{x} | x_0, t}_c \\
                  & = & \displaystyle {}_c\braket{x_0 | \hat{x}_H(t) | x_0}_c \\
                  & = & \displaystyle {}_c\braket{x_0 | \left( \hat{x} \cos \omega t + \frac{1}{m\omega} \hat{p} \sin \omega t \right)  | x_0 } {}_c \\
                  & = & \displaystyle x_0 \cos \omega t

                  \\ \\ 

            \displaystyle \braket{\hat{p}}_{x_0}(t)
                & = & \displaystyle -m \omega x_0 \sin \omega t
            \end{array}
          
        \end{equation*}
    $$

- Time-dependent position and momentum uncertainties:

    $$ \begin{equation*}
          
            \begin{array} {rcl}
              \displaystyle (\Delta x )^2
                  & = & \displaystyle \frac{1}{2} L_0^2 \quad \text{on the state}\, \ket{x_0}_c

                  \\ \\

              \displaystyle (\Delta p )^2
                  & = & \displaystyle \frac{1}{2} \left(\frac{\hbar}{L_0}\right)^2  \quad \text{on the state}\, \ket{x_0}_c

                  \\ 

              \displaystyle L_0 
                & = & \displaystyle \sqrt{\frac{\hbar}{m \omega}} \quad \text{is the ground state length}

                  \\ \\
            \end{array}
          
        \end{equation*}
    $$

- Commutator identities:

    $$ \begin{equation*}
          
            \begin{array} {rcl}
              \displaystyle e^{A+B} 
                  & = & \displaystyle e^{A}e^{B}e^{-\frac{1}{2}[A,B]} \quad \text{if}\, [A,[A,B]] = [B,[A,B]] = 0 \\
              \displaystyle [A, e^{B}] 
                  & = & \displaystyle [A, B] e^{B} \quad \text{if}\, [[A,B], B] = 0 \\
            \end{array}
          
        \end{equation*}
    $$

- Creation and annihilation operators:

    $$ \begin{equation*}
          
            \begin{array} {rcl}
              \displaystyle \hat{a} 
                  & = & \displaystyle \sqrt{\frac{m \omega}{2 \hbar}} \left( \hat{x} + \frac{i}{m \omega} \hat{p} \right) \\ \\
              \displaystyle \hat{a}^\dagger 
                  & = & \displaystyle \sqrt{\frac{m \omega}{2 \hbar}} \left( \hat{x} - \frac{i}{m \omega} \hat{p} \right) \\ \\
              \displaystyle [\hat{a}, \hat{a}^\dagger]
                  & = & \displaystyle 1 \\ \\
                \displaystyle \hat{H} 
                    & = & \displaystyle \hbar \omega \left( \hat{a}^\dagger \hat{a} + \frac{1}{2} \right) \\ \\
                \displaystyle \hat{N}   
                    & = & \displaystyle \hat{a}^\dagger \hat{a} \\ \\
                \displaystyle [\hat{N}, \hat{a}^\dagger] 
                    & = & \displaystyle \hat{a}^\dagger \\ \\
                \displaystyle [\hat{N}, \hat{a}] 
                    & = & \displaystyle  - \hat{a} \\ \\
                \displaystyle [\hat{N}, (\hat{a}^\dagger)^k] 
                    & = & \displaystyle k (\hat{a}^\dagger)^k \\ \\
                \displaystyle [\hat{N}, (\hat{a})^k] 
                    & = & \displaystyle   - k (\hat{a})^k \\ \\
                \displaystyle [\hat{a}^\dagger, (\hat{a})^k] 
                    & = & \displaystyle  -k (\hat{a})^{k-1} \\ \\
                \displaystyle [\hat{a}, (\hat{a}^\dagger)^k] 
                    & = & \displaystyle   k (\hat{a}^\dagger)^{k-1} \\ \\
                \displaystyle \ket{n} 
                    & \equiv & \displaystyle  \frac{1}{\sqrt{n!}} (\hat{a}^\dagger)^n \ket{0} \\ \\
                \displaystyle \hat{a}\ket{n} 
                    & = & \displaystyle \sqrt{n} \ket{n-1} \\ \\
                \displaystyle \hat{a}^\dagger\ket{n} 
                    & = & \displaystyle  \sqrt{n+1} \ket{n+1} \\ \\
            \end{array}
          
        \end{equation*}
    $$

- $\hat{x}$ and $\hat{p}$ in terms of $\hat{a}^\dagger$, $\hat{a}$ and $L_0$:

    $$ \begin{equation*}
          
            \begin{array} {rcl}
              \displaystyle \hat{p} 
                  & = & \displaystyle \frac{i}{\sqrt{2}} \frac{\hbar}{L_0} (\hat{a}^\dagger - \hat{a}) \\ \\
              \displaystyle \hat{x} 
                  & = & \displaystyle \frac{L_0}{\sqrt{2}} (\hat{a} + \hat{a}^\dagger) \\
            \end{array}
          
        \end{equation*}
    $$

- Coherent state

    $$ \begin{equation*}
          \ket{x_0}_c = \exp \left( -\frac{i\hat{p} x_0}{\hbar} \right) \ket{0} = \exp \left( -\frac{1}{4} \frac{x_0^2}{L_0^2} \right) \exp \left( \frac{x_0}{\sqrt{2}L_o} \hat{a}^\dagger \right) \ket{0}
        \end{equation*}
    $$

    or

    $$ \begin{equation*}
          \ket{x_0}_c = \sum_{n=0}^\infty c_n \ket{n}, \quad \text{with}\, c_n = \exp \left( -\frac{1}{4} \frac{x_0^2}{L_0^2} \right) \frac{1}{\sqrt{n!}} \left( \frac{x_0}{\sqrt{2}L_o} \right)^n
        \end{equation*}
    $$

    Probability $P_n$ of finding the energy $\displaystyle E_n = \hbar \omega \left( n+\frac{1}{2} \right) $:

    $$ \begin{equation*}
          P_n = |c_n|^2 = \exp \left( -\frac{1}{2} \frac{x_0^2}{L_0^2} \right) \frac{1}{n!} \left( \frac{x_0^2}{2L_o^2} \right)^n
        \end{equation*}
    $$

    or

    $$ \begin{equation*}
          P_n = \frac{\lambda^n}{n!} e^{-\lambda}, \quad \text{with}\, \lambda \equiv \frac{x_0^2}{2L_o^2}
        \end{equation*}
    $$

- Expectation value of $n$:

    $$ \begin{equation*}
            \braket{n} = \sum_{n=0}^\infty n P_n = \lambda = \frac{x_0^2}{2L_o^2}
        \end{equation*}
    $$

- Expectation value of $n^2$:
    
    $$ \begin{equation*}
            \braket{n^2} = \sum_{n=0}^\infty n^2 P_n = \lambda^2 + \lambda = \frac{x_0^4}{4L_o^4} + \frac{x_0^2}{2L_o^2}
        \end{equation*}
    $$

- Uncertainty in $n$:

    $$ \begin{equation*}
            (\Delta n)^2 = \braket{n^2} - \braket{n}^2 = \lambda^2 + \lambda - \lambda^2 = \lambda = \frac{x_0^2}{2L_o^2}
        \end{equation*}
    $$

- Expectation value of energy $E$:

    $$ \begin{equation*}
            \braket{E} = \sum_{n=0}^\infty E_n P_n = \hbar \omega \left( \frac{1}{2} + \lambda \right) = \frac{1}{2} \hbar \omega + \frac{1}{2} m \omega^2 x_0^2
        \end{equation*}
    $$

- Uncertainty in energy $E$:

    $$ \begin{equation*}
            (\Delta E) = \hbar \omega \sqrt{\lambda} = \hbar \omega \frac{x_0}{\sqrt{2}L_o}
        \end{equation*}
    $$

    Note that for large $\lambda$ the average energy is much higher than the uncertainty in energy:

    $$ \begin{equation*}
            \frac{\braket{E}}{(\Delta E)} = \sqrt{\lambda} + \frac{1}{2\sqrt{\lambda}} \simeq \sqrt{\lambda}
        \end{equation*}
    $$

- Arbitrary coherent state $\ket{\alpha}$:

    $$ \begin{equation*}
          
            \begin{array} {rcl}
                \displaystyle \ket{\alpha} 
                    & \equiv & \displaystyle D(\alpha) \ket{0} \\
                    & = & \displaystyle \exp \left( \alpha \hat{a}^\dagger - \alpha^* \hat{a} \right) \ket{0}, \quad\text{with}\, \alpha \in \mathbb{C} \\
                \displaystyle D(\alpha) 
                    & = & \displaystyle \exp \left( \alpha \hat{a}^\dagger - \alpha^* \hat{a} \right) \\  \\
                \displaystyle \hat{a}\ket{\alpha} 
                    & = & \displaystyle \alpha \ket{\alpha} \\ \\
                    
                \displaystyle \braket{\alpha|\hat{x}|\alpha} 
                    & = & \displaystyle L_0 \sqrt{2} \operatorname{Re}(\alpha) \\
                \displaystyle \implies \operatorname{Re}(\alpha)
                    & = & \displaystyle \frac{1}{\sqrt{2}} \frac{\braket{\hat{x}}_\alpha}{L_0} \\ \\
                    
                \displaystyle \braket{\alpha|\hat{p}|\alpha} 
                    & = & \displaystyle \sqrt{2} \frac{\hbar}{L_0} \operatorname{Im}(\alpha) \\
                \displaystyle \implies \operatorname{Im}(\alpha)
                    & = & \displaystyle \frac{1}{\sqrt{2}} \frac{L_0}{\hbar} \braket{\hat{p}}_\alpha \\ \\

                \displaystyle \implies \alpha
                    & = & \displaystyle \frac{1}{\sqrt{2}} \left( \frac{\braket{\hat{x}}_\alpha}{L_0} + i \frac{L_0\braket{\hat{p}}_\alpha}{\hbar} \right) \\ \\ 

                \displaystyle \ket{\alpha}
                    & = & \displaystyle \exp \left( -\frac{i\hat{p}\braket{\hat{x}}_\alpha}{\hbar} + \frac{i\braket{\hat{p}}_\alpha\hat{x}}{\hbar} \right) \ket{0} \\ \\

                \displaystyle \ket{\alpha, t}
                    & = & e^{-i\omega t/2} \ket{ e^{-i\omega t} \alpha } \\ \\

            \end{array}
          
        \end{equation*}
    $$

- Integral of Gamma function

    $$ \begin{equation*}
          \int_0^\infty e^{-u} u^n \, du = n!
        \end{equation*}
    $$