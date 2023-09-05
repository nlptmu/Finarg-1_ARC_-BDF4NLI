# Finarg-1_ARC_-BDF4NLI
<img width="967" alt="image" src="https://github.com/nlptmu/Finarg-1_ARC_-BDF4NLI/assets/113884253/2ca99174-8508-4cae-8812-876ef1d3ea01">  

The system architecture of our proposed method is shown in Figure.
First, the Preprocessing Module is crucial in readying data for subsequent steps.Tailored to model needs and the voting process, it handles tasks like padding, truncation, and adding special tokens like [CLS] and [SEP] for Transformer-based models. This module also enhances the dataset by employing techniques like text augmentation, especially beneficial for limited datasets. The Voting Mechanism boosts the prediction performance for the goal.

The firm of dataset is Given two sentences s1 and s2, the problem of this task can be defined as creating a method m is expected to determine the relationship between s1 and s2, categorizing it into one of the three relation class R={support, attack, none}, ensuring high accuracy in discerning the intricate intersentential relations. To begin, we paired the dataset, inherently composed of two discrete. texts. This joint processing was facilitated through a transformer-based language model. A pivotal step here involved the integration of the [SEP] token, seamlessly interspersed between these paired texts, laying a robust groundwork for impending analyses.

In addition, there was an inherent imbalance in the dataset that was the most noticeable, which inevitably ushered in less-than-optimal results. To navigate this impediment, we undertook a multipronged
strategy: (1) SMOTE Data Augmentation (RS): An experimental foray into the Synthetic Minority Over-sampling Technique (SMOTE) was undertaken. This technique artfully rebalanced the dataset by synthetically oversampling the minority classes. (2) Class Weighting (CL): Parallelly, we ventured into Class Weighting, applied judiciously to the loss function. The essence of this tactic was to allocate disparate weights to classes in alignment with their frequency. This inherently accorded higher significance to the more sparsely represented classes. In the integration of BERT for enhancing the performance, we employed a soft voting ensemble technique to amalgamate both BART and DEBERTA seamlessly.

Noteworthy, in the study by (Chang et al., 2022), there's compelling evidence illustrating the efficacy of the Log Likelihood Ratio (LLR) in generating and amalgamating linguistic patterns, leading to a substantial enhancement in predictive accuracy. Drawing inspiration from this revelation, we harness LLR to discern the significance of individual words nested within both sentences. This empowers us to cultivate distinguishing linguistic patterns rooted in their relationship scores. Thus Subsequently, this crafted feature space is seamlessly concatenated with the latent vector derived post an ensemble with BERT.

## Reference
Please cite these papers in your publications if BDF4NLI helps your research.

  @author = {Hen-You Lin, Eugene Sy, Tzu-Cheng Peng, Shih-Hsuan Huang, Yung-Chung Chang},
    title = {TMUNLP at the NTCIR-17 FinArg-1 Task},
    year = {2023}
  @author = {Eugene L. Sy,Tzu-Cheng Peng, Shih-Hsuan Huang, Hen-You Lin, Yung-Chung Chang},
    title = {Fine-Grained Argument Understanding with BERT Ensemble Techniques:A Deep Dive into Financial Sentiment Analysis},
    year = {2023}

    
