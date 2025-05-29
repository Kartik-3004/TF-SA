<div align="center">

# Training-Free Stylized Abstraction

[Aimon Rahman*](https://aimansnigdha.github.io) &emsp; [Kartik Narayan*](https://kartik-3004.github.io/portfolio/) &emsp; [Vishal M. Patel](https://engineering.jhu.edu/faculty/vishal-patel/)  

Johns Hopkins University

<a href='https://kartik-3004.github.io/TF-SA/'><img src='https://img.shields.io/badge/Project-Page-blue'></a>
<a href='https://arxiv.org/abs/2505.22663'><img src='https://img.shields.io/badge/Paper-arXiv-red'></a>

</div>

Official implementation of **[Training-Free Stylized Abstraction](https://kartik-3004.github.io/TF-SA/)**.
<hr />

## What is Stylized Abstraction ?
<p align="center" width="100%">
  <img src='docs/static/images/intro_figs.png'>
</p>

Stylized abstraction involves exaggerating or simplifying the features of a subject to create a stylized representation. Rather than aiming for photorealism, it emphasizes recognizable traits that evoke the subject's concept or identity (Illustrated in Figure 1.(a)). Stylized representation aims to capture the essence of a subject through visual abstraction, focusing less on exact likeness and more on the retention of key, recognizable features. For instance, a knitted doll or a LEGO figure of Einstein may omit intricate facial geometry or biometric precision, yet still be immediately identifiable due to consistent visual traits such as his distinctive hair, mustache, or attire. These features serve as semantic anchors, allowing viewers to recognize the subject even in highly abstracted or playful forms. This form of representation is widespread in media, animation, and merchandising, where retaining a character's identity in a simplified, reproducible form is essential. Terms like personified toy representation or iconic stylization are often used to describe such instances. Unlike traditional image-to-image translation, which typically enforces structural consistency, stylized abstraction embraces simplification, distortion, or even exaggeration to evoke familiarity and conceptual identity.

---

## Contributions
<p align="center" width="100%">
  <img src='docs/static/images/main_figure.png'>
</p>

## 🔑 Key Contributions

- **🧠 Training-Free Stylized Abstraction Framework**  
  A fully training-free pipeline that generates stylized abstractions from a single input image by leveraging inference-time scaling in vision-language models (VLLMs) to extract and preserve identity-relevant features.

- **🔁 Cross-Domain Rectified Flow Inversion**  
  A novel latent reversal strategy using rectified flows to reconstruct subject structure in the abstracted style domain, guided by style-dependent priors rather than photo-realistic inversions.

- **⏱️ Style-Aware Temporal Scheduling**  
  A VLLM-driven controller that dynamically modulates structural restoration, balancing semantic identity preservation with stylistic exaggeration during the generation process.

- **🔄 Multi-Round Abstraction-Aware Generation Loop**  
  An iterative, VLLM-in-the-loop process where missing or misaligned identity cues are identified and reintegrated across multiple rounds—achieving convergence without any model fine-tuning.

- **🧪 StyleBench: Human-Aligned Evaluation Protocol**  
  A GPT-based evaluation metric tailored for abstraction styles, explicitly designed to measure style adherence, identity preservation, and fusion quality—where traditional pixel-level metrics fall short.

With our proposed work, we are able to achieve strong generalization across unseen identities and styles. We demonstrate through extensive experiments (quantitative metrics like KID and CLIPScore, plus human studies) that the framework generalizes robustly to a wide variety of abstract styles (e.g., LEGO, knitted dolls, South Park) and out-of-distribution, everyday subjects, all in a fully open-source setup.


> **<p align="justify"> Abstract:** *Stylized abstraction synthesizes visually exaggerated yet semantically
> faithful representations of subjects, balancing recognizability with perceptual distortion. Unlike
> image-to-image translation, which prioritizes structural fidelity, stylized abstraction demands selective
> retention of identity cues while embracing stylistic divergence, especially challenging for out-of-distribution
> individuals. We propose a training-free framework that generates stylized abstractions from a single image
> using inference-time scaling in vision-language models (VLLMs) to extract identity-relevant features, and a
> novel cross-domain rectified flow inversion strategy that reconstructs structure based on style-dependent
> priors. Our method adapts structural restoration dynamically through style-aware temporal scheduling, enabling
> high-fidelity reconstructions that honor both subject and style. It supports multi-round abstraction-aware
> generation without fine-tuning. To evaluate this task, we introduce StyleBench, a GPT-based human-aligned
> metric suited for abstract styles where pixel-level similarity fails. Experiments across diverse abstraction
> (e.g., LEGO, knitted dolls, South Park) show strong generalization to unseen identities and styles in a
> fully open-source setup.* </p>

## :rocket: News
- [05/28/2025] 🔥 We release <i>Training-Free Stylized Abstraction</i>.


## TODOs
- [ ] Release Code.
- [ ] Release HuggingFace Demo.

## Citation
If you find our work useful for your research, please consider citing us:

```bibtex
Coming Soon ...
```
## Contact
If you have any questions, please create an issue on this repository or contact at arahma30@jhu.edu and knaraya4@jhu.edu
