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
  <video width="15%" autoplay muted playsinline loop>
    <source src="/images/animation_only_cone_id=1_v4_full_cripped_Nov.mp4" type="video/mp4">
  </video>
  <video width="83%" autoplay muted playsinline loop>
    <source src="/images/animation_only_maps_id=1_v4_full_cripped_Nov.mp4" type="video/mp4">
  </video>
</div>

Animation shows the contribution of the kSZ effect to the CMB temperature maps. 

Most recently, in [Hotinli et al.](https://arxiv.org/pdf/2506.21657), we developed the [kszx](https://kszx.readthedocs.io/en/latest/) framework, enabling the kSZ effect to be combined with galaxy data to measure long-wavelength cosmological modes and small-scale electron distributions at the highest precision to date. This work establishes the method, introduces rigorous covariance-simulation techniques for accurate uncertainty quantification, detects the signal at high significance (at signal-to-noise ~12), an obtains the strongest kSZ-based bounds on primordial non-Gaussianity. 

<br/><img src='/images/Pgv_150_and_90_v6 (2).pdf' width="500">

Galaxy–velocity cross-power spectra \(P_{gv}(k)\) using the 90 GHz (top) and 150 GHz (bottom) CMB maps from ACT DR5 and the DESI Legacy Survey (black points with error bars).  
**Solid red lines** show model predictions with \(b_g = 2.2\), \(\fnl = 0\), and \(b_v = \{0.47, 0.39\}\) for \(\{90,150\}\) GHz. This model is a good fit (\(\chi^2 = 8.5\) or \(8.2\) with \(N_{\rm dof} = 8\)) over the range of scales used in this paper (\(k \lesssim 0.018\ \mathrm{Mpc}^{-1}\), delimited by the grey band). The **dashed** and **dotted** lines correspond to model predictions with \(f_{\rm NL} = \pm 100\). The signal-to-noise ratio (SNR) is \(\{8.4, 10.3\}\) at \(\{90,150\}\) GHz. The **purple cross markers** show the estimated \(P_{gv}(k)\) obtained when omitting the \(\hat v_r\) mean-subtraction step in Eq.~\eqref{eq:hvr_ms}. The large difference between the black points and purple crosses indicates significant foreground contamination at 90 GHz, which is mitigated by the mean-subtraction step. From [Hotinli et al.](https://arxiv.org/pdf/2506.21657).


Over the years I have helped define its scientific vision by identifying its most powerful early-Universe and late-time targets. 

These include smoking-gun tests of primordial non-Gaussianity and isocurvature:

<br/><img src='/images/fig3.png' width="500">
Forecasted error ellipses on \(f_{NL}\) and (\tau_{NL})\ at 68 and 95 percent confidence intervals, after marginalizing over bias parameters. Left: results when only galaxy survey data is considered. Right: results when velocity reconstruction data is added to the analysis. From [Neha Anil Kumar et al.](https://arxiv.org/pdf/2205.03423)

<br/><img src='/images/fig2.png' width="500">

<br/><img src='/images/fig1.png' width="500">







In the recent years I have also authored research papers which demonstrated that the kinetic Sunyaev Zel'dovich (kSZ) tomography (or radial-velocity reconstruction) (Cayuso et al 2020) will provide the most competitive constraints on primordial non-Gaussianity (Kumar et al 2022) and isocurvature (Hotinli et al 2019, Kumar et al 2022), smoking-gun signatures of inflationary scenarios or unknown components that may have been active during the early epoch of our Universe. In the former study, we have also demonstrated an opportunity to unambiguously probe unknown components in the early Universe by comparing different forms of higher-order statistics of the density fluctuations. These efforts are complementary to the core science goals of upcoming CMB experiments, such as measuring the effective number of relativistic species. My research has shown, for example, that the Figure of Merit (FoM) characterising the statistical information content of the joint analysis of large-scale galaxy clustering and velocity fields (latter reconstructed from measurements of the kSZ effect) with Simons Observatory and DESI data by 2026 can be greater by a factor of over an order-of-magnitude compared to considering DESI galaxy clustering in isolation. After the first year data release of LSST, this difference could reach over two orders of magnitude compared to considering LSST in isolation.


<br/><img src='/images/selim-hotinli-imperial-research-fellowship_1669244802034_0.jpg' width="500">

### Probing Helium reionization with CMB x LSS

In addition to probing large-scale deviations from LCDM, the reconstruction program can contribute significantly to the characterisation of both hydrogen (Hotinli and Johnson 2020) and helium (Hotinli et al 2022) reionization (image below).

<br/><img src='/images/selim-hotinli-imperial-research-fellowship-1_1669245023933_0.jpg' width="500">

Characterising helium reionization has great significance for understanding galaxy formation, quasar activity and cosmology, and may open a new window on big bang nucleosynthesis.  Since photons emitted by the first stars (sourcing the reionization of hydrogen) are not energetic enough to fully ionize helium, helium reionization occurs only after the emergence of a substantial number of quasars. As a result, the history of helium reionization strongly depends on the properties of quasars, such as their luminosity function, accretion mechanisms and other astrophysics, clustering, variability, lifetimes, as well as the general growth and evolution of super-massive black holes. Since essentially all of the helium in the Universe is ultimately doubly ionized, the total change in the ionization fraction is also a measure of the primordial helium abundance—a sensitive probe of big bang nucleosynthesis. Furthermore, probing helium reionization can also improve our understanding of relativistic species through improving the primordial helium fraction measurement and breaking the degeneracy between the number of relativistic species and primordial helium fraction. As the primordial helium abundance depends on the weak interaction rates as well as the neutron lifetime, improving its measurement can also allow further valuable insights into our cosmological history. Observational challenges posed by helium emission line measurements make additional probes extremely valuable.

One of the main research programs I lead focuses on characterisation of both hydrogen (Hotinli and Johnson 2020) and helium reionization (Hotinli et al 2022)  from joint analyses of LSS and CMB data. In particular, characterising helium reionization has great significance for understanding galaxy formation, quasar activity and cosmology.  Since photons emitted by the first stars (sourcing the reionization of hydrogen) are not energetic enough to fully ionize helium, helium reionization occurs only after the emergence of a substantial number of quasars.

As a result, the history of helium reionization strongly depends on the properties of quasars, such as their luminosity function, accretion mechanisms and other astrophysics, clustering, variability, lifetimes, as well as the general growth and evolution of super-massive black holes. Observational challenges posed by helium emission line measurements make additional probes extremely valuable. I anticipate a multitude of studies will follow my work, capitalising on the statistical power of cross-correlations between CMB and different high-redshift LSS probes. These results are extremely promising and will likely re-ignite the interest from the community for helium reionization. My efforts currently focus on advancing scientific programs involving characterisation of helium reionization with joint analyses of CMB and LSS including contributing to building up the science cases of the line-intensity signals, which will be a promising direction within this program, and transform this area into an active, evolving field of research. 

<br/><img src='/images/selim-hotinli-imperial-research-fellowship-2_1669245332786_0.jpg' width="500">

On this image: We now know that the hydrogen and helium fully ionizes in the Universe after the formation of first luminous objects. During this process, the ionization fraction (the fraction of free electrons) goes from zero to, say 1, for all the electrons in the hydrogen atom being ionized (kicked away of their proton). This happens soon after the first stars form. You may notice that this line does not end at one, however, which is because helium also ionizes, loosing its first electron around the same time as hydrogen. However the second electron in helium requires much more energy to ionize which only happens after sufficient numbers of much more luminous objects such as quasars, due to active galactic nuclei formation. As a result, the history of helium reionization strongly depends on the properties of quasars, such as their luminosity, accretion mechanisms and other very much unknown astrophysics, clustering, variability, lifetimes, as well as the general growth and evolution of super-massive black holes. In a recent work, I have shown for the first time that the joint analysis of the CMB and upcoming high-redshift galaxy surveys can indeed probe this epoch. (See arXiv:2207.07660)

### Other CMB signatures

In the last years I have also made valuable contributions to identifying various novel CMB signatures including the moving lens effect (Hotinli et al 2018, Hotinli et al 2020, Hotinli et al 2021), the pSZ (Lee et al 2022) and kpSZ (Hotinli et al 2022) effects. My efforts on these lines also explored the full reach of the prospects to probing fundamental physics with these signatures. The moving-lens effect is due to cosmological structure moving transverse to our line of sight and results of purely gravitational effects. As a result, it can be used to measure quantities which cannot be accessed directly with the kSZ effect alone, such as the growth rate of density fluctuations, which is useful for studying dark energy, modified gravity, and the effects of neutrino mass (Hotinli et al 2018). The polarized Sunyaev Zel'dovich (pSZ) effect is a linear blackbody polarization sourced by photons that scatter off free electrons in the large-scale structure, proportional to the remote CMB temperature quadrupole observed in the electrons’ rest frame. The measurement of pSZ effect allows reconstructing the linear polarization of the CMB as a function of redshift on the light cone. This allows probing the tensor to scalar ratio as well as the cosmic birefringence angle (Lee et al 2022) that is sourced if the physics behind dark energy and/or dark matter violates the parity symmetry assumed in the standard cosmological paradigm. Relativistic corrections to the remote quadrupole field also give rise to a non-blackbody polarization anisotropy proportional to the square of the transverse peculiar velocity field; this is the kinetic polarized Sunyaev Zel’dovich (kpSZ) effect. The kpSZ effect is also a probe of cosmic birefringence and primordial non-Gaussianity (Hotinli et al 2022).

### Improving CMB measurements

The effects of gravitational lensing and scattering on the CMB photons is both a help and hindrance to our understanding of the history and contents of the Universe. Both lensing and scattering effects manifest themselves as a distortion of the primary CMB anisotropies and also functions as an obstacle to analyses which rely on a pristine view of the last scattering surface. Simons Observatory and the succeeding experiments will map the CMB sky with unprecedented precision where these effects will be limiting factors to cosmological inference. My current and future efforts also focus on mitigating the effects of lensing and scattering on the primary CMB with the goal of improving the forthcoming cosmological parameter constraints. 

To this end, I co-developed a code for robust treatments of CMB ‘delensing’ on the curved sky, demonstrating the impact that removing the lensing effect from the CMB map will have with future surveys. Together with the forecasting framework I co-developed, these softwares are now becoming parts of the main analysis pipelines of the upcoming CMB experiments. I have also authored research papers on assessing the prospects to delens the CMB temperature and polarisation maps as well as to remove the kSZ effect using external galaxy templates, or ‘de-kSZing' (Foreman, Hotinli et al 2020).

The delensed CMB spectra have sharper acoustic peaks and more prominent damping tails, allowing for improved inferences of cosmological parameters that impact those features. Delensing reduces the B-mode power, aiding the search for primordial gravitational waves and allowing for lower variance reconstruction of lensing and other sources of secondary CMB anisotropies. Lensing-induced power spectrum covariances are reduced by delensing, simplifying analyses and improving constraints on primordial non-Gaussianities. Biases that result from incorrectly modelling nonlinear and baryonic feedback effects on the lensing power spectrum are mitigated by delensing. All of these benefits are possible without any changes to experimental or survey design. 

The situation with the kSZ effect is analogous to that of gravitational lensing. In a recent work, we investigated the prospects for external “de-kSZing'' of CMB temperature maps, whereby an external galaxy survey is used to construct a template for the kSZ effect, which is then subtracted from the observed maps. The kSZ effect can significantly bias lensing reconstruction, affecting our ability to constrain neutrino mass, dark energy, and dark matter. Furthermore, kSZ fluctuations at small scales add noise to measurements of the Silk-damped regime of the primary CMB, which can be used to probe Neff, the primordial helium abundance, and the spectrum of primordial scalar perturbations. The kSZ effect also acts as noise for measurements of other CMB secondaries, such as the moving-lens effect.
