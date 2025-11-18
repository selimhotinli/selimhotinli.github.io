---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
use_math: true
---

{% include base_path %}



At the heart of my research is a program that combines large-scale structure (LSS) and cosmic microwave background (CMB) measurements, using the CMB as a cosmic backlight to study the scattering and lensing effects of dark-matter halos, filaments, galaxies, and diffuse ionized gas. This multi-tracer frontier has been evolving quickly, and my work over the past decade has played a role in shaping its trajectory.

<br/><img src='/images/Secondary_Signals.jpg' width="500">

Image by: Merrill Sherman/Quanta Magazine.

I lead multiple collaborations and survey-analysis pipelines, but my central effort has been the development of a major science program built around measurements of the kinetic Sunyaev–Zel’dovich (kSZ) effect, a doppler effect due to CMB photons scattering off on energetic electrons in the large-scale structure that have some non-zero radial velocity. This program is poised to transform CMB and LSS studies by unlocking unprecedented information across both cosmological and astrophysical scales. It will drive new discoveries and influence the design and use of future surveys, whose scientific impact will increasingly hinge on their contributions to multi-tracer analyses.

### Kinetic Sunyaev Zel'dovich tomography

Though subtle in appearance, the kSZ is a unique and powerful probe of cosmic structure: nearly all small-scale CMB blackbody fluctuations arise from the kSZ signal, surpassing even gravitational lensing at arcminute scales. 

The kSZ effect directly measures the large-scale velocity field, providing a unique probe of structure formation and matter distribution. When jointly analyzed with other tracers, it delivers effectively arbitrarily precise, cosmic-variance–free constraints on subtle departures in clustering, making it a leading method for uncovering primordial non-Gaussianity and related early-Universe signals.

<div style="display:flex; gap:20px;">
  <video width="20%" autoplay muted playsinline loop>
    <source src="/images/animation_only_cone_id=1_v4_full_cripped_Nov.mp4" type="video/mp4">
  </video>
  <video width="78%" autoplay muted playsinline loop>
    <source src="/images/animation_only_maps_id=1_v4_full_cripped_Nov.mp4" type="video/mp4">
  </video>
</div>

Animation shows the contribution of the kSZ effect to the CMB temperature maps. 

Most recently, in [Hotinli et al.](https://arxiv.org/abs/2506.21657), we developed the [kszx](https://kszx.readthedocs.io/en/latest/) framework, enabling the kSZ effect to be combined with galaxy data to measure long-wavelength cosmological modes and small-scale electron distributions at the highest precision to date. This work establishes the method, introduces rigorous covariance-simulation techniques for accurate uncertainty quantification, detects the signal at high significance (at signal-to-noise ~12), an obtains the strongest kSZ-based bounds on primordial non-Gaussianity. 


<div style="display: flex; gap: 10px; align-items: flex-start;">
  <img src="/images/page_1.jpg" width="58%; height: auto;">
  <img src="/images/page_1_fnl.jpg" width="38%; height: auto;">
</div>

From [Hotinli et al. (2506.21657)](https://arxiv.org/abs/2506.21657). Galaxy–velocity cross-power spectra using the 90 GHz (top) and 150 GHz (bottom) CMB maps from ACT DR5 and the DESI Legacy Survey (black points with error bars). **Solid red lines** show model predictions in the absense of primordial non-Gaussianity. This model is a good fit over the range of scales used in this paper, delimited by the grey band. The **dashed** and **dotted** lines correspond to model predictions with primordial non-Gaussianity amplitude +/-100. The signal-to-noise ratio (SNR) is (8.4, 10.3) at (90, 150) GHz. The **purple cross markers** show the estimated galaxy-velocity cross-correlation obtained when omitting the mean-subtraction step described in the paper. The large difference between the black points and purple crosses indicates significant foreground contamination at 90 GHz, which is mitigated by the mean-subtraction step. 




In the past year, in [Jordan Krywonos et al. (2408.05264)](https://arxiv.org/abs/2408.05264), we also used reconstruction based on data from Planck and unWISE surveys to rule out non-linear Gpc-scale voids, provide the tightest constraint on the intrinsic dipole (< 14 km/s at 68% confidence), rule out matter-radiation isocurvature as an explanation of discrepancies between the measured CMB and galaxy number count dipoles, and constrain the amplitude of local-type primordial non-Gaussianity (−220 < fNL < 136 at 68% confidence) and compensated isocurvature (−147 < ACIP < 281 at 68% confidence). This representative set of constraints on beyond-ΛCDM scenarios demonstrates the breadth of fundamental science possible with measurements of secondary CMB anisotropies.




The kSZ effect also offers powerful astrophysical insight into the ***distribution of ionized gas*** in cosmic structures. It constrains electron-gas profiles, probes the physics of ***baryonic feedback***, and provides an independent test of hydrodynamical simulations. Recent kSZ measurements suggest that a ***large fraction of baryons lie at greater radii*** than predicted and that feedback varies with halo mass and epoch. Because feedback strongly shapes both astrophysics and cosmological inference, characterizing it is essential. My near-term research will test feedback models against high-resolution simulations and data, building on pipelines that already perform these analyses. Advancing these tools is a major focus of my work.

Over the years I have helped define its scientific vision by identifying its most powerful early-Universe and late-time targets. 

These include developing unique ***unbiased*** probes of ***electron gas distribution***:

<br/><img src='/images/page_1_gal.jpg' width="1200">

From [Neha Anil Kumar et al. (2509.18249)](https://arxiv.org/abs/2509.18249). Forecasted errors on the reconstruction of electron auto-correlation in three redshift bins of equal comoving width, ordered from lowest to highest z from left to right. The model predictions for the electron gas signal computed assuming the Battaglia ‘AGN’ model. All error bars assume CMB data from an SO-like telescope and DESI and LSST-like galaxy surveys.



..and smoking-gun tests of ***primordial non-Gaussianity and isocurvature***:

<br/><img src='/images/fig3.png' width="600">

From [Neha Anil Kumar et al. (2205.03423)](https://arxiv.org/abs/2205.03423). Forecasted error ellipses on primordial non-Gaussianity signals at 68 and 95 percent confidence intervals, after marginalizing over bias parameters. Left: results when only galaxy survey data is considered. Right: results when velocity reconstruction data is added to the analysis.

<br/><img src='/images/fig2.png' width="600">

From [Neha Anil Kumar et al. (2208.02829)](https://arxiv.org/abs/2208.02829). Forecasted error on the primordial isocurvature amplitude after marginalizing over bias parameters as a function of largest scales (Left) and galaxy density (Right) considered in the analysis. Baseline I (II) corresponds to an LSST (DESI)-like galaxy survey. 

<br/><img src='/images/fig1.png' width="1200">

From [Hotinli et al. (1908.08953)](https://arxiv.org/abs/1908.08953). The impact of changing various survey parameters relevant for, or related to, cosmological experiments.



The kSZ tomography will also play a role in probing many fundemental signatures including ***neutrino masses*** [Avery J. Tishue et al. 2502.05260](https://arxiv.org/abs/2502.05260), ***dark-energy microphysics*** [Julius Aldoff et al. (2511.05653)](https://arxiv.org/abs/2511.05653),  ***parity violation*** [Eleonora Vanzan et al. (2311.18121)](https://arxiv.org/abs/2311.18121), eternal inflation [P. Zhang and M. C. Johnson (1501.00511)](https://arxiv.org/abs/1501.00511) and ***modified gravity*** [Z. Pan, M. C. Johnson (1906.04208)](https://arxiv.org/abs/1906.04208).




Among other things, the kSZ tomography and CMB secondaries program can also contribute significantly to the characterisation of both hydrogen and helium reionization.

<br/><img src='/images/selim-hotinli-imperial-research-fellowship-1_1669245023933_0.jpg' width="550">

Characterizing helium reionization is crucial for understanding galaxy formation, quasar evolution, and cosmology, and may even open a new window on big bang nucleosynthesis. Because photons from the first stars cannot fully ionize helium, helium reionization occurs only after a significant population of quasars emerges; its history therefore encodes quasar luminosities, accretion physics, clustering, variability, lifetimes, and the growth of supermassive black holes. Since nearly all helium becomes doubly ionized, the total change in ionization fraction also traces the primordial helium abundance—a sensitive probe of big bang nucleosynthesis. Improved constraints on helium reionization can tighten measurements of the primordial helium fraction, break degeneracies with the effective number of relativistic species, and shed light on weak interaction rates and the neutron lifetime. Given the observational challenges of helium emission-line measurements, complementary probes are especially valuable.

In the recent years I have lead a program that demonstrated that joint analyses of CMB and large-scale structure data can detect signatures of helium reionization.

<div style="display: flex; gap: 10px; align-items: flex-start;">
  <img src="/images/helium1.png" width="52%; height: auto;">
  <img src="/images/helium2.png" width="41%; height: auto;">
</div>

From [Hotinli et al. (2207.07660)](https://arxiv.org/abs/2207.07660). ***Left***: Fractional change in the electron fraction during helium reionization of the three models we consider here. Here, we include forecasts for the combination of VRO and CMB-S4, and MegaMapper and CMB-HD. ***Right***: The sensitivities on the helium reionization parameters from two survey combinations: VRO and CMB-S4 shown with blue contours, and MegaMapper and CMB-HD, shown with orange contours. 

<br/><img src='/images/helium3.png' width="1200">

From [Caliskan et al. (2312.00118)](https://arxiv.org/abs/2312.00118). Fractional errors of helium (right panel) and hydrogen (left panel) reionization parameters from patchy optical depth reconstruction. Technique uses a four-point statistic combining CMB temperature, polarization, and galaxy clustering.

<br/><img src='/images/helium4.png' width="1200">

From [Anil Kumar et al. (2506.11188)](https://arxiv.org/abs/2506.11188). Fractional errors of helium (right panel) and hydrogen (left panel) reionization parameters from projected kSZ. Technique uses a four-point statistic combining CMB temperature and galaxy clustering.


Measurements using these teqniue will provide an independent observational probe of this key cosmic epoch and opening new possibilities to explore its connection to galaxy formation, quasar evolution, and the growth of cosmic structures. 



### Other CMB signatures

In the last years I have also made valuable contributions to identifying various novel CMB signatures including the moving lens effect (Hotinli et al 2018, Hotinli et al 2020, Hotinli et al 2021), the pSZ (Lee et al 2022) and kpSZ (Hotinli et al 2022) effects. My efforts on these lines also explored the full reach of the prospects to probing fundamental physics with these signatures. The moving-lens effect is due to cosmological structure moving transverse to our line of sight and results of purely gravitational effects. As a result, it can be used to measure quantities which cannot be accessed directly with the kSZ effect alone, such as the growth rate of density fluctuations, which is useful for studying dark energy, modified gravity, and the effects of neutrino mass (Hotinli et al 2018). The polarized Sunyaev Zel'dovich (pSZ) effect is a linear blackbody polarization sourced by photons that scatter off free electrons in the large-scale structure, proportional to the remote CMB temperature quadrupole observed in the electrons’ rest frame. The measurement of pSZ effect allows reconstructing the linear polarization of the CMB as a function of redshift on the light cone. This allows probing the tensor to scalar ratio as well as the cosmic birefringence angle (Lee et al 2022) that is sourced if the physics behind dark energy and/or dark matter violates the parity symmetry assumed in the standard cosmological paradigm. Relativistic corrections to the remote quadrupole field also give rise to a non-blackbody polarization anisotropy proportional to the square of the transverse peculiar velocity field; this is the kinetic polarized Sunyaev Zel’dovich (kpSZ) effect. The kpSZ effect is also a probe of cosmic birefringence and primordial non-Gaussianity (Hotinli et al 2022).

### Improving CMB measurements

The effects of gravitational lensing and scattering on the CMB photons is both a help and hindrance to our understanding of the history and contents of the Universe. Both lensing and scattering effects manifest themselves as a distortion of the primary CMB anisotropies and also functions as an obstacle to analyses which rely on a pristine view of the last scattering surface. Simons Observatory and the succeeding experiments will map the CMB sky with unprecedented precision where these effects will be limiting factors to cosmological inference. My current and future efforts also focus on mitigating the effects of lensing and scattering on the primary CMB with the goal of improving the forthcoming cosmological parameter constraints. 

To this end, I co-developed a code for robust treatments of CMB ‘delensing’ on the curved sky, demonstrating the impact that removing the lensing effect from the CMB map will have with future surveys. Together with the forecasting framework I co-developed, these softwares are now becoming parts of the main analysis pipelines of the upcoming CMB experiments. I have also authored research papers on assessing the prospects to delens the CMB temperature and polarisation maps as well as to remove the kSZ effect using external galaxy templates, or ‘de-kSZing' (Foreman, Hotinli et al 2020).

The delensed CMB spectra have sharper acoustic peaks and more prominent damping tails, allowing for improved inferences of cosmological parameters that impact those features. Delensing reduces the B-mode power, aiding the search for primordial gravitational waves and allowing for lower variance reconstruction of lensing and other sources of secondary CMB anisotropies. Lensing-induced power spectrum covariances are reduced by delensing, simplifying analyses and improving constraints on primordial non-Gaussianities. Biases that result from incorrectly modelling nonlinear and baryonic feedback effects on the lensing power spectrum are mitigated by delensing. All of these benefits are possible without any changes to experimental or survey design. 

The situation with the kSZ effect is analogous to that of gravitational lensing. In a recent work, we investigated the prospects for external “de-kSZing'' of CMB temperature maps, whereby an external galaxy survey is used to construct a template for the kSZ effect, which is then subtracted from the observed maps. The kSZ effect can significantly bias lensing reconstruction, affecting our ability to constrain neutrino mass, dark energy, and dark matter. Furthermore, kSZ fluctuations at small scales add noise to measurements of the Silk-damped regime of the primary CMB, which can be used to probe Neff, the primordial helium abundance, and the spectrum of primordial scalar perturbations. The kSZ effect also acts as noise for measurements of other CMB secondaries, such as the moving-lens effect.
