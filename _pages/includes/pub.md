
# 📝 Selected Publications 

<style>
.box {
  display: inline-block;
  background-color: lightgray;
}

.blue-text {
  color: blue;
}
</style>

(<sup>*</sup> indicates equal contribution;  <sup>#</sup> indicates corresponding authorship.) 


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">BMVC 2024</div><img src='images/RAZA_BMVC.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[FLARE up your data: Diffusion-based Augmentation Method in Astronomical Imaging](https://arxiv.org/abs/2405.13267) \\
<b>Raza Imam<sup>*</sup><sup>#</sup></b>, Mohammed Talha Alam<sup>*</sup>, Mohsen Guizani, Fakhri Karray.  (BMVC 2024) <a href="https://github.com/Razaimam45/PlanetX_Dxb">code(+)data</a> 

- FLARE is a diffusion-based augmentation method which initially enhances the resolution of raw input samples. Given the widespread dispersion of these raw inputs in feature space, we have implemented a two-stage augmentation strategy. Also, we introduce an optimally distributed dataset via FLARE: SpaceNet, comprising approximately 12,900 samples.

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">SPAICE 2024</div><img src='images/RAZA_CosmoCLIP.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[CosmoCLIP: Generalizing Large Vision-Language Models for Astronomical Imaging](https://arxiv.org/abs/2407.07315) \\
<b>Raza Imam<sup>*</sup><sup>#</sup></b>, Mohammed Talha Alam<sup>*</sup>, Umaima Rahman, Mohsen Guizani, Fakhri Karray.  (SPAICE 2024)

- We introduce CosmoCLIP, an astronomical image-text contrastive learning framework precisely fine-tuned on the pre-trained CLIP model using SpaceNet and BLIP-based captions. The rich semantics derived from this SpaceNet and BLIP descriptions, when learned contrastively, enable CosmoCLIP to achieve superior generalization across various in-domain and out-of-domain tasks in astronomical imaging.

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">ICCE 2024</div><img src='images/RAZA_evoke.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[EVOKE: Emotion Enabled Virtual Avatar Mapping Using Optimized Knowledge Distillation](https://ieeexplore.ieee.org/abstract/document/10444200/) \\
Maryam Nadeem<sup>#</sup>, <b>Raza Imam<sup>*</sup></b>, Rouqaiah Al-Refai<sup>*</sup>, Meriem Chkir, Mohamad Hoda, Abdulmotaleb El Saddik. (ICCE 2024) 

- EVOKE leverages knowledge distillation involving multi-label classification on the publicly available DEAP dataset, which covers valence, arousal, and dominance as primary emotional classes. Remarkably, our distilled model, a CNN with only two convolutional layers and 18 times fewer parameters than the teacher model, achieves competitive results, boasting an accuracy of 87% while demanding far less computational resources. This equilibrium between performance and deployability positions our framework as an ideal choice for virtual environment systems. Furthermore, the multi-label classification outcomes are utilized to map emotions onto custom-designed 3D avatars.

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">MICCAI 2023, spotlight</div><img src='images/RAZA_seda.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[SEDA: Self-ensembling ViT with Defensive Distillation and Adversarial Training for Robust Chest X-Rays Classification](https://arxiv.org/abs/2308.07874) \\
<b>Raza Imam<sup>#</sup></b>, Ibrahim Almakky, Salma Alrashdi, Baketah Alrashdi, Mohammad Yaqub. (MICCAI 2023) <a href="https://github.com/Razaimam45/SEDA">code</a> 

- SEDA utilizes efficient CNN blocks to learn spatial features with various levels of abstraction from feature representations extracted from intermediate ViT blocks, that are largely unaffected by adversarial perturbations. Furthermore, SEDA leverages adversarial training in combination with defensive distillation for improved robustness against adversaries. Extensive experiments performed with the proposed architecture and training paradigm on publicly available Tuberculosis x-ray dataset shows SOTA efficacy of SEDA compared to SEViT in terms of computational efficiency with 70x times lighter framework and enhanced robustness of +9%.

</div>
</div>


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">MIUA 2023</div><img src='images/RAZA_defensive_diffusion.png' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">
[On enhancing the robustness of Vision Transformers: Defensive Diffusion](https://arxiv.org/abs/2305.08031) \\
  <b>Raza Imam</b>, Muhammad Huzaifa<sup>#</sup>, Mohammed El-Amine Azz.
  (MIUA 2023) <a href="https://github.com/Muhammad-Huzaifaa/Defensive_Diffusion">code</a> 

- In this work, we introduced a defensive diffusion technique as an adversarial purifier to eliminate adversarial noise introduced by attackers in the original image. By utilizing the denoising capabilities of the diffusion model, we employ a reverse diffusion process to effectively eliminate the adversarial noise from the attack sample, resulting in a cleaner image that is then fed into the ViT blocks. Extensive experiments conducted on a publicly available Tuberculosis X-ray dataset validate the computational efficiency and improved robustness achieved by our proposed architecture.
</div>
</div>


<!-- <div class='paper-box'><div class='paper-box-image'><div><div class="badge">UAI 2023</div><img src='images/RAZA_brain tumor.jpeg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[Optimizing Brain Tumor Classification: A Comprehensive Study on Transfer Learning and Imbalance Handling in Deep Learning Models](https://arxiv.org/abs/2308.06821) \\
<b>Raza Imam<sup>#</sup></b>, Mohammed Talha Alam. 
(UAI 2023) <a href="https://github.com/Razaimam45/AI701-Project-Transfer-Learning-approach-for-imbalance-classification-of-Brain-Tumor-MRI-">code</a> 

- In this work, we present a novel deep learning-based approach, called Transfer Learning-CNN, for brain tumor classification using MRI data. The proposed model leverages the predictive capabilities of existing publicly available models by utilizing their pre-trained weights and transferring those weights to the CNN. We investigate the impact of different loss functions, including focal loss, and oversampling methods, such as SMOTE and ADASYN, in addressing the data imbalance issue. Notably, the proposed strategy, which combines VGG-16 and CNN, achieved an impressive accuracy rate of 96%, surpassing alternative approaches significantly.
</div>
</div> -->


<div class='paper-box'><div class='paper-box-image'><div><div class="badge">Elsevier JKSU</div><img src='images/RAZA_abe_survey.jpg' alt="sym" width="100%"></div></div>
<div class='paper-box-text' markdown="1">

[A systematic literature review of attribute based encryption in health services](https://www.sciencedirect.com/science/article/pii/S1319157822002269) \\
<b>Raza Imam</b>, Kaushal Kumar, Syed Mehran Raza, Rumi Sadaf, Faisal Anwer<sup>#</sup>, Noor Fatima, Mohammad Nadeem, Mohamed Abbas, Obaidur Rahman. (Elsevier JKSU)

- This survey presents a systematic and comprehensive study of ABE works concerning E-Health as the authors rigorously investigate healthcare-focused ABE frameworks and examine them based on various descriptive criteria, along with categorizing them systematically in 10 distinct domains and sub-domains, ultimately offering observations and potential recommendations. The descriptive research design, significant findings along with the suggested future works will help future research in ABE to secure the existing E-Health data sharing more effectively.
</div>
</div>

<!-- - <span style="color: blue; background-color: lightgray; "> ICCV 2023 </span>&nbsp;[Rethinking Data Distillation: Do Not Overlook Calibration](https://arxiv.org/abs/2307.12463), D. Zhu, B. Lei, **Jie Zhang**, Y. Fang, Y. Xie, R. Zhang, D. Xu. 
- <span style="color: blue; background-color: lightgray; "> ICCV 2023 </span>&nbsp;[TARGET: Federated Class-Continual Learning via Exemplar-Free Distillation](https://arxiv.org/abs/2303.06937), **Jie Zhang**, Chen Chen, Weiming Zhuang, Lingjuan Lv. 
- <span style="color: blue; background-color: lightgray; "> ICLR 2023 </span>&nbsp;[IDEAL: Query-Efficient Data-Free Learning from Black-Box Models](https://openreview.net/pdf?id=ConT6H7MWL), **Jie Zhang<sup>*</sup>**, Chen Chen<sup>*</sup>, Lingjuan Lyu. <a href="https://github.com/SonyResearch/IDEAL">code</a> 
- <span style="color: blue; background-color: lightgray; "> Best Student Paper Award, AAAI 2022 FL workshop </span>&nbsp;[GEAR: A Margin-based Federated Adversarial Training Approach](https://federated-learning.org/fl-aaai-2022/Papers/FL-AAAI-22_paper_34.pdf), Chen Chen<sup>*</sup>, **Jie Zhang**<sup>*</sup>, Lingjuan Lyu.  -->

