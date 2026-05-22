---
layout: archive
title: "Research"
permalink: /research/
author_profile: true
use_math: true
---

{% include base_path %}

My research program is organized around two observations in productive interplay: the striking simplicity of the early Universe and the rich complexity of the astrophysical processes that followed. The cosmic microwave background — the oldest light in the Universe — travels billions of years before reaching our telescopes, and along the way it is scattered, distorted, and imprinted by every structure it encounters. I exploit the CMB as a cosmic backlight, developing methods that use these imprints to simultaneously probe fundamental physics and the astrophysical processes that shape structure formation.

<img src='/images/Secondary_Signals.jpg' class="img-small" alt="Illustration of secondary CMB signals from scattering and lensing by large-scale structure">
<p class="research-block__caption">Image: Merrill Sherman / Quanta Magazine.</p>

<div class="research-nav">
  <a href="#velocity">Velocity Reconstruction</a>
  <a href="#initial-conditions">Initial Conditions</a>
  <a href="#gas-feedback">Gas &amp; Feedback</a>
  <a href="#neutrinos-de">Neutrinos &amp; Dark Energy</a>
  <a href="#beyond-ksz">Beyond kSZ</a>
  <a href="#tools">Sharpening the Tools</a>
</div>


<div id="velocity" class="research-section" markdown="1">

## How can we turn the CMB into a map of cosmic velocities?

<p class="research-intro">As CMB photons pass through clouds of ionized gas, they receive tiny energy shifts from the bulk motion of the electrons — the kinetic Sunyaev-Zel'dovich effect. I have developed methods to invert this process: starting from the observed temperature shifts, reconstruct the three-dimensional velocity field of the Universe.</p>

The kSZ effect dominates small-scale CMB blackbody fluctuations, surpassing even gravitational lensing at arcminute scales. It directly measures the large-scale velocity field, probing structure formation and matter distribution. When combined with galaxy survey data, it attains effectively cosmic-variance-free sensitivity to departures in matter and galaxy clustering — making it a leading method for detecting primordial non-Gaussianity and related early-Universe signals.

<div class="fig-row fig-row--videos" markdown="0">
  <video autoplay muted playsinline loop>
    <source src="/images/animation_only_cone_id=1_v4_full_cripped_Nov.mp4" type="video/mp4">
  </video>
  <video autoplay muted playsinline loop>
    <source src="/images/animation_only_maps_id=1_v4_full_cripped_Nov.mp4" type="video/mp4">
  </video>
</div>
<p class="research-block__caption">Animation showing the contribution of the kSZ effect to CMB temperature maps as a function of redshift.</p>

In [Hotinli, Smith & Ferraro (2506.21657)](https://arxiv.org/abs/2506.21657), we developed the [kszx](https://kszx.readthedocs.io/en/latest/) framework, enabling the first three-dimensional kSZ velocity reconstruction using a photometric galaxy survey. Using ACT DR5 CMB maps cross-correlated with the DESI Legacy Imaging Surveys, we detected the signal at signal-to-noise ~12 and obtained the strongest kSZ-based bounds on primordial non-Gaussianity to date.

<div class="fig-row fig-row--60-40" markdown="0">
  <img src="/images/page_1.jpg" alt="Galaxy-velocity cross-power spectra from ACT and DESI at 90 and 150 GHz">
  <img src="/images/page_1_fnl.jpg" alt="Constraints on primordial non-Gaussianity from kSZ velocity reconstruction">
</div>
<p class="research-block__caption">Measured galaxy-velocity cross-spectra from ACT and DESI data compared with theoretical predictions. Agreement across two frequency channels confirms a robust kSZ detection. From <a href="https://arxiv.org/abs/2506.21657">Hotinli et al. (2506.21657)</a>.</p>

</div>


<div id="initial-conditions" class="research-section" markdown="1">

## What do cosmic velocities reveal about the origin of structure?

<p class="research-intro">The velocities of matter carry a remarkably clean record of the conditions set during the earliest moments — cleaner, in some regimes, than the density field itself. By combining kSZ velocity reconstruction with galaxy surveys, we can place powerful new constraints on primordial non-Gaussianity, isocurvature perturbations, and parity-violating signatures in the initial conditions.</p>

**Primordial non-Gaussianity.** The kSZ velocity field provides a direct handle on long-wavelength modes that modulate small-scale clustering. In [Anil Kumar et al. (2205.03423)](https://arxiv.org/abs/2205.03423), we showed that combining next-generation galaxy surveys with kSZ reconstruction improves constraints on the non-Gaussianity amplitude $f_{\rm NL}$ by an order of magnitude — and enables first constraints on the primordial trispectrum $\tau_{\rm NL}$, a probe of extra degrees of freedom during inflation.

<img src='/images/fig3.png' class="img-medium" alt="Forecasted error ellipses on primordial non-Gaussianity from kSZ tomography">
<p class="research-block__caption">Forecasted constraints on primordial non-Gaussianity with galaxy data alone (left) vs. with kSZ velocity reconstruction added (right). From <a href="https://arxiv.org/abs/2205.03423">Anil Kumar et al. (2205.03423)</a>.</p>

**Compensated isocurvature perturbations.** These are primordial fluctuations in the relative baryon and dark matter density that leave the total matter density unchanged — making them nearly invisible to the CMB alone. Current constraints allow them to be hundreds of times larger than adiabatic perturbations, a surprisingly large gap in our knowledge. In [Hotinli et al. (1908.08953)](https://arxiv.org/abs/1908.08953) and [Anil Kumar et al. (2208.02829)](https://arxiv.org/abs/2208.02829), we showed that kSZ tomography can improve these constraints by over two orders of magnitude. I have also explored complementary probes using the 21-cm signal during cosmic dawn in [Hotinli et al. (2106.11979)](https://arxiv.org/abs/2106.11979).

<div class="fig-row fig-row--half" markdown="0">
  <img src="/images/fig2.png" alt="Forecasted isocurvature amplitude constraints as a function of survey parameters">
  <img src="/images/fig1.png" alt="Impact of survey parameters on kSZ-based constraints">
</div>
<p class="research-block__caption">Left: forecasted isocurvature constraints from kSZ tomography with different survey combinations. Right: impact of survey parameters on constraining power. From <a href="https://arxiv.org/abs/2208.02829">Anil Kumar et al. (2208.02829)</a> and <a href="https://arxiv.org/abs/1908.08953">Hotinli et al. (1908.08953)</a>.</p>

**Constraints beyond LCDM.** In [Krywonos et al. (2408.05264)](https://arxiv.org/abs/2408.05264), we used velocity reconstruction from Planck and unWISE data to simultaneously: rule out nonlinear Gpc-scale voids; set the tightest constraint on the intrinsic CMB dipole (< 14 km/s, 68% CL); rule out matter-radiation isocurvature as the source of CMB–galaxy dipole discrepancies; and constrain primordial non-Gaussianity and compensated isocurvature. This demonstrates the breadth of fundamental science accessible with kSZ-based methods, even in the current noise-dominated regime.

**Parity violation.** In [Vanzan, Kamionkowski & Hotinli (2311.18121)](https://arxiv.org/abs/2311.18121), we developed the phenomenology of a primordial vector field that generates compensated isocurvature perturbations and may explain recently reported parity-odd signals in galaxy surveys — testable with upcoming kSZ measurements.

</div>


<div id="gas-feedback" class="research-section" markdown="1">

## What can scattering signatures teach us about the life cycle of cosmic gas?

<p class="research-intro">The same CMB cross-correlations that probe fundamental physics also encode detailed information about baryonic processes — how gas is heated, expelled, and redistributed by feedback from galaxies and active nuclei. These astrophysical signatures are both a science target in their own right and a critical systematic for precision cosmology.</p>

**Electron gas distribution and baryonic feedback.** The kSZ effect constrains electron-gas profiles, probes the physics of baryonic feedback, and provides independent tests of hydrodynamical simulations. Recent measurements suggest that a large fraction of baryons lie at greater radii than predicted and that feedback varies with halo mass and epoch. Because baryonic feedback can induce significant deviations in lensing and matter power spectra, characterizing it is essential for both astrophysics and cosmological inference.

In [Anil Kumar et al. (2509.18249)](https://arxiv.org/abs/2509.18249), we developed unbiased probes of the electron gas auto-correlation using kSZ tomography, with forecasts for the Simons Observatory combined with DESI and LSST-like surveys.

<img src='/images/page_1_gal.jpg' class="img-wide" alt="Forecasted electron auto-correlation reconstruction in three redshift bins">
<p class="research-block__caption">Forecasted errors on electron auto-correlation reconstruction in three redshift bins, assuming the Battaglia AGN model. From <a href="https://arxiv.org/abs/2509.18249">Anil Kumar et al. (2509.18249)</a>.</p>

<img src='/images/selim-hotinli-imperial-research-fellowship-1_1669245023933_0.jpg' class="img-small" alt="Selim Hotinli presenting research on helium reionization">

**Helium reionization.** Helium reionization is a distinct, later cosmic event driven by quasars. Its history encodes information about quasar evolution, the growth of supermassive black holes, and even the primordial helium abundance — a probe of big bang nucleosynthesis. I have led a program demonstrating that joint CMB and large-scale structure analyses can detect signatures of helium reionization, using multiple independent techniques.

<div class="fig-row fig-row--40-30" markdown="0">
  <img src="/images/helium1.png" alt="Helium reionization models showing fractional change in electron fraction">
  <img src="/images/helium2.png" alt="Forecasted sensitivities on helium reionization parameters">
</div>
<p class="research-block__caption">Left: helium reionization models. Right: forecasted sensitivities from VRO + CMB-S4 (blue) and MegaMapper + CMB-HD (orange). From <a href="https://arxiv.org/abs/2207.07660">Hotinli et al. (2207.07660)</a>.</p>

<img src='/images/helium3.png' class="img-medium" alt="Fractional errors on reionization parameters from patchy optical depth reconstruction">
<p class="research-block__caption">Fractional errors on helium and hydrogen reionization parameters from patchy optical depth reconstruction. From <a href="https://arxiv.org/abs/2312.00118">Caliskan et al. (2312.00118)</a>.</p>

<img src='/images/helium4.png' class="img-medium" alt="Fractional errors on reionization parameters from projected kSZ">
<p class="research-block__caption">Fractional errors from projected kSZ, combining CMB temperature and galaxy clustering. From <a href="https://arxiv.org/abs/2506.11188">Anil Kumar et al. (2506.11188)</a>.</p>

These measurements provide an independent observational probe of this key cosmic epoch, opening new possibilities to explore its connection to galaxy formation and the growth of cosmic structures.

</div>


<div id="neutrinos-de" class="research-section" markdown="1">

## What can kSZ tomography reveal about neutrino masses and dark energy?

<p class="research-intro">Neutrino masses and the nature of dark energy both leave signatures in how quickly structure grows over cosmic time. The velocity field reconstructed from kSZ measurements provides an independent probe of this growth rate, breaking degeneracies that limit traditional methods.</p>

**Dark energy microphysics.** In [Adolff, Hotinli & Dalal (2511.05653)](https://arxiv.org/abs/2511.05653), we showed that kSZ tomography can go beyond measuring the expansion history to probe the perturbative properties of dark energy — its sound speed and clustering behavior. Forecasts show that adding kSZ data tightens constraints on the dark energy equation of state by 15–32%, with degeneracy directions distinct from geometric probes. This is especially relevant given recent tentative hints from DESI of deviations from LCDM.

**Neutrino masses.** kSZ tomography provides complementary sensitivity to the sum of neutrino masses through its effect on the growth rate of structure. Forecasts in [Tishue et al. (2502.05260)](https://arxiv.org/abs/2502.05260) demonstrate that upcoming survey combinations will place competitive constraints.

**Modified gravity and eternal inflation.** The kSZ velocity field also probes the growth rate directly, making it a natural test of modified gravity theories (see [Pan & Johnson (1906.04208)](https://arxiv.org/abs/1906.04208)) and large-scale signatures of eternal inflation (see [Zhang & Johnson (1501.00511)](https://arxiv.org/abs/1501.00511)).

</div>


<div id="beyond-ksz" class="research-section" markdown="1">

## What other CMB signatures carry information about large-scale structure?

<p class="research-intro">The kSZ effect is one member of a broader family of CMB–large-scale-structure interactions. Each signature opens an independent window onto cosmology and astrophysics, and the methods developed in one context often unlock measurements in another.</p>

**The moving-lens effect.** The bulk transverse motion of massive structures induces a small-scale dipolar temperature pattern centered on each halo. Unlike the kSZ effect, this is a purely gravitational signature, making it a clean probe of the transverse velocity field and the growth rate of structure. I derived optimal detection filters and forecasted signal-to-noise ~20 with next-generation CMB experiments and the Rubin Observatory. [[Hotinli et al. (1710.08913)]](https://arxiv.org/abs/1710.08913) [[Hotinli, Johnson & Meyers (2006.03060)]](https://arxiv.org/abs/2006.03060) [[Read more →]](/movinglenseffect/)

**Polarized Sunyaev-Zel'dovich (pSZ) effect.** CMB photons scattering off free electrons acquire a polarization proportional to the CMB quadrupole at the scatterer's location. Measuring this allows reconstruction of CMB polarization as a function of redshift — a new probe of the tensor-to-scalar ratio and cosmic birefringence. Tentative hints of birefringence in Planck and WMAP data motivate this as an independent validation path. [[Lee, Hotinli & Kamionkowski (2207.05687)]](https://arxiv.org/abs/2207.05687)

**Kinetic polarized SZ (kpSZ) effect.** Relativistic corrections to the remote quadrupole produce a non-blackbody polarization signal proportional to the square of the transverse velocity. This is an additional probe of cosmic birefringence and primordial non-Gaussianity, detectable with upcoming CMB experiments. [[Hotinli et al. (2204.12503)]](https://arxiv.org/abs/2204.12503)

</div>


<div id="tools" class="research-section" markdown="1">

## How can we remove foreground contamination to sharpen every measurement?

<p class="research-intro">Many of the signals described above also act as contaminants for one another. I have developed techniques to subtract these contributions, improving sensitivity across multiple science targets. These methods close the loop: the same reconstructions that enable new science also clean the data for existing analyses.</p>

**Delensing.** Gravitational lensing of the CMB is both a rich signal and a source of noise for other measurements. I co-developed a code for robust delensing on the curved sky, now being integrated into analysis pipelines for upcoming CMB experiments. Delensed CMB spectra have sharper acoustic peaks and reduced B-mode power, improving constraints on primordial gravitational waves and mitigating biases from baryonic feedback modeling.

**De-kSZing.** The kSZ effect itself can bias lensing reconstruction and add noise to measurements of the Silk-damped primary CMB — affecting sensitivity to $N_{\rm eff}$, the primordial helium abundance, and the spectrum of primordial scalar perturbations. In [Foreman, Hotinli et al. (2009.03060)](https://arxiv.org/abs/2009.03060), we showed that external galaxy templates can be used to construct and subtract kSZ estimates from the observed maps, improving sensitivity to these targets as well as to neutrino mass, dark energy, and other CMB secondaries.

</div>


<div class="research-section" markdown="1">

## Looking Ahead

The next generation of CMB experiments and galaxy surveys — including the Simons Observatory, DESI, and the Rubin Observatory — will transform these methods from forecasts into high-precision measurements. My ongoing work focuses on preparing the analysis frameworks needed to extract the full scientific return from these datasets, continuing to bridge the simplicity of the early Universe with the complexity of the structures it gave rise to.

</div>
