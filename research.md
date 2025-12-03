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

A relatively underexplored area in computational neuroscience is the relationship between cellular-level biophysical diversity, such as heterogeneous receptor types, and their impact on network-level computation and behavior. One key feature of such diversity is the introduction of temporal heterogeneity in neuronal dynamics. Different ionotropic and metabotropic receptor types influence membrane time constants by modulating ionic conductances on varying timescales, leading to a distribution of effective integration windows across a population of neurons. Recurrent neural networks (RNNs) are computational models inspired by biological neural networks, in which neurons are connected in loops that allow information to persist over time, making them a useful tool for studying temporal integration and memory in neural circuits. However, in most RNNs, commonly used to model neural activity during cognitive tasks, neuronal time constants are typically fixed and homogeneous across the network. While some machine learning research has explored the benefits of time constant heterogeneity, either by assigning individual time constants to units and/or by learning them during training in architectures such as LSTMs or GRUs, these studies have largely focused on engineering tasks like image or sequence classification. In computational neuroscience, recent work has shown that imposing heterogeneity in neuronal time constants, particularly by organizing neurons into groups with distinct timescales, can improve model performance on tasks with temporal or memory components. However, to our knowledge, a comprehensive analysis of how the distribution of time constants, e.g., uniform, bimodal, affects task performance and learning dynamics in RNNs has not been conducted. To investigate this, we designed a task that requires integrating information across multiple timescales. We then compared the training performance and learned solutions of standard RNNs and dimensionality-restricted low-rank RNNs on this task, across different distributions of intrinsic timescales. We found that uniformly distributed time constants consistently yielded the best performance, bringing the network’s initial temporal structure closer to the time constants it eventually learned through training.

This is a project that another NIH postbac and my friend, [Aidan Higgs](https://github.com/ahiggs13), and I developed almost entirely on our own, from initial idea to a full poster presentation at NIMH Scientific Training Day this past September. I'm pretty proud of it for those reasons. You can find the [poster](/pdfs/timescale_rnn_final.pdf) and GitHub [repo](https://github.com/ahiggs13/timescale_RNN) attached.

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
