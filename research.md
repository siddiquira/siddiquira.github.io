---
layout: page
title: Research
permalink: /research/
---

These are some selected research projects that have resulted in something tangible and/or that I really enjoyed.

#### Machine learning analyses of optogenetic perturbations in mouse V1

<figure>
  <img src="/imgs/mouse_stim_cartoon.png" style="width: 100%; height: auto; display: block; margin: 0 auto;">
  <figcaption>
    <em>Two-photon calcium imaging with targeted optogenetic perturbations in mouse V1. (Left) Schematic of holographic optogenetic stimulation of selected neurons (red) while recording population activity. (Middle) Example calcium imaging field of view showing identified neurons (colored circles). (Right, two panels) Neurons grouped by different ensemble sizes; colors correspond to a given ensemble.</em>
  </figcaption>
</figure>

Something will appear here eventually.

#### Recurrent neural networks with diverse intrinsic timescales

<figure>
  <img src="/imgs/beiran_2021.jpg" style="width: 70%; height: auto; display: block; margin: 0 auto;">
  <figcaption>
    <em>Reproduced from Beiran et al., 2021.</em>
  </figcaption>
</figure>

This is a largely self-led project with me and another postbac at NIH, [Aidan Higgs](https://github.com/ahiggs13), that we presented together at the NIMH Scientific Training Day back in September of this year. The project grew out of our participation in NIH’s Computational Neuroscience Journal Club, where many of our discussions this year have centered on RNNs and their use in modeling different neural computations. A question that arose, originally posed by an experimentalist in the group, Dr. Hugo Tejeda, who studies opioid receptors, captured our interest. He asked how the diversity observed at the single-neuron level, particularly in receptor expression, might influence the higher-level computations implemented by the kinds of RNNs we were studying. His question highlighted a broader issue: the relationship between cellular-level biophysical heterogeneity and network-level computation. One key mechanism linking these levels is temporal heterogeneity in neuronal dynamics. Different ionotropic and metabotropic receptors shape membrane time constants by modulating ionic conductances over distinct timescales. This produces a distribution of effective integration windows across neurons in a circuit. In contrast, most RNN models used in computational neuroscience assume fixed, homogeneous time constants. While some machine-learning studies have introduced time-constant heterogeneity, either by assigning each unit its own time constant or by learning them in architectures such as LSTMs or GRUs, these efforts have primarily targeted engineering tasks like sequence modeling or image classification. Recently, a few computational neuroscience papers have shown that grouping neurons into clusters with distinct timescales can improve RNN performance on tasks with temporal or memory demands. However, to our knowledge, no systematic analysis has examined how different distributions of time constants (e.g., uniform, bimodal, heavy-tailed) affect task performance, learning dynamics, or the emergence of neural representations. Our project takes a first step toward filling that gap. We trained RNNs on tasks requiring multiple working-memory timescales and compared performance across networks initialized with different distributions of intrinsic time constants. We found that uniformly distributed time constants consistently yielded the best performance, bringing the network’s initial temporal structure closer to the time constants it eventually learned through training. 

#### Instability driven by partial relaxation of zero-row-sum constraints in random networks

<figure>
  <img src="/imgs/rajan_abbot_2006_fig1.png" style="width: 90%; height: auto; display: block; margin: 0 auto;">
  <figcaption>
    Numerical results for the distribution of eigenvalues in the complex plane for N = 1000.  
    (a) If excitatory and inhibitory elements are drawn from distributions with different means but the same variance, a few eigenvalues lie outside the unit circle.  
    (b) When every row of the matrix individually sums to zero, the eigenvalues lie inside the unit circle.  
    <br><br>
    <em>Reproduced from Rajan & Abbott, 2006.</em>
  </figcaption>
</figure>

Something will also appear here eventually.

The <em>Eigenvalue Value (in Neuroscience)</em> by Georgia Christodoulou and Tim Vogels helped me with this project and is a good read, but I had trouble finding it when I recently looked for it again so 
[here](/pdfs/christodoulou_vogels_2022.pdf) it is.

<style>
figure {
  margin: 2em auto 1.5em auto; /* top auto, bottom spacing to next text */
  max-width: 1200px;
}
figcaption {
  text-align: center;
  font-style: italic;
  margin-top: 8px;  /* spacing between image and caption */
  margin-bottom: 1.5em; /* spacing after caption before next text */
  line-height: 1.4;
}
</style>
