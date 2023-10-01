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

- Commutator identity:

    $$ \begin{equation*}
          
            \begin{array} {rcl}
              \displaystyle e^{A+B} 
                  & = & \displaystyle e^{A}e^{B}e^{-\frac{1}{2}[A,B]} \quad \text{if}\, [A,[A,B]] = [B,[A,B]] = 0
            \end{array}
          
        \end{equation*}
    $$