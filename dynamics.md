### Hamiltonian dynamics

###### [*] Lagrangian, Hamiltonian, Hamilton's equations

​	<span style='color:DodgerBlue'> $L=T-V, \quad \dot{p}_j=\frac{\rm d}{{\rm d}t}(\frac{\partial L}{\partial \dot{q_j}})=\frac{\partial L}{\partial q_j},$ </span>

​	<span style='color:DodgerBlue'> $H=p_j \dot{q}_j-L, \quad \dot{q}_j=\frac{\partial H}{\partial p_j}, \quad \dot{p}_j=-\frac{\partial H}{\partial q_j}$. </span>			

###### [*] constants of motion from cyclic coordinates

​	<span style='color:DodgerBlue'> If $L$ does not explicitly depend on $q_j$, then $p_j$ is a constant of motion.</span>

###### [  ] actions and angles

​	<span style='color:DodgerBlue'> Actions: for time-independent Hamiltonian, $n$ independent constants of motion $I_k$ whose Poisson brackets with one another vanish. </span>

​	<span style='color:DodgerBlue'> Angles: the conjugate coordinates $\Theta_k$, with frequency $\omega_k=\dot{\Theta_k}=\partial H/\partial I_k$. </span>

​	<span style='color:DodgerBlue'> In 1-dim: $I(E)=\frac{1}{2\pi}\oint p(q,E){\rm d}q.$ </span>

###### [  ] canonical transformations

​	<span style='color:DodgerBlue'> Transforms that preserve Hamilton's equations. **TODO:** add math? </span>

###### [*] adiabatic invariance

​	<span style='color:DodgerBlue'>  If the Hamiltonian only slowly changes with $\omega_k T \gg 1$, the corresponding $I_k$ will be almost constant, with d$I_k\propto\exp(-\omega_k T).$</span>

​	<span style='color:DodgerBlue'> For keplerian motion in the mid plane$,\quad I_{\phi}=m\sqrt{GMa(1-e^2)},\quad I_r=m\sqrt{GMa}(1-\sqrt{1-e^2})$. </span>

​	<span style='color:DodgerBlue'> $I_{\phi}$, and therefore $Ma(1-e^2)$, are exactly constant, as long as the mass loss is spherically symmetric. $I_r$, and therefore $e$ and $Ma$, are adiabatic invariants.</span>

###### [  ] symplectic integrators

​	<span style='color:DodgerBlue'>  Based on canonical transforms so that the Hamiltonian is conserved.  </span>



### Potential theory

###### [*] Newton's Theorem (for spherically-symmetric mass distributions)

​	<span style='color:DodgerBlue'> A spherical shell exerts no gravitational forces on its interior. </span>

​	<span style='color:DodgerBlue'> The gravitational forces exerted by a spherical body on its exterior are the same as if the entire mass of the body were concentrated at its center. </span>

###### [*] Virial Theorem

​	<span style='color:DodgerBlue'> $2\left<K\right>+\left<W\right>=0$ </span>

###### [*] Poisson's equation (differential & integral forms)

​	<span style='color:DodgerBlue'> $\nabla^2\Phi=4\pi G\rho,\quad \Phi=-\int\frac{G\,\rho\,{\rm d}^3r'}{|r-r'|}$ </span>

###### [  ] Solving for potentials with spherical harmonics

​	<span style='color:DodgerBlue'>  Expand both sides of Poisson's equation with spherical harmonics. **TODO:** add math? </span>

###### [  ] Potentials of razor-thin sheets & disks

​	<span style='color:DodgerBlue'> Razor-thin: $\rho(x,y,z)=\Sigma(x,y)\delta(z)$, then do Fourier transform. **TODO:** add math? </span>



### Two-body motion

###### [  ] Runge-Lenz vector

​	<span style='color:DodgerBlue'> $A=p\times L-m\,k\,\hat{r},\quad e=-\hat{r}+\frac{p\times L}{mk}$ </span>

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/5/57/Laplace_Runge_Lenz_vector.svg/2880px-Laplace_Runge_Lenz_vector.svg.png" style="zoom: 16%;" />

###### [*] keplerian orbital elements (in 3D)

​	<span style='color:DodgerBlue'> Inclination $I$,  longitude of the ascending node $\Omega$,  argument of pericenter $\omega$. </span>

<img src="https://i.imgur.com/Z0XGiWy.png" alt="image-20220426021557346" style="zoom:50%;" />

###### [  ] true, mean, & eccentric anomalies

​	<span style='color:DodgerBlue'> True anomaly $f$,  eccentric anamoly $E$,  mean anomoly $l$,  nearest pericenter / periapsis,  farthest apocenter / apoapsis, Sun perihelion / aphelion, Earth perigee / apogee.</span>

​	<span style='color:DodgerBlue'> $r=a(1-e\cos E),\quad E-e\sin E=n(t-t_p),\quad n=2\pi/P,\quad l=n(t-t_p)$.</span>

<img src="https://i.imgur.com/OMZeKKY.png" alt="image-20220426015425221" style="zoom: 50%;" />

###### [*] expressions for orbital energy, angular momentum, period/mean motion, & distance from focus (r) in terms of $a$, $e$, & true anomaly

​	<span style='color:DodgerBlue'> $H=-\frac{GMm}{2a},\quad L=m\sqrt{GMa(1-e^2)},\quad P=2\pi\sqrt{\frac{a}{GM}},\quad r=a(1-e\cos E).$ </span>

​	<span style='color:DodgerBlue'> $\tan\left(\frac{f}{2}\right)=\sqrt{\frac{1+e}{1-e}}\tan\left(\frac{E}{2}\right).$ </span>

###### [+] Delaunay variables

​	<span style='color:DodgerBlue'> $l=n(t-t_p),\quad g=\omega,\quad h=\Omega$</span>

​	<span style='color:DodgerBlue'> $L=m\sqrt{ka},\quad G=m\sqrt{ka(1-e^2)},\quad H=m\sqrt{ka(1-e^2)}\cos I$</span>

###### [  ] perturbations causing apsidal precession (relativistic, tidal, etc.)

​	<span style='color:DodgerBlue'> $H_{\rm GR}=-\frac{3GMmR_g}{r^2}\propto r^{-2},\quad R_g=\frac{GM}{c^2}$ </span>

​	<span style='color:DodgerBlue'> $H_{\rm tidal}=-\frac{G_N}{2r^6}(k_{2,A}M_B^2R_A^5+k_{2,B}M_A^2R_B^5) \propto r^{-6}$ </span>



### Planar restricted 3-body problem

###### [*] Lagrange points

​	<span style='color:DodgerBlue'> L1, L2 and L3 unstable,  L4 and L5 stable iff $\mu(1-\mu)<1/27$,  $\mu=M_2/M$.</span>

<img src="https://upload.wikimedia.org/wikipedia/commons/thumb/e/ee/Lagrange_points2.svg/1280px-Lagrange_points2.svg.png" alt="img" style="zoom:33%;" />

###### [*] Hill sphere / Roche lobe

​	<span style='color:DodgerBlue'> The region around some astronomical body where it dominates the gravitational attraction,  $r_H=a(\mu/3)^{1/3}$.</span>

###### [  ] Jacobi constant

​	<span style='color:DodgerBlue'> Motion in a potential that is constant in a frame rotating at $\Omega$ conserves the Jacobi constant $E-\Omega\cdot L$.</span>



### Secular theory for near-keplerian systems

###### [  ] secular hamiltonians

​	<span style='color:DodgerBlue'> Average the Hamiltonian for a long period of time.</span>

###### [  ] angular-momentum deficit

​	<span style='color:DodgerBlue'> A measure of the phase space available to secular systems$,\quad{\rm AMD}=\sum_k (L_k-H_k)$.</span>

​	<span style='color:DodgerBlue'>${\rm AMD}=0$ means all orbits are circular and coplanar, nothing happens.</span>

​	<span style='color:DodgerBlue'>${\rm AMD}>0$ means angular momentum transfer between the planets is possible.</span>

###### [*] Kozai-Lidov mechanism

​	<span style='color:DodgerBlue'> For a two planet system, with the outer planet much more massive so that its orbit can be considered as unperturbed.</span>

​	<span style='color:DodgerBlue'> For the leading quadrupole term of perturbing Hamiltonian, $L$, $H$ and $H'_{\rm sec}$ are conserved. So $a$ and $\sqrt{1-e_1^2}\cos I$ are conserved, i.e. it can trade eccentricity with inclination. However, $G$ is not conserved.</span>



### Resonance and near-resonance

###### [+] disturbing function

​	<span style='color:DodgerBlue'> Minus the potential of $j$ due to $k,\quad \mathcal{R}_{jk}=\dfrac{Gm_k}{|r_j-r_k|}-Gm_k\dfrac{r_j \cdot r_k}{r_k^3}$</span>

###### [*] mean-motion resonance

​	<span style='color:DodgerBlue'> Two or more planetary periods whose ratios are rational numbers.</span>

###### [  ] slow angle, pendulum model, libration & circulation

​	<span style='color:DodgerBlue'> Do a Taylar followed by Fourier expansion of the system, usually only one term of interaction Hamiltonian dominates.</span>

​	<span style='color:DodgerBlue'> $H=H_1(J_1)+H_2(J_2)-\epsilon \cos(j_1\Theta_1+j_2\Theta_2),\quad \Psi_s=j_1\Theta_1+j_2\Theta_2,\quad H_s\approx \frac{\mu}{2}(I_s-I_{s,0})^2-\epsilon\cos\Psi_s.$</span>

​	<span style='color:DodgerBlue'> For a pendulum, libration (in resonance, locked in resonance) means it does not reach the highest point, while circulation (near resonance) means it does.</span>

###### [  ] capture into resonance (the general idea)

​	<span style='color:DodgerBlue'> The separatrix (boundary of libration and circulation) moves such that the libration phase space becomes larger, i.e. more states are captured into resonance.</span>

###### [+] first observed exoplanet system

​	<span style='color:DodgerBlue'> PSR 1257, the pulsar arrvial time oscillates with a periodic 1ms pattern of 66 and 98 days, due to the projected semimajor axis of the pulsar.</span>

###### [  ] transit-timing variations

​	<span style='color:DodgerBlue'> The planets perturb one another’s times of transit.</span>



### Chaos

###### [*] integrable/quasi-periodic vs. chaotic motion

​	<span style='color:DodgerBlue'>A Hamiltonian system in $n$ degrees of freedom is said to be integrable or regular if there exist at least $n$ independent constants of the motion such that the Possion brackets between them all vanish. Unlike the discussion regarding actions, here the Hamiltonian does not need to be time independent. </span>

​	<span style='color:DodgerBlue'>Quasi-periodic motion: the frequencies of different angles are all incommensurate.</span>

​	<span style='color:DodgerBlue'>Chaotic: non-integrable. May appear when resonance regions overlap.</span>

###### [  ] surface of section

​	<span style='color:DodgerBlue'>To record two of the phase-space variables at those times when a third variable passes through zero, useful for two degrees of freedom.</span>

###### [  ] KAM theorem (the statement, not the proof!)

​	<span style='color:DodgerBlue'>For an integrable $H_0$, the perturbed $H=H_0+\epsilon H_1$ is still integrable in a fraction of $(1-\sqrt{\epsilon})$ of the phase space. The chaotic orbits are called the Arnol'd web.</span>



### Tidal effects

###### [  ] Love number

​	<span style='color:DodgerBlue'> For sphrical harmonic degress $\ell=2$, $k_2$ is the ratio of the potential associated with the quadrupolar distortion of A by B, to the quadrupolar potential of B, at the unperturbed surface of A. Similar for $\ell>2$.</span>

​	<span style='color:DodgerBlue'> $\delta \Phi_{AB}(R_A,\theta)=k_2 \delta\Phi_B(R_A,\theta).$ </span>

###### [  ] Tidal Q

​	<span style='color:DodgerBlue'> $Q=2\pi \times \dfrac{\rm peak\ elastic\ energy\ stored}{\rm energy\ dissipated\ per\ cycle}.$ </span>



### The Milky Way & Solar neighborhood

###### [  ] coordinate systems: equatorial vs. galactic

​	<span style='color:DodgerBlue'> Galactic longitude $l, \quad$galactic latitude $b$. </span>

<img src="https://i.imgur.com/tsHiWz4.png" alt="image-20220426090814131" style="zoom:45%;" />

###### [*] major components: disk, bulge, stellar halo, dark halo

![halo2.jpg](https://astronomy.swin.edu.au/cms/cpg15x/albums/userpics/halo2.jpg)

###### [*] vital statistics: stellar mass, total mass, $R_0$, $V_0$

​	<span style='color:DodgerBlue'> $M_{\rm stellar}\approx 5\times 10^{10} M_{\odot},\quad M_{\rm total}\approx 10^{12} M_{\odot},\quad R_0=8\,{\rm kpc},\quad V_0=220\,{\rm km/s}.$ </span>

###### [  ] Schwarzschild distribution

​	<span style='color:DodgerBlue'> A solution to the collisionless Boltzmann equation in the epicycle approximation. </span>

###### [  ] Oort constants

​	<span style='color:DodgerBlue'> $A(R)=-\dfrac{1}{2}R\dfrac{{\rm d}\Omega}{{\rm d}R},\quad B(R)=-\dfrac{1}{2R}\dfrac{{\rm d}(R^2\Omega)}{{\rm d}R},\quad \Omega=A-B.$ </span>

###### [  ] stellar streams

​	<span style='color:DodgerBlue'> A stellar stream is an association of stars orbiting a galaxy that was once a globular cluster or dwarf galaxy that has now been torn apart and stretched out along its orbit by tidal forces. </span>



### Galactic (large-$N$) dynamics: generalities

###### [*] distribution function, collisionless Boltzmann equation

​	<span style='color:DodgerBlue'> $\frac{\partial f}{\partial t}+\dot{q}\cdot \frac{\partial f}{\partial q}+\dot{p}\cdot \frac{\partial f}{\partial p}=0.$ </span>

###### [  ] Jeans Theorem, isolating integrals

​	<span style='color:DodgerBlue'> Isolating integrals $I_k$ satisfy $[I_k,H]=0$.</span>

​	<span style='color:DodgerBlue'> Jeans theorem: any steady-state solution of the collisionless Boltzmann equation depends on the phase-space coordinates only through integrals of motion in the given potential, and any function of the integrals yields a steady-state solution of the collisionless Boltzmann equation.</span>

###### [  ] Jeans Equations

​	<span style='color:DodgerBlue'> Moments of CBE. **TODO:** add math?</span>

###### [*] Jeans Instability

​	<span style='color:DodgerBlue'> $t_{\rm sound}=R/c_s,\quad t_{\rm ff}=1/(G\rho)^{1/2},\quad t_{\rm ff}<t_{\rm sound} \to \lambda_J=c_s/(G\rho)^{1/2}.$ </span>

​	<span style='color:DodgerBlue'> Perturbations with scales larger than $\lambda_J$ is unstable.</span>



### Disk dynamics

###### [*] epicyclic theory (first-order)

​	<span style='color:DodgerBlue'> For an axis-symmetric Hamiltonian$:\quad H=\dfrac{p^2_R+p^2_z}{2}+\dfrac{L_z^2}{2R^2}+\Phi(R,z),$</span>

​	<span style='color:DodgerBlue'> Taylar expand the potential$:\quad U-U_c=\dfrac{1}{2}[\kappa^2 (R-R_c)^2 + \nu_z^2 z^2],\quad \Omega=L_z/R_c,$</span>

​	<span style='color:DodgerBlue'> The equations of motion become$:\quad \delta\ddot{R}+\kappa^2 \delta R=0,\quad R_c\delta\dot{\phi}+2\Omega\delta R=0,\quad \delta\ddot{z}+\nu_z^2\delta z=0,$</span>

​	<span style='color:DodgerBlue'> Epicyclic frequency $\kappa$, vertical frequency $\nu_z$. $R$ and $z$ are uncoupled harmonic oscillators, while $R$ and $\phi$ are coupled (actually closed ellipse).</span>

​	<span style='color:DodgerBlue'> Box orbits do not have time-averaged angular momenta, ring orbits do.</span>

###### [*] Toomre (Q) criterion

​	<span style='color:DodgerBlue'> $Q_{\rm gaseous}=\dfrac{\kappa c_s}{\pi G \Sigma_0},\quad Q_{\rm collisionless}=\dfrac{\kappa\sigma_R}{3.36G\Sigma_0}$ </span>

###### [  ] density waves, WKBJ (Lin-Shu) dispersion relation, swing amplification

​	<span style='color:DodgerBlue'> Density waves: perturbations to $\Sigma$ and $V$ that preserve the symmetry plane of the disk, as opposed to bending waves that wrap it. </span>

​	<span style='color:DodgerBlue'> Dispersion relation (gasous)$:\quad\omega^2=\kappa^2-2\pi G \Sigma_0 |k|+c_s^2k^2$ </span>

<img src="https://i.imgur.com/gMloxFd.png" alt="image-20220502202524388" style="zoom:50%;" />

​	<span style='color:DodgerBlue'> Spiral waves go from left to right, i.e. short leading -> long leading -> long trailing -> short trailing. </span>

​	<span style='color:DodgerBlue'> Swing amplification: spiral waves can be substantially amplified as they pass from leading to trailing. </span>



### Collisional stellar dynamics

###### [*] two-body relaxation, relaxation time

​	<span style='color:DodgerBlue'> Relaxation via two-body scattering$,\quad t_{\rm dyn}=\sqrt{\dfrac{R^3_{\rm vir}}{GM_{\rm tot}}},\quad t_{\rm rel}\sim \mathcal{O}(\dfrac{N}{\ln N})\,t_{\rm dyn}.$ </span>

###### [*] dynamical friction

​	<span style='color:DodgerBlue'>  First moment of scattering rate:  dynamical friction,  when $m\gg m_f$,  $D[v]\sim -\rho\,m\,v$,  independent of $m_f$,  so it applies to friction of a satellite galaxy against the DM halo. </span>

​	<span style='color:DodgerBlue'>  Second moment of scattering rate: tend to increase the kinetic energy . </span>

​	<span style='color:DodgerBlue'> The Fokker-Planck Equation describes changes to the DF of test stars due to frequent weak collisions . </span>

###### [  ] gravothermal evolution, core collapse, post collapse

​	<span style='color:DodgerBlue'>  Self-gravitating stellar systems can never reach thermal equilibrium:  (1) high energy tail will escape,  (2) exactly Maxwellian DF means $\infty$ total mass. </span>

​	<span style='color:DodgerBlue'>  Self-gravitating stellar systems have negative specific heat, so they will lose heat, become hotter and contract. </span>

​	<span style='color:DodgerBlue'>  The formation of a hard (tightly bound) binary releases energy to heat the single-star DF, stopping the contraction of the core. </span>

###### [  ] star clusters around black holes: tidal disruption, loss cone

​	<span style='color:DodgerBlue'>  Plunging orbits:  $L<4GM_{\rm BH}/c$. </span>

​	<span style='color:DodgerBlue'> Tidal distruption:  $GM_{\rm BH}R_*/r_p^3 \gtrsim GM_*/R_*^2,\quad r_p \lesssim r_T = R_*(M_{\rm BH} / M_*)^{1/3}.$ </span>

<img src="https://i.imgur.com/yHV9qWe.png" alt="image-20220502230927862" style="zoom:45%;" />


