---
permalink: /
title: "About Me"
excerpt: "Research Scientist/Engineer at Adobe Photoshop. LLM and VLM reasoning, reasoning-based image editing, and an interest in AI safety and control."
author_profile: true
redirect_from: 
  - /about/
  - /about.html
---

I am a Research Scientist/Engineer on the Applied Research team at [Adobe Photoshop](https://www.adobe.com/products/photoshop.html). I work on language and vision-language models that reason carefully, and on turning that reasoning into precise image edits.

I received my Ph.D. in Computer Engineering from [Northeastern University](https://www.northeastern.edu/), advised by Prof. [Yun Raymond Fu](http://www1.ece.neu.edu/~yunfu/).

I want AI that stays under human control. Agents should not leave the sandbox they are given, and their goals should stay aligned with human values, so they do not harm or threaten people because the objective was specified wrong.

---

## Research

<div class="research-card">
  <div class="research-card__icon" aria-hidden="true"><i class="fas fa-brain"></i></div>
  <div>
    <h3>LLM and VLM reasoning</h3>
    <p>How multimodal models plan, keep a working context, and ground intermediate steps in the image. On the language side, how decoding should change when the model is unsure of the next token.</p>
    <p class="research-links">
      <a class="link-chip" href="https://arxiv.org/pdf/2501.19201"><i class="fas fa-file-pdf" aria-hidden="true"></i> Efficient Reasoning with Hidden Thinking</a>
      <a class="link-chip" href="https://www.arxiv.org/pdf/2507.03038"><i class="fas fa-file-pdf" aria-hidden="true"></i> Cautious Next Token Prediction</a>
      <a class="link-chip" href="https://arxiv.org/pdf/2605.04304"><i class="fas fa-file-pdf" aria-hidden="true"></i> Hierarchical Visual Agent</a>
      <a class="link-chip" href="https://arxiv.org/pdf/2312.02310.pdf"><i class="fas fa-file-pdf" aria-hidden="true"></i> VaQuitA</a>
      <a class="link-chip" href="https://openreview.net/forum?id=4r3zsJBBla"><i class="fas fa-file-pdf" aria-hidden="true"></i> Multimodal Generative Composition Recommendation</a>
    </p>
  </div>
</div>

<div class="research-card">
  <div class="research-card__icon" aria-hidden="true"><i class="fas fa-image"></i></div>
  <div>
    <h3>Reasoning-based Visual Understanding and Editing</h3>
    <p>Instruction-guided editing should understand an object and the effects it causes, not only the pixels of the object. That line of work shipped in Photoshop as Remove objects and related elements.</p>
    <p class="research-links">
      <a class="link-chip" href="https://helpx.adobe.com/photoshop/desktop/repair-retouch/remove-objects-fill-space/remove-related-elements.html"><i class="fas fa-bullhorn" aria-hidden="true"></i> Remove Tool of Photoshop</a>
      <a class="link-chip" href="https://aclanthology.org/2026.acl-long.2155.pdf"><i class="fas fa-file-pdf" aria-hidden="true"></i> LLMs for visual segmentation</a>
      <a class="link-chip" href="https://arxiv.org/pdf/2511.14183"><i class="fas fa-file-pdf" aria-hidden="true"></i> UniSER</a>
    </p>
  </div>
</div>

---

## What I want to work on next

<div class="research-card">
  <div class="research-card__icon" aria-hidden="true"><i class="fas fa-shield-alt"></i></div>
  <div>
    <h3>AI safety and control</h3>
    <p>The problem I want to work on is control. Advanced agents should remain inside the limits people set, including the sandbox they run in, and should not break out of human oversight. In the longer term, that means stopping agents from harming or threatening people when their goals drift from human values.</p>
    <p>The closest I have come so far is <a href="https://arxiv.org/pdf/2501.19201">Efficient Reasoning with Hidden Thinking</a>. It compresses chain-of-thought into a few hidden thinking tokens and uses an interpreter to map them back to text. Whether reasoning that happens in latent space can still be read and overseen is the question I want to take further.</p>
    <p class="research-links">
      Related papers I contributed to:<br>
      <a class="link-chip" href="https://ref-adv.github.io/"><i class="fas fa-file-pdf" aria-hidden="true"></i> Ref-Adv: reasoning shortcuts in MLLMs</a>
      <a class="link-chip" href="https://arxiv.org/pdf/2604.12944"><i class="fas fa-file-pdf" aria-hidden="true"></i> Hallucination in video LLMs</a>
      <a class="link-chip" href="https://arxiv.org/pdf/2406.13763"><i class="fas fa-file-pdf" aria-hidden="true"></i> Theory of mind in video LLMs</a>
    </p>
  </div>
</div>

---

## Tech transfer

<div class="experience-item">
  <h3>Remove objects and related elements</h3>
  <p class="experience-meta"><strong>Adobe Photoshop</strong> &nbsp;|&nbsp; 2026</p>
  <p>
    First research-to-product transfer. Remove an object, and the model also clears its shadows, reflections, and other related elements in one step.
    <a class="link-chip" href="https://helpx.adobe.com/photoshop/desktop/repair-retouch/remove-objects-fill-space/remove-related-elements.html"><i class="fas fa-book" aria-hidden="true"></i> Adobe Help page</a>
    <a class="link-chip" href="https://www.youtube.com/watch?v=NmgOcJXcHt8&amp;t=772s"><i class="fab fa-youtube" aria-hidden="true"></i> Feature walkthrough</a>
  </p>
</div>

---

## Selected publications

Five first-author papers, and the second-author paper closest to where I want to go next. The full list is on the [Publications](/publications/) page.

- **Cautious Next Token Prediction**<br>
  *ACL 2025* · First author, from my Adobe Photoshop internship<br>
  A training-free decoding strategy. When prediction entropy is high, the model samples several continuations and keeps the one with the lowest perplexity.<br>
  [[Paper](https://www.arxiv.org/pdf/2507.03038)] [[Code](https://github.com/wyzjack/CNTP)]

- **Efficient Reasoning with Hidden Thinking**<br>
  *ICML 2026* · Second author<br>
  Compresses chain-of-thought in multimodal LLMs into a few thinking tokens, with an interpreter that reconstructs the reasoning as text.<br>
  [[Paper](https://arxiv.org/pdf/2501.19201)] [[Code](https://github.com/shawnricecake/Heima)]

- **From Words to Pixels: A Comprehensive Survey on Large Language Models in Visual Segmentation**<br>
  *ACL 2026* · First author<br>
  A survey of how large language models are used for visual segmentation.<br>
  [[Paper](https://aclanthology.org/2026.acl-long.2155.pdf)] [[Code](https://github.com/wyzjack/Awesome-LLM-Visual-Segmentation)]

- **Multimodal Generative Composition Recommendation**<br>
  *ICLR 2026 rejected* · First author, from my Adobe Photoshop internship<br>
  Fine-tunes multimodal LLMs to recommend what object to add to an image and where to place and scale it, trained on data generated automatically from stock images.<br>
  [[Paper](https://openreview.net/forum?id=4r3zsJBBla)]

- **VaQuitA: Enhancing Alignment in LLM-Assisted Video Understanding**<br>
  *Preprint* · First author, from my Adobe Research internship<br>
  Video question answering with an LLM, using CLIP-score-guided frame sampling and a Visual-Query Transformer that conditions the video features on the question.<br>
  [[Paper](https://arxiv.org/pdf/2312.02310.pdf)]

- **Towards Zero-shot 3D Anomaly Localization**<br>
  *WACV 2025 (Oral)* · First author, from my MERL internship<br>
  Defines zero-shot 3D anomaly detection and localization, where training and test classes do not overlap, and proposes a patch-level contrastive method for it.<br>
  [[Paper](https://arxiv.org/pdf/2412.04304)] [[Project](https://wyzjack.github.io/3DzAL/)] [[Video](https://youtu.be/GAoRO-hOvuw)]

---

## Education

<div class="education-item">
  <strong><i class="fas fa-graduation-cap" aria-hidden="true"></i> Northeastern University (NEU)</strong> &nbsp;|&nbsp; 2020 - 2026<br>
  <em>Ph.D. in Computer Engineering</em><br>
  Supervisor: Prof. <a href="http://www1.ece.neu.edu/~yunfu/">Yun Raymond Fu</a>
</div>

<div class="education-item">
  <strong><i class="fas fa-graduation-cap" aria-hidden="true"></i> Northeastern University (NEU)</strong> &nbsp;|&nbsp; 2020 - 2023<br>
  <em>M.S. in Electrical Engineering</em><br>
  Concentration: Computer Vision, Machine Learning & Algorithms
</div>

<div class="education-item">
  <strong><i class="fas fa-university" aria-hidden="true"></i> Xi'an Jiaotong University (XJTU)</strong> &nbsp;|&nbsp; 2016 - 2020<br>
  <em>B.S. in <a href="http://bjb.xjtu.edu.cn/info/1071/2192.htm">Mathematics and Applied Mathematics (National Honors Program)</a></em>
</div>

---

## Contact

<p><i class="fas fa-envelope" aria-hidden="true"></i> <strong>Email:</strong> wyzjack990122 (at) gmail (dot) com</p>
