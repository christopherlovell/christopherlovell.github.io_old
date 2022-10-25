---
layout: page
permalink: /research/
title: Research
---

Below are some brief summaries of research areas I am currently working in, or have recently worked on. If you're interested in any of these topics and would like to chat further, please <a href="/contact/">get in touch!</a>

<ul>
<li><a href="#FLARES">First Light And Reionisation Epoch Simulations (FLARES)</a></li>
<li><a href="#Machine Learning & Astronomy">Machine Learning & Astronomy</a></li>
<li><a href="#EVS">Extreme Value Statistics</a></li>
<li><a href="#SMGs">Sub-millimetre galaxies in simulations</a></li>
<li><a href="#Galaxy Protoclusters">Galaxy Protoclusters</a></li>
</ul>

{% include page_divider.html %}




<h2><a name="FLARES">First Light And Reionisation Epoch Simulations (FLARES)</a></h2>

Cosmological hydrodynamic simulations have, in recent years, become capable of matching key distribution functions in the local universe, such as those of stellar mass and star formation rate. 
However, high resolution, large volume simulations  have rarely been tested in the high redshift ($z > 5$) regime, particularly in the most overdense environments.
Creating models that fit both high redshift and low redshift observables self consistently is a significant challenge, but key to understanding the properties of galaxies in the first billion years of the universe's history, and how this affects their latter evolution.
Such models are also necessary to make detailed predictions, and plan observations, for upcoming space based instruments, such as JWST, WFIRST and Euclid.

<img class="small" src="/images/all_components.png" title="FLARES components">
<p style="text-align:center; font-style:italic">The column density of gas, stars and dark matter in the most overdense region in the FLARES sample.</p>

<a href="flaresimulations.github.io/" target="source">The First Light And Reionisation Epoch Simulations (FLARES)</a> are one approach to these issues.
FLARES consists of a suite of 40 'zoom' simulations using a modified version of the <a href="http://icc.dur.ac.uk/Eagle/" target="blank">EAGLE</a> code.
We selected regions at high redshift, with a range of overdensities, from an enormous periodic dark matter-only volume, and resimulated these with full hydrodynamics at fiducial EAGLE resolution. 
I led the first release paper (<a href="https://arxiv.org/abs/2004.07283">Lovell et al 2021; arXiv:2004.07283</a>) in which we study predictions for the galaxy stellar mass function, star formation rate function and star-forming sequence.
Below is an introductory talk that I gave at the 2020 SAZERAC meeting (with awkward slide transition requests due to a technical error...!).

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/95pZbjGGpjA" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>

The FLARES project has now produced a number of published papers on a range of topics.
For further details please check out our dedicated website, <a href="https://flaresimulations.github.io/">flaresimulations.github.io</a>, where you can find data products and visualisations.
I am currently working on predictions for the passive galaxy population at $z > 5$, some early results are presented in this talk at SAZERAC 2021 <a href="https://www.youtube.com/watch?v=VRHcg5EHJOs">here</a>.

<!--img class="small" src="/images/flares_fom.png" title="FLARES figure of merit">
<p style="text-align:center; font-style:italic">Figure of merit showing the distribution of a number of simulations on a plane of dark matter element resolution against simulated volume. FLARES, whilst explicitly simulating a similar volume to similar resolution simulations, has an 'effective' volume 4 orders of magnitude larger when combining the regions.</p-->



<h2><a name="Machine Learning & Astronomy">Machine Learning & Astronomy</a></h2>

I am keenly interested in the interface between simulations and machine learning (ML) methods, and have written a number of papers on a variety of related topics.

Recently, I submitted a paper (<a href="https://arxiv.org/abs/2106.04980">Lovell et al. 2021c</a>) that attempts to predict the baryonic properties of dark matter halos directly from their dark matter properties using matched hydrodynamic and dark matter only (DMO) simulations.
Whilst this method has been demonstrated in previous works, the unique thing about our approach was that we used both periodic and zoom simulations of cluster environments, which allowed us to sample both mean and overdense regions. 
This then allowed us to apply the trained model to a much <em>larger</em> DMO simulation, the $800 \mathrm{Mpc^3}$ P-Millennium simulation, and predict distribution functions and clustering statistics in this much larger volume for a fraction of the cost of a full-hydro simulation.

<img class="small" src="/images/ml_sims.png" title="">
<p style="text-align:center; font-style:italic">The simulations, features and predictors in the EAGLE and C-EAGLE simulations, as well as the dark matter only P-Millennium simulation to which we applied our model.</p>

<center>
<iframe width="560" height="315" src="https://www.youtube.com/watch?v=I66Sd4yUW9Y&t=3237s" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>

I have also developed an online tool, <a href="https://www.christopherlovell.co.uk/sengi/">Sengi</a>, for viewing the outputs of Stellar Population Synthesis (SPS) models in the browser. 
It's fully client-side Javascript, using Non-negative matrix factorisation to serve the large grids in age-metallicity space in a fast, lightweight tool (paper <a href="https://www.sciencedirect.com/science/article/pii/S2213133720300986?via%3Dihub">here</a>).

In <a href="https://arxiv.org/abs/1903.10457" target="blank">Lovell et al. 2019</a> I worked with <a href="https://www.drvivianaacquaviva.com/" target="blank">Prof. Viviana Acquaviva</a> at City University New York to develop a new tool for predicting Star Formation Histories (SFH).
We trained a Convolutional Neural Network to learn the relationship between spectra and SFH in the EAGLE and Illustris simulations, and the applied this to the SDSS catalogue. 
Below is a talk I gave on this research at the Royal Astronomical Society meeting, <a href="https://ras.ac.uk/events-and-meetings/ras-meetings/machine-learning-and-artificial-intelligence-applied-astronomy" target="blank">"Machine Learning and Artificial Intelligence applied to astronomy"</a> in March 2019 (slides available <a href="https://drive.google.com/file/d/1AoFtiu9alxbwuBQ7Dp9ujX9g8XZmTudq/view" target="blank">here</a>).
We followed this up with a paper (<a href="https://arxiv.org/abs/2012.00066">Acquaviva, Lovell & Ishida, 2020</a>) accepted for the 2020 NeurIPS workshop "Machine Learning and the Physical Sciences", in which we attempt to model the 'generalization error', and provide a means of estimating how models trained on simulation data might perform on real-world data.

<center>
<iframe width="560" height="315" src="https://www.youtube.com/embed/R2MZ5HXZH_A" title="YouTube video player" frameborder="0" allow="accelerometer; autoplay; clipboard-write; encrypted-media; gyroscope; picture-in-picture" allowfullscreen></iframe>
</center>

<!--a href="https://www.youtube.com/watch?v=R2MZ5HXZH_A" target="blank"><img class="small" src="/images/RAS2019_talk.jpg" title="RAS 2019 talk"></a-->

<!-- <h2><a href="High Redshift Galaxy Evolution" name="High Redshift Galaxy Evolution">High Redshift Galaxy Evolution</a></h2> -->

<h2><a name="EVS">Extreme Value Statistics</a></h2>

What's the most massive galaxy we expect in the observable Universe?
And do any currently observed galaxies break our cosmological model?
In order to answer these questions we used Extreme Value Statistics to make predictions for the most massive halo and galaxy, comparing to both simulations and recent JWST observations at $z > 8$.
We found that many recent JWST candidates are in significant tension with our current cosmological model.
Check out the paper (<a href="https://arxiv.org/abs/2208.10479" target="source">Lovell et al. 2022; arXiv:2208.10479</a>) for more details.

<img class="small" src="/assets/jwst_evs.png" title="JWST EVS">
<p style="text-align:center; font-style:italic">The predicted distribution of stellar mass of the most massive galaxy as a function of redshift, compared to recent JWST candidates.</p>

<h2><a name="SMGs">Sub-millimetre galaxies in simulations</a></h2>
Sub-millimetre galaxies, or SMGs, are an enigmatic population of galaxies in the early universe that are incredibly bright in submillimetre wavelengths ($\sim 100 \mathrm{\mu m} - 1 \mathrm{mm}$), forming huge numbers of stars.
It has been very difficult to model these objects in cosmological simulations whilst still self-consistently matching other observational constraints, such as the galaxy stellar mass function, at $z = 0$, and many authors have proposed alternative modelling approaches, such as a varibale IMF, to explain them.
For a concise summary of the issues faced modelling these objects, see <a href="https://twitter.com/desikanarayanan/status/1277940211285180416" target="_blank">this thread from Desika!</a>

<img class="small" src="/images/simba_render.png" title="SIMBA SMG render">
<p style="text-align:center; font-style:italic">An example SMG showing the gas, stellar and dust distribution, as well as the resolved and integrated $S_{850}$ emission.</p>

In Lovell et al. 2021a (<a href="https://arxiv.org/abs/2006.15156">arXiv:2006.15156</a>), we used the <a href="https://arxiv.org/abs/1901.10203">SIMBA</a> simulation combined with the radiative transfer package <a href="https://arxiv.org/abs/2006.10757">Powderday</a> to model the sub-mm emission, and found unprecedented agreement with observationally inferred integrated number counts from single-dish instruments.
We assessed the impact of unassociated blending by building a lightcone, and found a slight boost in the normalisation of at the bright end.
The good agreement is driven primarily by the good match to IR-constraints on the high-redshift star formation rate function in SIMBA, as well as the self-consistent dust model which leads to higher dust masses compared to using a fixed dust-to-metals ratio, by up to a factor of 2.5.

<!--img class="small" src="/images/square_counts.png" title="SIMBA 850 micron counts">
<p style="text-align:center; font-style:italic">$S_{850}$ counts from the SIMBA simulation, compared with observational constraints, as well as predictions from the EAGLE model.</p-->

In a subsequent work (<a href="https://arxiv.org/abs/2106.11588">Lovell et al. 2022; arXiv:2106.11588</a>), we studied how the emission of SMGs is dependent on their morphology and orientation, and found an 'orientation bias' in observations of SMGs. 
This has knock-on effects on inferred properties, such as dust temperatures and IR luminosities, as well as SFRs and other derived properties.
It also manifests as a selection effect, that is both wavelength and redshift dependent, and we provide a <a href="https://github.com/christopherlovell/orientation_bias">tool</a> for modelling this for arbitrary surveys. 

<img class="small" src="/images/smg_orientation.png" title="Simba SMG orientation dependence">
<p style="text-align:center; font-style:italic">Four massive star forming galaxies in Simba, viewed from three orthogonal angles (top three rows), and their integrated sub-mm emission (bottom row) from 50 random orientations.</p>


<h2><a name="Galaxy Protoclusters">Galaxy Protoclusters</a></h2>

Galaxy clusters are the largest collapsed objects in the universe, comprising of a highly evolved galaxy population embedded in a hot, rarefied InterCluster Medium (ICM). Their pre-collapse progenitors, known as galaxy *protoclusters*, are host to some of the most extreme objects (in terms of mass, star formation rate and nuclear activity) at these early times.
Protoclusters are of significant interest for understanding the environmental dependence of galaxy evolution at early times, as well as the build-up, enrichment and heating of the ICM.

<img class="small" src="/images/dm_example.png" title="Simulated Protocluster">
<p style="text-align:center; font-style:italic">The dark matter distribution in a Protocluster at $z \sim 5$ simulated with the EAGLE code</p>
<!-- <img class="small" src="/images/gas_test_zoom_1_r_1.gif" title="Simulated Protocluster">
<p style="text-align:center; font-style:italic">Gas distribution in a Protocluster at $z \sim 5$ simulated with the EAGLE code</p> -->

Protoclusters do not yet host an X-ray emitting ICM, and so are primarily identified through 3D galaxy overdensities. 
In <a href="http://adsabs.harvard.edu/cgi-bin/bib_query?arXiv:1710.02148" target="blank">Lovell et al. 2018</a> I studied in detail the relationship between galaxy overdensity and the presence and descendant mass of protoclusters in the <a href="http://galformod.mpa-garching.mpg.de/public/LGalaxies/" target="blank">L-galaxies</a> semi-analytic model.

<br><br>

<!-- <h2><a name="Extreme Value Statistics">Extreme Value Statistics</a></h2>

During my Masters I worked with <a href="https://telescoper.wordpress.com/" target="blank">Prof. Peter Coles</a> and <a href="http://www.jb.man.ac.uk/~harrison/" target="blank">Dr. Ian Harrison</a> on <a href="https://www.ncl.ucar.edu/Applications/extreme_value.shtml" target="blank">Extreme Value Statistics</a>, a technique for predicting the most extreme objects in a distribution. I studied the EVS predictions for the halo masses of galaxy clusters and compared to numerical simulation predictions, as well as EVS predictions for the largest voids in the universe, utilising excursion set theory.

<img class="vsmall" src="/images/masters_project_ss.png" title="WebbUK">
<p style="text-align:center; font-style:italic">The dark matter distribution in a small volume containing a massive cluster, simulated using the <a href="http://enzo-project.org/" target="blank">ENZO</a> code</p> -->
