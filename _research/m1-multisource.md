---
title: "Multisource, Multimodal, Multitemporal Classification"
collection: research
permalink: /research/m1-multisource
---

Research on multi-* data mining and machine learning, ...

<ul>
  <li> <span style="color:red">Classification:</span> 
    In many practical situations, data is generated from multiple sources (e.g., satellite image datasets 
    which are often modeled as continuous random variables, and GIS data like soil maps, slope, aspect, etc., 
    which are modeled as discrete random variables), multiple sensors (e.g., optical vs. radar images), 
    multitemporal (MODIS daily NDVI data), and multi-resolution (Landsat ETM+ 30 meter vs DigitalGlobe's 
    WorldView-3 data at 31 cm panchromatic, 1.24 m multispectral, and 3.7 m short-wave infrared resolution 
    images). In the past, we developed a mixture model based semi-supervised learning
   that jointly exploits features that are continuous and discrete. Our recent work is focused on joint
   exploitation of signals from high spatial and spectral resolution images (but low temporal resolution)
   and high temporal (but low spatial and spectral) resolution images for crop classification.  Traditionally, 
   multispectral remote sensing imagery has been widely used for mapping crops worldwide. However, single 
   date imagery does not capture temporal characteristics (phenology) of growing crops, leading to imprecise 
   crop maps and food estimates. On the other hand, purely temporal classification approaches also produce 
   inaccurate crop maps as they do not account for spatial autocorrelations. To address this well-known
   practical challenge, we developed a novel multimodal deep learning solution that jointly exploits spatial-spectral 
   and temporal (phenological) properties to identify major crop types. Using a two stream deep learning
   architecture, spatial characteristics are captured via a spatial stream consisting of very high resolution 
   images (single date, 1-meter, 3-spectral bands, USDA NAIP) with a CNN and the phenological characteristics 
   via a temporal stream images (biweekly, 250m, MODIS NDVI) with an LSTM. Experimental results showed that 
   the proposed multimodal solution reduces prediction error by 60% (published in ACM KDD 2020).
   <ul>
      <li>Krishna Karthik Gadiraju, Bharathkumar Ramachandra, Zexi Chen, Ranga Raju Vatsavai: 
      Multimodal Deep Learning Based Crop Classification Using Multispectral and Multitemporal 
      Satellite Imagery. The 26th ACM SIGKDD Conference on Knowledge Discovery and Data Mining, KDD 2020: 3234-3242</li>
      <li>Ranga Raju Vatsavai: Multitemporal data mining: From biomass monitoring to nuclear proliferation detection. 
      8th International Workshop on the Analysis of Multitemporal Remote Sensing Images, MultiTemp 2015, Annecy, 
      France. (Keynote) </li>
      <li>Varun Chandola, Ranga Raju Vatsavai: Multi-temporal remote sensing image classification - A multi-view approach. 
      Proceedings of the 2010 Conference on Intelligent Data Understanding, CIDU 2010: 258-270 </li>
      <li>Ranga Raju Vatsavai, Budhendra L. Badhuri, Shashi Shekhar, Thomas E. Burk:
      Multisource Data Classification using a Hybrid Semi-Supervised Learning Scheme. IGARSS (3) 2008: 1016-1019 </li>
    </ul>
  </li>
  
   <li> <span style="color:red">Change Detection: </span>
    In monitoring man-made critical infrastructures which requires comparing multi-sensor and 
    multi-resolution images. These images may not have been perfectly georegistered. Traditional remote sensing based change 
    detection approaches compare individual (or first/second order neighborhood) pixels from same sensor data to identify changes. 
    However, image to image and map to image registrations, through increasingly becoming accurate, contains errors (often by 
    several pixels), as a result direct pixel-wise comparison is not accurate. In addition, often changes happen at 
    a bigger spatial footprint than individual pixels. In addition, in adverse climatic conditions (e.g., during hurricanes) 
    it would hard get good optical (or same) sensor data for pre- and post-events. To overcome these limitations, we developed 
    a novel and unique image patch-based probabilistic change detection that is shown to be not only accurate than traditional methods, 
    but also allows utilization of multi-resolution and multi-sensor data. The results were published in leading venues (Procedia 
    Computer Science, Vol. 9, 2012; Demo paper at ICDM 2012), and has been extensively used in several NGA, DOD, 
    and DHS sponsored projects at the ORNL.
    
   <ul>
      <li>Ranga Raju Vatsavai: Rapid Damage eXplorer (RDX): A Probabilistic Framework for Learning Changes from 
        Bitemporal Images. IEEE International Conference on Data Mining (ICDM: Demo Paper) 2012: 906-909</li>
      <li>Ranga Raju Vatsavai, Jordan Graesser: Probabilistic Change Detection Framework for Analyzing 
        Settlement Dynamics Using Very High-resolution Satellite Imagery. ICCS 2012: 907-916</li>
      <li>Varun Chandola, Ranga Raju Vatsavai: A Gaussian Process Based Online Change Detection Algorithm for 
        Monitoring Periodic Time Series. SIAM Data Mining Conference (SDM 2011): 95-106 </li>
   </ul>
  </li>
</ul>
