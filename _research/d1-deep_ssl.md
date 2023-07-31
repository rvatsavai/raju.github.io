---
title: "Deep Semi-supervised Learning"
collection: research
permalink: /research/d1-deep_ssl
location: "NCSU"
---

Research on Mean Teacher and  Generative Adversarial Networks (GANs) based semi-supervised learning (SSL) ...

<ul>
  <li>Our present research is exploring the semi-supervised learning in the era of deep learning. Recently we made 
    two significant contributions to address the <span style="color:red">confirmation bias </span> and 
    <span style="color:red">consistency </span> issues in well-known deep learning models. 
    The Mean Teacher (MT) model is known to suffer from confirmation bias, that is, reinforcing incorrect teacher model predictions.  
    To address this problem, we developed a simple, yet effective method called Local Clustering (LC) to mitigate the effect of 
    confirmation bias. In MT model, each data point is considered independent of other points during training; however, we note 
    that data points are likely to be close to each other in feature space if they share similar features. Motivated by this 
    observation, we cluster data points locally by minimizing the pairwise distance between neighboring data points in feature space. 
    Combined with a standard classification cross-entropy objective on labeled data points, the misclassified unlabeled data points 
    are pulled towards high-density regions of their correct class with the help of their neighbors, thus improving model performance. 
    Thorough experiments on semi-supervised benchmark datasets SVHN and CIFAR-10 showed that adding our LC loss to MT yields significant 
    improvements compared to MT and performance and comparable to the state of the art in semi-supervised learning.
  </li>
    
  <li>
    Generative Adversarial Networks (GANs) based semi-supervised learning (SSL) approaches though shown to improve classification 
    accuracy, their performance is lagging behind the state-of-the-art non-GAN based SSL approaches. We note that the lack of 
    consistency in class probability predictions on the same image under local perturbations is one of the reasons for this 
    performance gap. This problem was addressed in the past in a generic setting using the label consistency regularization, 
    which enforces the class probability predictions for an input image to be unchanged under various semantic-preserving perturbations. 
    We developed a new composite consistency regularization method in the framework of GAN based SSL and demonstrated the efficacy of 
    new approach on two SSL image classification benchmark datasets, SVHN and CIFAR-10. Our experiments show that this new composite 
    consistency regularization based semi-GAN significantly improves its performance and achieves new state-of-the-art performance 
    among GAN-based SSL approaches.
  
   <ul>
      <li>Zexi Chen, Benjamin Dutton, Bharathkumar Ramachandra, Tianfu Wu, and Ranga Raju Vatsavai (2020): 
        "Local Clustering with Mean Teacher for Semi-supervised learning." 25th International Conference on Pattern Recognition. 
      </li>
      <li>Zexi Chen, Bharathkumar Ramachandra, Ranga Raju Vatsavai (2020): Consistency Regularization with Generative Adversarial 
        Networks for Semi-Supervised Image Classification. CoRR abs/2007.03844 (under review).
      </li>   
   </ul>
  </li>
</ul>
