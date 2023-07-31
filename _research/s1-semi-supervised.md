---
title: "Semi-supervised Learning"
collection: research
permalink: /research/s1-semi-supervised
location: "ORNL and NCSU"
---

Research on classification with limited ground-truth data, aggregate classes, ...

<ul>
  <li>Our past research has successfully addressed two well-known limitations in remote sensing image classification: 
    limited ground-truth (small or limited training samples) and aggregate classes (e.g., “forest” aggregate class label 
    instead of actual classes like “hard-wood forest”, “coniferous forest”). Semi-supervised learning methods, which are 
    designed to address paucity of labeled samples in classification, assume that both labeled and unlabeled samples come 
    from the same underlying distribution. However, this assumption is violated in remote sensing image classification due 
    to prevalence of aggregate classes. For example, USGS-NLCD uses 21-classes, whereas the USDA-CDL employs more than 100 
    classes in classifying remote sensing data. That is, the number of labeled classes are always less than the total number 
    classes. This violation of in semi-supervised learning leads intraclass variance when the model is learned from pooled 
    labeled and unlabeled samples. To address these challenges, I developed novel algorithms that addressed several subproblems 
    including: (i) finding the optimal number of clusters from the unlabeled data using GX-Means, and (ii) matching classes 
    (labeled samples) and clusters (unlabeled samples) based on the relative entropy principle. Using this approach, samples 
    from additional components (or clusters) can be eliminated or treated as new classes.
    <ul>
      <li>Ranga Raju Vatsavai, Christopher T. Symons, Varun Chandola, Goo Jun: GX-Means: A model-based divide and merge 
        algorithm for geospatial image clustering.  Procedia Computer Science 4 (ICCS-2011) 186–195 </li>
      <li>Ranga Raju Vatsavai, Shashi Shekhar, Budhendra L. Bhaduri: A Learning Scheme for Recognizing Sub-classes 
        from Model Trained on Aggregate Classes. Joint IAPR International Workshops on Statistical Techniques in Pattern 
        Recognition (SPR) and Structural and Syntactic Pattern Recognition (SSPR) 2008: 967-976</li>
      <li>Ranga Raju Vatsavai, Shashi Shekhar, Thomas E. Burk: An efficient spatial semi-supervised learning algorithm. 
        Int. J. Parallel Emergent Distributed Syst. 22(6): 427-437 (2007)</li>
    </ul>
  </li>
</ul>
