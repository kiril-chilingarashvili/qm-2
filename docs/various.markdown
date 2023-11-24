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

    $$\begin{aligned} & \mid \Phi_0\rangle=\mathbf{1} \otimes \mathbf{1}\mid \Phi_0\rangle=\frac{1}{\sqrt{2}}(\mid +\rangle\mid +\rangle+\mid -\rangle\mid -\rangle) \\ & \mid \Phi_1\rangle=\mathbf{1} \otimes \sigma_1\mid \Phi_0\rangle=\frac{1}{\sqrt{2}}(\mid +\rangle\mid -\rangle+\mid -\rangle\mid +\rangle) \\ & \mid \Phi_2\rangle=\mathbf{1} \otimes \sigma_2\mid \Phi_0\rangle=\frac{i}{\sqrt{2}}(\mid +\rangle\mid -\rangle-\mid -\rangle\mid +\rangle) \\ & \mid \Phi_3\rangle=\mathbf{1} \otimes \sigma_3\mid \Phi_0\rangle=\frac{1}{\sqrt{2}}(\mid +\rangle\mid +\rangle-\mid -\rangle\mid -\rangle)\end{aligned}$$

- Spins

    $$
        \begin{aligned} {\left[\hat{S}_x, \hat{S}_y\right] } =i \hbar \hat  {S}_z \\ {\left[\hat{S}_y, \hat{S}_z\right] } =i \hbar \hat{S}_x \\   {\left[\hat{S}_z, \hat{S}_x\right] } =i \hbar \hat{S}_y\end{aligned}
    $$

    $$ \begin{equation*}
            \begin{aligned} \hat{S}_x=\frac{\hbar}{2}\left(\begin{array}{ll}0 & 1 \\ 1 & 0\end{array}\right), \quad \hat{S}_y=\frac{\hbar}{2}\left(\begin{array}{cc}0 & -i \\ i & 0\end{array}\right), \quad \hat{S}_z=\frac{\hbar}{2}\left(\begin{array}{cc}1 & 0 \\ 0 & -1\end{array}\right) \end{aligned}
        \end{equation*}
    $$

    $$
        \begin{equation*}
        \sigma_1=\left(\begin{array}{ll}0 & 1 \\ 1 & 0\end{array}\right), \quad \sigma_2=\left(\begin{array}{cc}0 & -i \\ i & 0\end{array}\right), \quad \sigma_3=\left(\begin{array}{cc}1 & 0 \\ 0 & -1\end{array}\right)
        \end{equation*}
    $$

    $$\begin{aligned} & \mid z:+\rangle=\mid 1\rangle \longleftrightarrow\left(\begin{array}{l}1 \\ 0\end{array}\right) \\ & \mid z:-\rangle=\mid 2\rangle \longleftrightarrow\left(\begin{array}{l}0 \\ 1\end{array}\right)\end{aligned}$$

    $$\langle z ;-\mid z ;+\rangle=0, \quad\langle z ;+\mid z ;+\rangle=1$$

    $$\langle z ;+\mid z ;-\rangle=0, \quad\langle z ;-\mid z ;-\rangle=1$$

    $$\begin{aligned} & \mid \alpha\rangle=\alpha_1\mid 1\rangle+\alpha_2\mid 2\rangle \longleftrightarrow\left(\begin{array}{l}\alpha_1 \\ \alpha_2\end{array}\right) \\ & \mid \beta\rangle=\beta_1\mid 1\rangle+\beta_2\mid 2\rangle \longleftrightarrow\left(\begin{array}{l}\beta_1 \\ \beta_2\end{array}\right)\end{aligned}$$

    $$\begin{aligned} & \mid x ;+\rangle=\frac{1}{\sqrt{2}}\mid z ;+\rangle+\frac{1}{\sqrt{2}}\mid z ;-\rangle \longleftrightarrow \frac{1}{\sqrt{2}}\left(\begin{array}{c}1 \\ 1\end{array}\right), \\ & \mid x ;-\rangle=\frac{1}{\sqrt{2}}\mid z ;+\rangle-\frac{1}{\sqrt{2}}\mid z ;-\rangle \longleftrightarrow \frac{1}{\sqrt{2}}\left(\begin{array}{c}1 \\ -1\end{array}\right),\end{aligned}$$

    $$\begin{aligned} & \mid z ;+\rangle=\frac{1}{\sqrt{2}}\mid x ;+\rangle+\frac{1}{\sqrt{2}}\mid x ;-\rangle \\ & \mid z ;-\rangle=\frac{1}{\sqrt{2}}\mid x ;+\rangle-\frac{1}{\sqrt{2}}\mid x ;-\rangle\end{aligned}$$

    $$\begin{aligned} & \mid y ;+\rangle=\frac{1}{\sqrt{2}}\mid z ;+\rangle+\frac{i}{\sqrt{2}}\mid z ;-\rangle \longleftrightarrow \frac{1}{\sqrt{2}}\left(\begin{array}{c}1 \\ i\end{array}\right), \\ & \mid y ;-\rangle=\frac{1}{\sqrt{2}}\mid z ;+\rangle-\frac{i}{\sqrt{2}}\mid z ;-\rangle \longleftrightarrow \frac{1}{\sqrt{2}}\left(\begin{array}{c}1 \\ -i\end{array}\right) .\end{aligned}$$

    $$\left(\sigma_1\right)^2=\left(\sigma_2\right)^2=\left(\sigma_3\right)^2=\mathbf{1}$$

    $$\operatorname{tr}\left(\sigma_i\right)=0, \quad i=1,2,3$$

    $$(\mathbf{a} \cdot \boldsymbol{\sigma})(\mathbf{b} \cdot \boldsymbol{\sigma})=(\mathbf{a} \cdot \mathbf{b}) \mathbf{1}+i(\mathbf{a} \times \mathbf{b}) \cdot \boldsymbol{\sigma}$$

    $$\begin{aligned} & \mid \mathbf{n} ;+\rangle=\cos \frac{\theta}{2}\mid +\rangle+\sin \frac{\theta}{2} e^{i \phi}\mid -\rangle \\ & \mid \mathbf{n} ;-\rangle=-\sin \frac{\theta}{2} e^{-i \phi}\mid +\rangle+\cos \frac{\theta}{2}\mid -\rangle\end{aligned}$$

- Swap operator

    $$F=\frac{1}{2}\left(1 \otimes 1+\sum_{i=1}^3 \sigma_i \otimes \sigma_i\right)$$
<<<<<<< HEAD
=======

- Angular Momentum Algebra

    $$
    \vec{L}=\vec{r} \times \vec{p} .
    $$


    $$
    \begin{aligned}
    & L_x=y p_z-z p_y, \\
    & L_y=z p_x-x p_z \\
    & L_z=x p_y-y p_x
    \end{aligned}
    $$

    $$\begin{aligned} & \vec{r} \rightarrow(\hat{x}, \hat{y}, \hat{z}), \\ & \vec{p} \rightarrow\left(\hat{p}_x, \hat{p}_y, \hat{p}_z\right), \\ & \vec{L} \rightarrow\left(\hat{L}_x, \hat{L}_y, \hat{L}_z\right) .\end{aligned}$$

    $$\begin{aligned} \mathbf{r} & \equiv \hat{x}_1 \vec{e}_1+\hat{x}_2 \vec{e}_2+\hat{x}_3 \vec{e}_3 \\ \mathbf{p} & \equiv \hat{p}_1 \vec{e}_1+\hat{p}_2 \vec{e}_2+\hat{p}_3 \vec{e}_3 \\ \mathbf{L} & \equiv \hat{L}_1 \vec{e}_1+\hat{L}_2 \vec{e}_2+\hat{L}_3 \vec{e}_3\end{aligned}$$

    $$\begin{aligned} & \mathbf{a} \equiv a_1 \vec{e}_1+a_2 \vec{e}_2+a_3 \vec{e}_3 \\ & \mathbf{b} \equiv b_1 \vec{e}_1+b_2 \vec{e}_2+b_3 \vec{e}_3\end{aligned}$$

    $$\begin{aligned} \mathbf{a} \cdot \mathbf{b} & \equiv a_i b_i \\ (\mathbf{a} \times \mathbf{b})_i & \equiv \epsilon_{i j k} a_j b_k\end{aligned}$$

    $$\mathbf{a} \cdot \mathbf{b}=a_i b_i=\left[a_i, b_i\right]+b_i a_i$$
    
    $$\mathbf{a} \cdot \mathbf{b}=\mathbf{b} \cdot \mathbf{a}+\left[a_i, b_i\right]$$

    $$\mathbf{r} \cdot \mathbf{p}=\mathbf{p} \cdot \mathbf{r}+\left[\hat{x}_i, \hat{p}_i\right]$$

    $$\mathbf{r} \cdot \mathbf{p}=\mathbf{p} \cdot \mathbf{r}+3 i \hbar$$

    $$(\mathbf{a} \times \mathbf{b})_i=-(\mathbf{b} \times \mathbf{a})_i+\epsilon_{i j k}\left[a_j, b_k\right]$$

    $$\mathbf{r} \times \mathbf{r}=0, \quad$$
     
    $$\quad \mathbf{p} \times \mathbf{p}=0$$

    $$(\mathbf{r} \times \mathbf{p})_i=-(\mathbf{p} \times \mathbf{r})_i+\epsilon_{i j k}\left[\hat{x}_j, \hat{p}_k\right]$$

    $$\mathbf{r} \times \mathbf{p}=-\mathbf{p} \times \mathbf{r}$$

    $$\begin{aligned}(\mathbf{a} \cdot \mathbf{b})^{\dagger} & =\mathbf{b}^{\dagger} \cdot \mathbf{a}^{\dagger} \\ (\mathbf{a} \times \mathbf{b})^{\dagger} & =-\mathbf{b}^{\dagger} \times \mathbf{a}^{\dagger}\end{aligned}$$

    $$\mathbf{L}=\mathbf{r} \times \mathbf{p}=-\mathbf{p} \times \mathbf{r}$$

    $$\hat{L}_i=\epsilon_{i j k} \hat{x}_j \hat{p}_k$$

    $$\mathbf{L}^{\dagger}=(\mathbf{r} \times \mathbf{p})^{\dagger}=-\mathbf{p}^{\dagger} \times \mathbf{r}^{\dagger}=-\mathbf{p} \times \mathbf{r}=\mathbf{L}$$

    $$\mathbf{L}^2=\mathbf{L} \cdot \mathbf{L}=\hat{L}_1 \hat{L}_1+\hat{L}_2 \hat{L}_2+\hat{L}_3 \hat{L}_3=\hat{L}_i \hat{L}_i$$

    $$\mathbf{r} \cdot \mathbf{L}=\hat{x}_i \hat{L}_i=\hat{x}_i \epsilon_{i j k} \hat{x}_j \hat{p}_k=\epsilon_{i j k} \hat{x}_i \hat{x}_j \hat{p}_k=0$$

    $$\mathbf{p} \cdot \mathbf{L}=\hat{p}_i \hat{L}_i=-\hat{p}_i(\mathbf{p} \times \mathbf{r})_i=-\hat{p}_i \epsilon_{i j k} \hat{p}_j \hat{x}_k=-\epsilon_{i j k} \hat{p}_i \hat{p}_j \hat{x}_k=0$$

    $$\mathbf{r} \cdot \mathbf{L}=\mathbf{p} \cdot \mathbf{L}=0$$

    $$\epsilon_{i j k} \epsilon_{i p q}=\delta_{j p} \delta_{k q}-\delta_{j q} \delta_{k p}$$

    $$\epsilon_{i j k} \epsilon_{i j q}=2 \delta_{k q}$$

    $$\begin{aligned} {[\mathbf{a} \times(\mathbf{b} \times \mathbf{c})]_k } & =\epsilon_{k j i} a_j(\mathbf{b} \times \mathbf{c})_i \\ & =\epsilon_{k j i} \epsilon_{i p q} a_j b_p c_q \\ & =-\epsilon_{i j k} \epsilon_{i p q} a_j b_p c_q \\ & =-\left(\delta_{j p} \delta_{k q}-\delta_{j q} \delta_{k p}\right) a_j b_p c_q \\ & =a_j b_k c_j-a_j b_j c_k \\ & =\left[a_j, b_k\right] c_j+b_k a_j c_j-a_j b_j c_k \\ & =\left[a_j, b_k\right] c_j+b_k(\mathbf{a} \cdot \mathbf{c})-(\mathbf{a} \cdot \mathbf{b}) c_k\end{aligned}$$

    $$\mathbf{a} \times(\mathbf{b} \times \mathbf{c})=\mathbf{b}(\mathbf{a} \cdot \mathbf{c})-(\mathbf{a} \cdot \mathbf{b}) \mathbf{c}+\left[a_j, \mathbf{b}\right] c_j$$

    $$(\vec{a} \times \vec{b})^2 \equiv(\vec{a} \times \vec{b}) \cdot(\vec{a} \times \vec{b})=\vec{a}^2 \vec{b}^2-(\vec{a} \cdot \vec{b})^2$$

    $$\mathbf{L}^2=\mathbf{r}^2 \mathbf{p}^2-(\mathbf{r} \cdot \mathbf{p})^2+i \hbar \mathbf{r} \cdot \mathbf{p}$$

    $$\mathbf{a} \cdot(\mathbf{b} \times \mathbf{c})=(\mathbf{a} \times \mathbf{b}) \cdot \mathbf{c}$$

    $$\begin{aligned} {\left[\hat{L}_i, \hat{x}_j\right] } & =i \hbar \epsilon_{i j k} \hat{x}_k \\ {\left[\hat{L}_i, \hat{p}_j\right] } & =i \hbar \epsilon_{i j k} \hat{p}_k\end{aligned}$$

    $$\begin{aligned} {\left[\hat{L}_i, \mathbf{u} \cdot \mathbf{v}\right] } & =0 \\ {\left[\hat{L}_i,(\mathbf{u} \times \mathbf{v})_j\right] } & =i \hbar \epsilon_{i j k}(\mathbf{u} \times \mathbf{v})_k .\end{aligned}$$

    $$\left[\hat{L}_i, \hat{L}_j\right]=i \hbar \epsilon_{i j k} \hat{L}_k$$

    $$\left[\hat{L}_i, \mathbf{L}^2\right]=0$$

    $$\mathbf{L} \times \mathbf{L}=i \hbar \mathbf{L} \quad \Longleftrightarrow \quad\left[\hat{L}_i, \hat{L}_j\right]=i \hbar \epsilon_{i j k} \hat{L}_k$$

    $$\left[a_i, b_j\right]=\epsilon_{i j k} c_k \rightarrow \mathbf{a} \times \mathbf{b}+\mathbf{b} \times \mathbf{a}=2 \mathbf{c}$$

- The central potential Hamiltonian

    $$\mathbf{L}^2=-\hbar^2\left(\frac{1}{\sin \theta} \frac{\partial}{\partial \theta} \sin \theta \frac{\partial}{\partial \theta}+\frac{1}{\sin ^2 \theta} \frac{\partial^2}{\partial \phi^2}\right)$$

    $$H=\frac{\mathbf{p}^2}{2 m}+V(r)=-\frac{\hbar^2}{2 m} \frac{1}{r} \frac{\partial^2}{\partial r^2} r+\frac{1}{2 m r^2} \mathbf{L}^2+V(r)$$

    Commuting observables: $H, \hat{L}_z, \mathbf{L}^2$.

- Algebraic theory of angular momentum 

    $$\begin{gathered}{\left[\hat{J}_i, \hat{J}_j\right]=i \hbar \epsilon_{i j k} \hat{J}_k} \\ {\left[\hat{J}_x, \hat{J}_y\right]=i \hbar \hat{J}_z} \\ {\left[\hat{J}_y, \hat{J}_z\right]=i \hbar \hat{J}_x} \\ {\left[\hat{J}_z, \hat{J}_x\right]=i \hbar \hat{J}_y}\end{gathered}$$

    $$\left[\hat{J}_i, \mathbf{J}^2\right]=0$$

    $$\begin{aligned} & \hat{J}_{+} \equiv \hat{J}_x+i \hat{J}_y \\ & \hat{J}_{-} \equiv \hat{J}_x-i \hat{J}_y\end{aligned}$$

    $$\left(\hat{J}_{+}\right)^{\dagger}=\hat{J}_{-}$$

    $$\begin{aligned} & \hat{J}_{+} \hat{J}_{-}=\hat{J}_x^2+\hat{J}_y^2+\hbar \hat{J}_z \\ & \hat{J}_{-} \hat{J}_{+}=\hat{J}_x^2+\hat{J}_y^2-\hbar \hat{J}_z\end{aligned}$$

    $$\left[\hat{J}_{+}, \hat{J}_{-}\right]=2 \hbar \hat{J}_z$$

    $$\mathbf{J}^2=\hat{J}_{+} \hat{J}_{-}+\hat{J}_z^2-\hbar \hat{J}_z=\hat{J}_{-} \hat{J}_{+}+\hat{J}_z^2+\hbar \hat{J}_z$$

    $$\left[\hat{J}_{ \pm}, \mathbf{J}^2\right]=0$$

    $$\left[\hat{J}_z, \hat{J}_{ \pm}\right]= \pm \hbar \hat{J}_{ \pm}$$

    $$\begin{aligned} \mathbf{J}^2|j, m\rangle & =\hbar^2 j(j+1)|j, m\rangle \\ \hat{J}_z|j, m\rangle & =\hbar m|j, m\rangle\end{aligned}$$

    $$\left\langle j^{\prime}, m^{\prime} \mid j, m\right\rangle=\delta_{j^{\prime}, j} \delta_{m^{\prime}, m}$$

    $$\hbar^2 j(j+1)=\left\langle j, m\left|\mathbf{J}^2\right| j, m\right\rangle=\sum_{i=1}^3\left\langle j, m\left|\hat{J}_i \hat{J}_i\right| j, m\right\rangle=\sum_{i=1}^3 \| \hat{J}_i|j, m\rangle \|^2 \geq 0$$

    $$\mathbf{J}^2\left(\hat{J}_{ \pm}|j, m\rangle\right)=\hat{J}_{ \pm} \mathbf{J}^2|j, m\rangle=\hbar j(j+1)\left(\hat{J}_{ \pm}|j, m\rangle\right)$$

    $$\hat{J}_{\mp} \hat{J}_{ \pm}=\mathbf{J}^2-\hat{J}_z^2 \mp \hbar \hat{J}_z$$

    $$\left|C_{ \pm}(j, m)\right|^2=\hbar^2(j(j+1)-m(m \pm 1))=\| \hat{J}_{ \pm}|j, m\rangle \|^2$$

    $$J_{ \pm}|j, m\rangle=\hbar \sqrt{j(j+1)-m(m \pm 1)}|j, m \pm 1\rangle$$

    $$2 j \in \mathbb{Z} \quad \rightarrow \quad j \in \mathbb{Z} / 2, \quad \rightarrow \quad j=0, \frac{1}{2}, 1, \frac{3}{2}, 2, \ldots$$

- Addition of Angular Momentum

    $$
    \hat{J}_i \equiv \hat{J}_i^{(1)} \otimes \mathbf{1}+\mathbf{1} \otimes \hat{J}_i^{(2)} \text { satisfies }\left[\hat{J}_i, \hat{J}_j\right]=i \hbar \epsilon_{i j k} \hat{J}_k \text { acting on } V_1 \otimes V_2 .
    $$
    
    $$\begin{aligned} {\left[\hat{J}_i, \hat{J}_j\right] } & =i \hbar \epsilon_{i j k} \hat{J}_k^{(1)} \otimes \mathbf{1}+i \hbar \epsilon_{i j k} \mathbf{1} \otimes \hat{J}_k^{(2)} \\ & =i \hbar \epsilon_{i j k}\left(\hat{J}_k^{(1)} \otimes \mathbf{1}+\mathbf{1} \otimes \hat{J}_k^{(2)}\right) \\ & =i \hbar \epsilon_{i j k} \hat{J}_k\end{aligned}$$

    $$\begin{aligned}|1,1\rangle & =|\uparrow \uparrow\rangle, \\ |1,0\rangle & =\frac{1}{\sqrt{2}}(|\uparrow \downarrow\rangle+|\downarrow \uparrow\rangle), \\ |1,-1\rangle & =|\downarrow \downarrow\rangle . \\ |0,0\rangle & =\frac{1}{\sqrt{2}}(|\uparrow \downarrow\rangle-|\downarrow \uparrow\rangle) .\end{aligned}$$

- Feynman-Hellman lemma

    $$\frac{d E(\lambda)}{d \lambda}=\left\langle\psi(\lambda)\left|\frac{d H(\lambda)}{d \lambda}\right| \psi(\lambda)\right\rangle$$

    $$\Delta E=\langle\psi(0)|\Delta H| \psi(0)\rangle$$

- General aspects of addition of angular momentum

    $$j_1 \otimes j_2=\left(j_1+j_2\right) \oplus\left(j_1+j_2-1\right) \oplus \ldots \oplus\left|j_1-j_2\right|$$

- Hydrogen atom and hidden symmetry

    $$E_n=-\frac{e^2}{2 a_0} \frac{1}{n^2}, \quad n=1,2, \ldots$$

    $$\ell=0,1, \ldots, n-1$$

    $$\mathcal{H}_n=(\ell=n-1) \oplus(\ell=n-2) \oplus \cdots \oplus(\ell=0)$$

    $$H=\frac{\mathbf{p}^{\mathbf{2}}}{2 m}-\frac{e^2}{r}$$

    $$[H, \mathbf{L}]=0, \quad \mathbf{L} \times \mathbf{L}=i \hbar \mathbf{L}$$

    This Runge-Lenz vector $R$ is defined to be:
    $$
    \mathbf{R} \equiv \frac{1}{2 m e^2}(\mathbf{p} \times \mathbf{L}-\mathbf{L} \times \mathbf{p})-\frac{\mathbf{r}}{r}
    $$

    $$[H, \mathbf{R}]=0$$

    $$\mathbf{p} \times \mathbf{L}=-\mathbf{L} \times \mathbf{p}+2 i \hbar \mathbf{p}$$

    $$\mathbf{R}=\frac{1}{m e^2}(\mathbf{p} \times \mathbf{L}-i \hbar \mathbf{p})-\frac{\mathbf{r}}{r}=\frac{1}{m e^2}(-\mathbf{L} \times \mathbf{p}+i \hbar \mathbf{p})-\frac{\mathbf{r}}{r}$$

    $$\mathbf{R}^2=1+\frac{2 H}{m e^4}\left(\mathbf{L}^2+\hbar^2\right)$$

    $$\mathbf{r} \cdot \mathbf{L}=0, \quad \mathbf{p} \cdot \mathbf{L}=0$$

    $$\mathbf{R} \cdot \mathbf{L}=\frac{1}{m e^2}(\mathbf{p} \times \mathbf{L}) \cdot \mathbf{L}$$

    $$(\mathbf{p} \times \mathbf{L}) \cdot \mathbf{L}=\epsilon_{i j k} p_j L_k L_i=p_j \epsilon_{j k i} L_k L_i=p_j(\mathbf{L} \times \mathbf{L})_j=\mathbf{p} \cdot(i \hbar \mathbf{L})=0$$

    $$\mathbf{R} \cdot \mathbf{L}=0$$

    $$\left[L_i, \hat{v}_j\right]=i \hbar \epsilon_{i j k} \hat{v}_k$$

    $$\begin{aligned}(\mathbf{L} \times \mathbf{v}+\mathbf{v} \times \mathbf{L})_i & =\epsilon_{i j k}\left(L_j \hat{v}_k+\hat{v}_j L_k\right) \\ & =\epsilon_{i j k}\left(L_j \hat{v}_k-\hat{v}_k L_j\right) \\ & =\epsilon_{i j k}\left[L_j, \hat{v}_k\right] \\ & =\epsilon_{i j k} i \hbar \epsilon_{j k l} \hat{v}_l \\ & =\epsilon_{i j k} \epsilon_{l j k} i \hbar \hat{v}_l \\ & =2 \delta_{i l} i \hbar \hat{v}_l=2 i \hbar \hat{v}_i\end{aligned}$$

    $$\mathbf{L} \times \mathbf{v}+\mathbf{v} \times \mathbf{L}=2 i \hbar \mathbf{v}$$

    $$\mathbf{L} \times \mathbf{R}+\mathbf{R} \times \mathbf{L}=2 i \hbar \mathbf{R}$$

    $$\left[L_i, R_j\right]=i \hbar \epsilon_{i j k} R_k$$

    $$\left[S_1, H\right]=\left[S_2, H\right]=0$$

    $$\begin{gathered}{\left[\left[S_1, S_2\right], H\right]+\left[\left[H, S_1\right], S_2\right]+\left[\left[S_2, H\right], S_1\right]=0} \\ {\left[\left[S_1, S_2\right], H\right]=\left[\left[S_1, H\right], S_2\right]-\left[\left[S_2, H\right], S_1\right]}\end{gathered}$$

    $$\left[\left[S_1, S_2\right], H\right]=0$$

    $$\mathbf{R} \times \mathbf{R}=(\cdots) \text{"conserved vector"} $$

    $$\mathbf{R} \times \mathbf{R}=i \hbar\left(-\frac{2 H}{m e^4}\right) \mathbf{L}$$

    $$H=E_\nu=-\frac{m e^4}{2 \hbar^2} \frac{1}{\nu^2}, \quad \nu \in \mathbb{R}$$

    $$-\frac{2 H}{m e^4}=\frac{1}{\hbar^2 \nu^2}$$

    $$\begin{aligned} \mathbf{R} \times \mathbf{R} & =i \hbar \frac{1}{\hbar^2 \nu^2} \mathbf{L} \\ \mathbf{R}^2 & =1-\frac{1}{\hbar^2 \nu^2}\left(\mathbf{L}^2+\hbar^2\right)\end{aligned}$$

    $$\begin{aligned}(\hbar \nu \mathbf{R}) \times(\hbar \nu \mathbf{R}) & =i \hbar \mathbf{L}, \\ \mathbf{L}^2+\hbar^2 \nu^2 \mathbf{R}^2 & =\hbar^2\left(\nu^2-1\right) .\end{aligned}$$

    $$\begin{aligned} & \mathbf{J}_1 \equiv \frac{1}{2}(\mathbf{L}+\hbar \nu \mathbf{R}) \\ & \mathbf{J}_2 \equiv \frac{1}{2}(\mathbf{L}-\hbar \nu \mathbf{R})\end{aligned}$$

    $$\begin{aligned} \mathbf{L} & =\mathbf{J}_1+\mathbf{J}_2 \\ \hbar \nu \mathbf{R} & =\mathbf{J}_1-\mathbf{J}_2\end{aligned}$$

    $$\begin{aligned} {\left[J_{1 i}, J_{2 j}\right] } & =\frac{1}{4}\left[L_i+\hbar \nu R_i, L_j-\hbar \nu R_j\right] \\ & =\frac{1}{4}\left(i \hbar \epsilon_{i j k} L_k-\hbar \nu\left[L_i, R_j\right]-\hbar \nu\left[L_j, R_i\right]-i \hbar \epsilon_{i j k} L_k\right)=0\end{aligned}$$

    $$\begin{aligned} \mathbf{J}_{1 / 2} \times \mathbf{J}_{1 / 2} & =\frac{1}{4}(\mathbf{L} \pm \hbar \nu \mathbf{R}) \times(\mathbf{L} \pm \hbar \nu \mathbf{R}) \\ & =\frac{1}{4}(i \hbar \mathbf{L}+i \hbar \mathbf{L} \pm(\mathbf{L} \times \hbar \nu \mathbf{R}+\hbar \nu \mathbf{R} \times \mathbf{L})) \\ & =\frac{1}{4}(2 i \hbar \mathbf{L} \pm 2 i \hbar \hbar \nu \mathbf{R}) \\ & =i \hbar \frac{1}{2}(\mathbf{L} \pm \hbar \nu \mathbf{R})=\mathbf{J}_{1 / 2}\end{aligned}$$

    $$\begin{aligned} \mathbf{J}_1 \times \mathbf{J}_1 & =i \hbar \mathbf{J}_1, \\ \mathbf{J}_2 \times \mathbf{J}_2 & =i \hbar \mathbf{J}_2, \\ {\left[\mathbf{J}_1, \mathbf{J}_2\right] } & =0\end{aligned}$$

    $$\left(\mathbf{J}_1+\mathbf{J}_2\right)\left(\mathbf{J}_1-\mathbf{J}_2\right)=0 \quad \rightarrow \quad \mathbf{J}_1^2=\mathbf{J}_2^2$$

    $$\mathbf{J}_1^2=\frac{1}{4}\left(\mathbf{L}^2+\hbar^2 \nu^2 \mathbf{R}^2\right)=\frac{1}{4} \hbar^2\left(\nu^2-1\right)$$

    $$\mathbf{J}_1^2=\mathbf{J}_2^2=\frac{1}{4} \hbar^2\left(\nu^2-1\right)=\hbar^2 j(j+1)$$

    $$\nu^2=1+4 j(j+1)=4 j^2+4 j+1=(2 j+1)^2 \quad \rightarrow \quad \nu=2 j+1$$

    $$\begin{aligned} j & =0, \frac{1}{2}, 1, \frac{3}{2}, \ldots \\ n \equiv \nu=2 j+1 & =1,2,3,4, \ldots\end{aligned}$$

    $$\mathcal{H}_n=j \otimes j \quad$$ 
    
    with basis states 
    
    $$\quad\left|j_1=j ; m_1\right\rangle \otimes\left|j_2=j ; m_2\right\rangle, \quad-j \leq m_1, m_2 \leq j$$

    $$j \otimes j=2 j \oplus 2 j-1 \oplus \ldots \oplus 0$$

    $$(\ell=2 j) \oplus(\ell=2 j-1) \oplus \ldots \oplus 0$$

    $$\mathcal{H}_n=(\ell=n-1) \oplus(\ell=n-2) \oplus \ldots \oplus(\ell=0)$$

    $$\ell=1:\left\{\begin{array}{l}|1,1\rangle=|\uparrow \uparrow\rangle, \\ |1,0\rangle=\frac{1}{\sqrt{2}}(|\uparrow \downarrow\rangle+|\downarrow \uparrow\rangle), \quad \ell=0: \quad|0,0\rangle=\frac{1}{\sqrt{2}}(|\uparrow \downarrow\rangle-|\downarrow \uparrow\rangle) . \\ |1,-1\rangle=|\downarrow \downarrow\rangle\end{array}\right.$$


>>>>>>> c61f3ae427d7f5899bdc297c820dc36a6bac14b7
