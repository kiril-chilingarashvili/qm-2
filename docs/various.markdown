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
          \braket{x \mid  p} = \frac{e^{ipx}}{\sqrt{2\pi \hbar}}
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
                \displaystyle \bra{x_1 \mid  T_{x_0}} 
                    & = & \displaystyle \bra{x_1 - x_0} \\
            \end{array}
          
        \end{equation*}
    $$

    $$ \begin{equation*}
          
            \begin{array} {rcl}
              \displaystyle T_{x_0} \braket{x\mid  T_{x_0}\mid \psi} 
                  & = & \displaystyle \braket{x - x_0 \mid  \psi} \\
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
          \psi_{x_0}(x) = \braket{x \mid  x_0}_c = \braket{x\mid T_{x_0}\mid 0} = \braket{x - x_0 \mid  0} = \varphi_0(x - x_0)
        \end{equation*}
    $$

    where we used $\braket{x\mid 0} = \varphi_0(x)$ is the ground state wave
function.

    Expectations in a coherent state:

    $$ \begin{equation*}
          
            \begin{array} {rcl}
              \displaystyle {}_{c}\braket{x_0\mid \hat{x}\mid x_0}_c 
                  & = & \displaystyle x_0 \\
              \displaystyle {}_{c}\braket{x_0\mid \hat{p}\mid x_0}_c 
                  & = & 0 \\
              \displaystyle {}_{c}\braket{x_0\mid \hat{H}\mid x_0}_c
                  & = & \displaystyle \frac{1}{2} \hbar \omega + \frac{1}{2} m \omega^2 x_0^2 \\
              \displaystyle {}_{c}\braket{x_0\mid \hat{x}^2\mid x_0}_c
                  & = & \displaystyle x_0^2 + \frac{\hbar}{2 m \omega}  \\
              \displaystyle {}_{c}\braket{x_0\mid \hat{p}^2\mid x_0}_c
                  & = & \displaystyle  \frac{m\hbar\omega}{2}  \\
              \displaystyle {}_{c}\braket{x_0\mid \hat{x}\hat{p}+\hat{p}\hat{x}\mid x_0}_c
                  & = & 0  \\
                  

            \end{array}
          
        \end{equation*}
    $$

- Time-dependent expectation values:

    $$ \begin{equation*}
          
            \begin{array} {rcl}
              \displaystyle \braket{\hat{x}}_{x_0}(t) 
                  & = & \displaystyle {}_{c}\braket{x_0, t \mid  \hat{x} \mid  x_0, t}_c \\
                  & = & \displaystyle {}_c\braket{x_0 \mid  \hat{x}_H(t) \mid  x_0}_c \\
                  & = & \displaystyle {}_c\braket{x_0 \mid  \left( \hat{x} \cos \omega t + \frac{1}{m\omega} \hat{p} \sin \omega t \right)  \mid  x_0 } {}_c \\
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
          P_n = \mid c_n\mid ^2 = \exp \left( -\frac{1}{2} \frac{x_0^2}{L_0^2} \right) \frac{1}{n!} \left( \frac{x_0^2}{2L_o^2} \right)^n
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
                    
                \displaystyle \braket{\alpha\mid \hat{x}\mid \alpha} 
                    & = & \displaystyle L_0 \sqrt{2} \operatorname{Re}(\alpha) \\
                \displaystyle \implies \operatorname{Re}(\alpha)
                    & = & \displaystyle \frac{1}{\sqrt{2}} \frac{\braket{\hat{x}}_\alpha}{L_0} \\ \\
                    
                \displaystyle \braket{\alpha\mid \hat{p}\mid \alpha} 
                    & = & \displaystyle \sqrt{2} \frac{\hbar}{L_0} \operatorname{Im}(\alpha) \\
                \displaystyle \implies \operatorname{Im}(\alpha)
                    & = & \displaystyle \frac{1}{\sqrt{2}} \frac{L_0}{\hbar} \braket{\hat{p}}_\alpha \\ \\

                \displaystyle \implies \alpha
                    & = & \displaystyle \frac{1}{\sqrt{2}} \left( \frac{\braket{\hat{x}}_\alpha}{L_0} + i \frac{L_0\braket{\hat{p}}_\alpha}{\hbar} \right) \\ \\ 

                \displaystyle \ket{\alpha}
                    & = & \displaystyle \exp \left( -\frac{i\hat{p}\braket{\hat{x}}_\alpha}{\hbar} + \frac{i\braket{\hat{p}}_\alpha\hat{x}}{\hbar} \right) \ket{0} \\ \\

                \displaystyle \ket{\alpha, t}
                    & = & e^{-i\omega t/2} \ket{ e^{-i\omega t} \alpha } \\ \\

                \displaystyle \frac{1}{\pi} \int d^2\alpha \ket{\alpha}\bra{\alpha}
                    & = & \displaystyle \mathbb{1} \\ \\

                \displaystyle \frac{1}{2\pi\hbar} \int \mathop{d x_0} \mathop{d p_0} \ket{x_0, p_0}\bra{x_0, p_0}
                    & = & \displaystyle \mathbb{1} \\ \\

            \end{array}
          
        \end{equation*}
    $$

- Integral of Gamma function

    $$ \begin{equation*}
          \int_0^\infty e^{-u} u^n \, du = n!
        \end{equation*}
    $$

- Property of a trace:

    $$ \begin{equation*}
          \operatorname{tr}\left( \ket{u}\bra{v} \right) = \braket{v \mid  u}
        \end{equation*}
    $$

- Squeezed vacuum states

    $$ \begin{equation*}
          \begin{aligned}
            & H_1=\frac{p^2}{2 m_1}+\frac{1}{2} m_1 \omega_1^2 x^2 \\ 
            & \Delta x=\sqrt{\frac{\hbar}{2 m_1 \omega_1}} \\
            & \Delta p=\sqrt{\frac{\hbar m_1 \omega_1}{2}} \\
            & \Delta x=\sqrt{\frac{m_2 \omega_2}{m_1 \omega_1}} \sqrt{\frac{\hbar}{2 m_2 \omega_2}} = e^{-\gamma} \sqrt{\frac{\hbar}{2 m_2 \omega_2}} \\
            & \Delta p=\sqrt{\frac{m_1 \omega_1}{m_2 \omega_2}} \sqrt{\frac{\hbar m_2 \omega_2}{2}} = e^\gamma \sqrt{\frac{\hbar m_2 \omega_2}{2}} \\
            & e^\gamma \equiv \sqrt{\frac{m_1 \omega_1}{m_2 \omega_2}} \\
            & \hat{a}_1=\hat{a}_2 \cosh \gamma+\hat{a}_2^{\dagger} \sinh \gamma \\
            & \hat{a}_1^{\dagger}=\hat{a}_2 \sinh \gamma+\hat{a}_2^{\dagger} \cosh \gamma \\
            & \hat{a}_2=\hat{a}_1 \cosh \gamma-\hat{a}_1^{\dagger} \sinh \gamma \\
            & \hat{a}_2^{\dagger}=-\hat{a}_1 \sinh \gamma+\hat{a}_1^{\dagger} \cosh \gamma \\
            & \mid 0\rangle_{(1)}= N (\gamma) \exp \left(-\frac{1}{2} \tanh \gamma \hat{a}_2^{\dagger} \hat{a}_2^{\dagger}\right)\mid 0\rangle_{(2)} \\
            & N (\gamma)=\frac{1}{\sqrt{\cosh \gamma}} \\
            & \mid 0\rangle_{(1)}=\frac{1}{\sqrt{\cosh \gamma}} \exp \left(-\frac{1}{2} \tanh \gamma \hat{a}_2^{\dagger} \hat{a}_2^{\dagger}\right)\mid 0\rangle_{(2)} \\
            & \left| 0_{\infty} \right \rangle \sim \exp \left(-\frac{1}{2} \hat{a}^{\dagger} \hat{a}^{\dagger}\right)\mid 0 \rangle \\
            & \left| 0_{-\infty}\right\rangle \sim \exp \left(\frac{1}{2} \hat{a}^{\dagger} \hat{a}^{\dagger}\right)\mid 0\rangle \\
            & \hat{x}\mid x\rangle=\sqrt{\frac{\hbar}{2 m \omega}}\left(\hat{a}+\hat{a}^{\dagger}\right)\mid x\rangle=x\mid x\rangle \\
            & D(\alpha)=\exp \left(\alpha \hat{a}^{\dagger}-\alpha^* \hat{a}\right), \quad\mid \alpha\rangle=D(\alpha)\mid 0\rangle \\
            & \left| 0_\gamma\right\rangle=S(\gamma)\mid 0\rangle, \quad \text { with } \quad S(\gamma)=\exp \left(-\frac{\gamma}{2}\left(\hat{a}^{\dagger} \hat{a}^{\dagger}-\hat{a} \hat{a}\right)\right) \\
            & \mid \alpha, \gamma\rangle \equiv D(\alpha) S(\gamma)\mid 0\rangle
            \end{aligned}
        \end{equation*}
    $$

- Bell states

    $\begin{aligned} & \left| \Phi_0\right\rangle=\mathbf{1} \otimes \mathbf{1}\left| \Phi_0\right\rangle=\frac{1}{\sqrt{2}}(\mid +\rangle\mid +\rangle+\mid -\rangle\mid -\rangle) \\ & \left| \Phi_1\right\rangle=\mathbf{1} \otimes \sigma_1\left| \Phi_0\right\rangle=\frac{1}{\sqrt{2}}(\mid +\rangle\mid -\rangle+\mid -\rangle\mid +\rangle) \\ & \left| \Phi_2\right\rangle=\mathbf{1} \otimes \sigma_2\left| \Phi_0\right\rangle=\frac{i}{\sqrt{2}}(\mid +\rangle\mid -\rangle-\mid -\rangle\mid +\rangle) \\ & \left| \Phi_3\right\rangle=\mathbf{1} \otimes \sigma_3\left| \Phi_0\right\rangle=\frac{1}{\sqrt{2}}(\mid +\rangle\mid +\rangle-\mid -\rangle\mid -\rangle)\end{aligned}$

- Spins

    $\begin{aligned} {\left[\hat{S}_x, \hat{S}_y\right] } & =i \hbar \hat{S}_z \\ {\left[\hat{S}_y, \hat{S}_z\right] } & =i \hbar \hat{S}_x \\ {\left[\hat{S}_z, \hat{S}_x\right] } & =i \hbar \hat{S}_y\end{aligned}$

    $\hat{S}_x=\frac{\hbar}{2}\left(\begin{array}{ll}0 & 1 \\ 1 & 0\end{array}\right), \quad \hat{S}_y=\frac{\hbar}{2}\left(\begin{array}{cc}0 & -i \\ i & 0\end{array}\right), \quad \hat{S}_z=\frac{\hbar}{2}\left(\begin{array}{cc}1 & 0 \\ 0 & -1\end{array}\right)$

    $\sigma_1=\left(\begin{array}{ll}0 & 1 \\ 1 & 0\end{array}\right), \quad \sigma_2=\left(\begin{array}{cc}0 & -i \\ i & 0\end{array}\right), \quad \sigma_3=\left(\begin{array}{cc}1 & 0 \\ 0 & -1\end{array}\right)$

    $\begin{aligned} & \mid z:+\rangle=\mid 1\rangle \longleftrightarrow\left(\begin{array}{l}1 \\ 0\end{array}\right) \\ & \mid z:-\rangle=\mid 2\rangle \longleftrightarrow\left(\begin{array}{l}0 \\ 1\end{array}\right)\end{aligned}$

    $\langle z ;-\mid z ;+\rangle=0, \quad\langle z ;+\mid z ;+\rangle=1$

    $\langle z ;+\mid z ;-\rangle=0, \quad\langle z ;-\mid z ;-\rangle=1$

    $\begin{aligned} & \mid \alpha\rangle=\alpha_1\mid 1\rangle+\alpha_2\mid 2\rangle \longleftrightarrow\left(\begin{array}{l}\alpha_1 \\ \alpha_2\end{array}\right) \\ & \mid \beta\rangle=\beta_1\mid 1\rangle+\beta_2\mid 2\rangle \longleftrightarrow\left(\begin{array}{l}\beta_1 \\ \beta_2\end{array}\right)\end{aligned}$

    $\begin{aligned} & \mid x ;+\rangle=\frac{1}{\sqrt{2}}\mid z ;+\rangle+\frac{1}{\sqrt{2}}\mid z ;-\rangle \longleftrightarrow \frac{1}{\sqrt{2}}\left(\begin{array}{c}1 \\ 1\end{array}\right), \\ & \mid x ;-\rangle=\frac{1}{\sqrt{2}}\mid z ;+\rangle-\frac{1}{\sqrt{2}}\mid z ;-\rangle \longleftrightarrow \frac{1}{\sqrt{2}}\left(\begin{array}{c}1 \\ -1\end{array}\right),\end{aligned}$

    $\begin{aligned} & \mid z ;+\rangle=\frac{1}{\sqrt{2}}\mid x ;+\rangle+\frac{1}{\sqrt{2}}\mid x ;-\rangle \\ & \mid z ;-\rangle=\frac{1}{\sqrt{2}}\mid x ;+\rangle-\frac{1}{\sqrt{2}}\mid x ;-\rangle\end{aligned}$

    $\begin{aligned} & \mid y ;+\rangle=\frac{1}{\sqrt{2}}\mid z ;+\rangle+\frac{i}{\sqrt{2}}\mid z ;-\rangle \longleftrightarrow \frac{1}{\sqrt{2}}\left(\begin{array}{c}1 \\ i\end{array}\right), \\ & \mid y ;-\rangle=\frac{1}{\sqrt{2}}\mid z ;+\rangle-\frac{i}{\sqrt{2}}\mid z ;-\rangle \longleftrightarrow \frac{1}{\sqrt{2}}\left(\begin{array}{c}1 \\ -i\end{array}\right) .\end{aligned}$

    $\left(\sigma_1\right)^2=\left(\sigma_2\right)^2=\left(\sigma_3\right)^2=\mathbf{1}$

    $\operatorname{tr}\left(\sigma_i\right)=0, \quad i=1,2,3$

    $(\mathbf{a} \cdot \boldsymbol{\sigma})(\mathbf{b} \cdot \boldsymbol{\sigma})=(\mathbf{a} \cdot \mathbf{b}) \mathbf{1}+i(\mathbf{a} \times \mathbf{b}) \cdot \boldsymbol{\sigma}$

    $\begin{aligned} & \mid \mathbf{n} ;+\rangle=\cos \frac{\theta}{2}\mid +\rangle+\sin \frac{\theta}{2} e^{i \phi}\mid -\rangle \\ & \mid \mathbf{n} ;-\rangle=-\sin \frac{\theta}{2} e^{-i \phi}\mid +\rangle+\cos \frac{\theta}{2}\mid -\rangle\end{aligned}$

    