# Finarg-1_ARC_-BDF4NLI
<img width="967" alt="image" src="https://github.com/nlptmu/Finarg-1_ARC_-BDF4NLI/assets/113884253/2ca99174-8508-4cae-8812-876ef1d3ea01">/n

The system architecture of our proposed method is shown in Figure.
First, the Preprocessing Module is crucial in readying data for subsequent steps.Tailored to model needs and the voting process, it handles tasks like padding, truncation, and adding special tokens like [CLS] and [SEP] for Transformer-based models. This module also enhances the dataset by employing techniques like text augmentation, especially beneficial for limited datasets. The Voting Mechanism boosts the prediction performance for the goal.
The firm of dataset is Given two sentences s1 and s2, the problem of this task can be defined as creating a method m is expected to determine the relationship between s1 and s2, categorizing it into one of the three relation class R={support, attack, none}, ensuring high accuracy in discerning the intricate intersentential relations. To begin, we paired the dataset, inherently composed of two discrete. texts. This joint processing was facilitated through a transformer-based language model. A pivotal step here involved the integration of the [SEP] token, seamlessly interspersed between these paired texts, laying a robust groundwork for impending analyses.
