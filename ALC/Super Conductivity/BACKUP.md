  

\section{Electrical Resistance and Temperature Dependence}

\label{sec:metals}

  

As established in the introduction, the vanishing of electrical resistance

below a critical temperature $T_c$ is one of the defining signatures of

superconductivity. To appreciate how remarkable this is, it is worth first

understanding how resistance behaves in ordinary materials. The mechanisms

governing electrical transport differ fundamentally between metals,

semiconductors, and superconductors, and each class shows a qualitatively

distinct $R(T)$ behaviour. In this experiment, resistance as a function of

temperature is measured for superconducting samples, and the results are

interpreted in the context of the theoretical picture developed in this

section \cite{experiment}.

  
  

\subsection{Metals}

  
  

In a metal, electrical conduction is carried by a gas of free electrons

occupying states up to the Fermi energy $E_F$. In the Drude model, a

constant electric field $\mathbf{E}$ accelerates electrons between

collisions, and the resulting steady-state current density gives the

conductivity \cite{Kittel2005}

  

\begin{equation}

\sigma = \frac{ne^2\tau}{m_e}

\label{eq:drude}

\end{equation}

  

where $n$ is the free electron density, $e$ is the electron charge, $m_e$

is the electron mass, and $\tau$ is the mean time between scattering events.

The electrical resistivity follows as $\rho = 1/\sigma = m_e/ne^2\tau$.

  

Two main scattering mechanisms contribute independently to the total

resistivity \cite{Kittel2005}. The first arises from thermally excited lattice

vibrations (phonons), which become more pronounced with increasing temperature

as the amplitude of ionic oscillations grows. The second comes from static

crystal imperfections such as impurities and vacancies, which are

temperature-independent. The two contributions add according to

Matthiessen's rule

  

\begin{equation}

\rho(T) = \rho_L(T) + \rho_i

\label{eq:matthiessen}

\end{equation}

  

where $\rho_L$ is the lattice (phonon) contribution and $\rho_i$ is the

residual resistivity due to impurity scattering \cite{Kittel2005}. At

temperatures well above the Debye temperature $\Theta_D$, the phonon

concentration is proportional to $T$ and therefore $\rho_L \propto T$. As

$T \to 0$, phonon scattering freezes out and $\rho$ saturates at the

residual value $\rho_i$, which depends only on the purity and structural

quality of the sample \cite{Kittel2005}. The overall behaviour is therefore

a resistance that decreases monotonically on cooling, levelling off at a

small residual value.

  

\begin{figure}[h]

\centering

% \includegraphics[width=0.6\textwidth]{figures/metal_RT.png}

\caption{Schematic $R(T)$ dependence for a typical metal, showing

approximately linear behaviour at high temperatures and saturation

toward a residual resistance $\rho_i$ at low temperatures, as described

by Matthiessen's rule (Eq.~\ref{eq:matthiessen}). Adapted from

Kittel \cite{Kittel2005}.}

\label{fig:metal_RT}

\end{figure}

  
  

\subsection{Semiconductors}

\label{sec:semiconductors}

  
  

In a semiconductor, the electronic structure consists of a completely filled

valence band and an empty conduction band, separated by an energy gap $E_g$

of order 1\,eV \cite{Kittel2005}. At zero temperature no free charge

carriers are available and the material is effectively insulating. As

temperature increases, electrons are thermally excited across the gap,

creating mobile electrons in the conduction band and holes in the valence

band. Both species contribute to conduction.

  

For an intrinsic (undoped) semiconductor, the equilibrium carrier

concentration is found by integrating the Fermi-Dirac distribution over the

density of states in each band. The result is \cite{Kittel2005}

  

\begin{equation}

n_i = p_i = 2\left(\frac{k_BT}{2\pi\hbar^2}\right)^{3/2}

(m_e m_h)^{3/4} \exp\!\left(-\frac{E_g}{2k_BT}\right)

\label{eq:intrinsic_carrier}

\end{equation}

  

where $m_e$ and $m_h$ are the electron and hole effective masses

respectively. The electrical conductivity is

  

\begin{equation}

\sigma = e(n\mu_e + p\mu_h)

\label{eq:sc_conductivity}

\end{equation}

  

where $\mu_e$ and $\mu_h$ are the electron and hole mobilities

\cite{Kittel2005}. Since the exponential factor in Eq.~(\ref{eq:intrinsic_carrier})

dominates the temperature dependence, the conductivity increases strongly

with temperature, and the resistivity decreases, which is the opposite

behaviour to metals

  

\begin{equation}

\rho(T) \propto \exp\!\left(\frac{E_g}{2k_BT}\right)

\label{eq:sc_rho}

\end{equation}

  

This activated behaviour means that a plot of $\ln\rho$ against $1/T$

yields a straight line with slope $E_g/2k_B$, providing a direct way to

extract the band gap from resistance measurements \cite{Kittel2005}. The

Fermi level of an intrinsic semiconductor lies approximately in the middle

of the gap.

  

\begin{equation}

\mu \approx \frac{1}{2}E_g + \frac{3}{4}k_BT\ln\!\left(\frac{m_h}{m_e}\right)

\label{eq:fermi_sc}

\end{equation}

  

\begin{figure}[h]

\centering

% \includegraphics[width=0.6\textwidth]{figures/semiconductor_RT.png}

\caption{Schematic $R(T)$ dependence for an intrinsic semiconductor,

showing the exponentially decreasing resistance with increasing

temperature characteristic of thermally activated carrier generation

(Eq.~\ref{eq:sc_rho}). Adapted from Kittel \cite{Kittel2005}.}

\label{fig:sc_RT}

\end{figure}

  
  

\subsection{Superconductors and BCS Theory}

\label{sec:bcs}

  
  

Above $T_c$, a superconductor behaves as a normal metal, showing resistivity

broadly consistent with the metallic picture described in

Section~\ref{sec:metals}. Below $T_c$, however, the resistance drops

abruptly to zero rather than saturating at a residual value

\cite{Buckel2004}. This cannot be explained by reduced phonon scattering

alone, since even a perfectly pure metal retains a finite phonon contribution

at any nonzero temperature. A fundamentally different mechanism must be

at work.

  

The explanation is provided by the Bardeen-Cooper-Schrieffer (BCS) theory

(1957), which identifies a phonon-mediated attractive interaction between

electrons near the Fermi surface \cite{Tinkham1996}. The direct Coulomb

interaction between two electrons is repulsive, but an electron moving

through the lattice leaves behind a slight positive polarisation of the

surrounding ions. A second electron arriving shortly after is attracted to

this polarisation. Provided the electron energy difference is smaller than

the characteristic phonon energy $\hbar\omega_D$, the phonon-mediated

attraction can override the screened Coulomb repulsion, giving a net

attractive matrix element $-V$ \cite{Tinkham1996}. The importance of the

electron-lattice interaction was confirmed by the isotope effect, in which

$T_c \propto M^{-1/2}$ for different isotopes of the same element, directly

implicating phonons in the mechanism \cite{Tinkham1996}.

  

Cooper showed in 1956 that the Fermi sea is unstable against the formation

of a bound pair of electrons whenever any net attractive interaction exists,

regardless of how weak it is \cite{Tinkham1996}. In the lowest energy state,

the two electrons in a Cooper pair have equal and opposite momenta and

opposite spins, so the pair carries zero net momentum and zero net spin.

Being effectively bosonic, all Cooper pairs condense into the same quantum

ground state, described by a single macroscopic wave function with a

well-defined phase \cite{Buckel2004}.

  

The key consequence of this condensation is the opening of an energy gap

$\Delta$ in the quasi-particle excitation spectrum. The energy of a

quasi-particle excitation with momentum $\hbar k$ is \cite{Tinkham1996}

  

\begin{equation}

E_k = \sqrt{\xi_k^2 + \Delta^2}

\label{eq:quasiparticle}

\end{equation}

  

where $\xi_k$ is the single-particle energy measured from the Fermi level.

The gap $\Delta$ represents the minimum energy required to break a Cooper

pair; as long as $k_BT \ll \Delta$, thermal fluctuations cannot disrupt the

condensate, and resistance remains zero. The self-consistency condition

on $\Delta$ yields, in the weak-coupling limit \cite{Tinkham1996}

  

\begin{equation}

\Delta(0) = 2\hbar\omega_D \exp\!\left(-\frac{1}{N(0)V}\right)

\label{eq:gap_zero}

\end{equation}

  

where $N(0)$ is the density of states at the Fermi level per spin and $V$

is the effective pairing interaction strength. The critical temperature is

related to the Debye frequency by \cite{Tinkham1996}

  

\begin{equation}

k_B T_c = 1.13\,\hbar\omega_D\,e^{-1/N(0)V}

\label{eq:Tc_bcs}

\end{equation}

  

Comparing Eqs.~(\ref{eq:gap_zero}) and (\ref{eq:Tc_bcs}), one obtains the

fundamental BCS relation between the zero-temperature gap and the critical

temperature \cite{Tinkham1996}

  

\begin{equation}

2\Delta(0) = 3.52\,k_BT_c

\label{eq:bcs_gap_ratio}

\end{equation}

  

This ratio has been measured in many materials and typically falls in the

range $3.0\,k_BT_c$ to $4.5\,k_BT_c$, with most clustering near the BCS

value \cite{Tinkham1996}. Near $T_c$, the gap closes continuously as

  

\begin{equation}

\Delta(T) = \Delta_0 \tanh\left(1.82 \sqrt{\frac{T_c - T}{T_c}}\right)

\label{eq:gap_T}

\end{equation}

  
  

\begin{equation}

\Delta(T) \approx 1.74\,\Delta(0)\left(1 - \frac{T}{T_c}\right)^{1/2}

\end{equation}

  

which is characteristic of a mean-field second-order phase transition.

The transition at $T_c$ is therefore sharp in a clean, homogeneous sample.

In practice, real samples such as the YBa$_2$Cu$_3$O$_7$ and

Bi$_2$Sr$_2$CaCu$_2$O$_{8+x}$ samples used in this experiment exhibit a

finite transition width $\Delta T_c$, defined as the temperature range

between 10\% and 90\% of the normal-state resistance $R_N$. This broadening

is attributed to inhomogeneities in oxygen concentration and crystal

quality \cite{experiment}.

  

\begin{figure}[h]

\centering

% \includegraphics[width=0.55\textwidth]{figures/bcs_gap.png}

\caption{Temperature dependence of the BCS energy gap $\Delta(T)$,

normalised to its zero-temperature value $\Delta(0) = 1.76\,k_BT_c$.

The gap is approximately constant below $0.5\,T_c$ and closes

continuously at $T_c$ following Eq.~(\ref{eq:gap_T}). Adapted from

Tinkham \cite{Tinkham1996}, Fig.~3.2.}

\label{fig:bcs_gap}

\end{figure}

  

\begin{figure}[h]

\centering

% \includegraphics[width=0.6\textwidth]{figures/superconductor_RT.png}

\caption{Schematic $R(T)$ curve for a superconductor, showing metallic

behaviour above $T_c$ followed by a sharp transition to zero resistance.

The characteristic temperatures $T_{c,\mathrm{on}}$,

$T_{c,\mathrm{mid}}$, and $T_{c,0}$ and the transition width

$\Delta T_c$ are indicated. Adapted from \cite{experiment}.}

\label{fig:sc_Rtransition}

\end{figure}

