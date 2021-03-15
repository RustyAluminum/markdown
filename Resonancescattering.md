<script type="text/javascript" src="http://cdn.mathjax.org/mathjax/latest/MathJax.js?config=default"></script>
# Paper
## Chen_2018
### home message
##### work: 
1. Here we apply direct Monte Carlo simulation scheme via dimensionless calculation to an isothermal, ch
2. emically uniform, and spherically symmetric
medium with a radial density distribution characterized by a β-model.<br>
2. apply the modeling scheme to the O VII and O VIII emission line complex observed in the XMM-Newton RGS spectrum of the M31 bulge. <br>
3. We estimate the isotropic turbulence Mach number of the medium in
M31 as ∼0.17 for the first time<br>

##### conclusion:
1. the RS could indeed account for much of the spatial distortion of the emission, as well as the relative intensities of the lines, especially the large forbidden-toresonant-line ratio of the O VII Heα triplet.<br>
2. the RS may in general play an important role in shaping the soft X-ray spectra of diffuse hot gas in normal galaxies.<br>
3. the line-emitting gas temperature as ∼2.3×10^6 K in M31.<br>
4. the RS effect may raise the O VII G-ratio to a value substantially higher than 1 within a few $r_c$ and suppress it to below 0.5 near the boundary.<br>

##### further
1. the isothermal model is too simplistic to explain the entire RGS spectrum of the plasma(有一段没拟合成功), extending the simulations to more physical models of the plasma distribution and to larger spectral ranges will enable us to study the RS effect in more realistic and complicated cases.<br>

### introduction
##### background:
1. characteristic temperature $\gtrsim 10^6$ K, the medium can be well traced by soft X-ray emission, which is dominated by various lines from K- or L-shell transitions of heavy elements such as O, Ne, and Fe ions (e.g., O VII, OVIII, NeIX, and Fe XVII).<br>
The emission is commonly assumed to be optically thin in spectral modeling.
2. this assumption may not hold for certain resonant lines(depend on oscillation strengths, the thermal, turbulent velocity dispersion, density of the hot gas, the abundances, ionization states of the elements).<br>
3. With the existing X-ray instruments, we can detect the spatial distortion of the surface intensity distribution of the line emission due to the RS effect.<br>
4. distortion degree depends upon the optical depth(目前观测到的并且escape from outer regions of the medium都是optically thin  which are  to the line).<br>
5. The spectra of diffuse X-ray emission from diffuse hot plasma systems typically show distinct iron emission lines from K-shell and L-shell transitions.<br>
6. 本工作讨论场景仅仅：hot ISM is assumed to be isothermal, chemically uniform, and spherically symmetric.<br>
7. 本工作使用的模型: a simple model of the medium with certain symmetry and uniformity to characterize the effects of the RS.<br>
8. The key parameter that determines the effectiveness of the RS is the line-center optical depth $\tau$.<br>
9. The G-ratio is defined as the ratio of the sum of intercombination and forbidden components to the resonant component (Gabriel & Jordan 1969).<br>
10. The RGS is a slit-less spectrometer and is sensitive to photons in the 0.3–2 keV range.<br>


##### extending:
1. Zanstra effect(see, e.g., Zanstra 1949; Field 1959).
2. the RS effects 的影响因素之一： the line optical depth 
3. The RS effect in X-rays has been studied mostly in diffuse hot plasma of massive elliptical galaxies and clusters of galaxies.<br>
e.g., Sazonov et al. 2002; Xu et al. 2002; Churazov et al. 2004; Molnar et al. 2006; Werner et al. 2009; Zhuravleva et al. 2011; Ogorzalek et al. 2017; Hitomi Collaboration et al. 2018)
4. earliest theoretical work by Gilfanov et al. (1987) is based on an iteration method, 忽视 the photoelectric absorption by cool gas可能与 hot medium混淆.
5. Monte Carlo (MC) radiative transfer simulations of the RS effect on lines typical for the $\gtrsim 10^7$ K gas.
6. X-ray absorption line spectroscopy of bright background point-like sources reveals: the hot ISM in our Galaxy is optically thick(O VII Heα triplet).
7. The XMM-Newton RGS study of the bulge of M31 shows: the forbidden-to-resonant line ratio of the O VII Heα triplet is much greater than 1

##### method:
MC simulation: <br>
seed photons are generated with random directional angles and with the location probability according to the volume emissivity distribution of the hot ISM.<br>
assume the isothermal and chemically uniform medium of a spherically symmetric distribution.<br>
in terms of dimensionless frequencies and dimensionless lengths, with the characteristic τ given, is essentially independent of specific lines and the gas velocity dispersion.<br>
an upper cutoff $\Delta l_{max}/r_c=0.01$ is set for the stepsize, while $\Delta \tau(x)/\tau_c=0.001$ is used.<br>
first simulation assuming a β-model of gas with $\beta=2/3$, next simulations with the considerations described in Section 2 for a β-model of the hot plasma distribution suitable for the M31 bulge.<br>
综合考虑，$10^6$个光子数最适合进行模拟


### personal thinking + difficluties:
1. need to know:<br>
collisional ionization equilibrium(CIE)<br>
overheating (e.g., due to recent shock-heating), overcooling<br>
charge exchange(CX) between ions and neutral atoms at the interface with cool gas<br>
M31 bulge<br>
RS event判定时，能量与direction变动规则所需理论<br>
2. 数理方面: Gaussian distribution, Voigt function, gamma function<br>
3. The RS is only partially coherent in the observer’s frame<br>
4. 离子的recoil作用忽略不计（哪些工作需要考虑recoil？量级比较)<br>
5. 本工作的simulation scheme 可适用于任意thermal, chemical, and kinematic properties 的 hot ISM 的 spatial distribution. hot ISM的空间分布理论需要了解.<br>
6. APEC model<br>
7. isothermal β-model<br>
8. RS event判定所需理论<br>
9. outer region对光谱影响很小


### question:
1. R1, R2, R3先随机生成后得出等式右边的参量（r, $/miu$)？<br>
2. (15)<br>
3. （14）是随机生成的？
4. table1比值的理论，以及为什么考虑这几条线: the weighted probability distribution is given by (Hamilton 1947; Churazov et al. 2010).