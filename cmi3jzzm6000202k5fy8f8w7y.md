---
title: "Ephemeral Learning"
datePublished: Mon Nov 17 2025 19:44:42 GMT+0000 (Coordinated Universal Time)
cuid: cmi3jzzm6000202k5fy8f8w7y
slug: ephemeral-learning
cover: https://raw.githubusercontent.com/ricardotrevisan/ricardotrevisan.github.io/master/images/image_1_20251014.png
tags: ephemerallearning, incontextai, adaptiveintelligence

---

Language models are revealing something fascinating: they can learn from the prompt itself. The study “Learning without training” (Google Research, 2025) shows that context-generated attention acts as a local gradient generator, dynamically adjusting the MLP weights — without backpropagation.

If confirmed at scale, this idea could transform the AI lifecycle: instead of retraining entire models (📉), they could learn in-context, store what counts as “useful memory,” and consolidate into real training only what proves functional over time — just as the brain turns working memory into durable learning. This enables low-cost adaptation to new regulatory environments, specific corporate communication styles, and dynamic conditions for risk analysis and decision-making — in addition to paving the way for continuous, streamlined learning.

Technically, the paper shows that the Transformer creates a temporary network tailored to the current prompt. This learning is ephemeral and task-specific, but powerful: the model adapts in real time, generalizes, and solves tasks without retraining. Well-designed prompts become a form of in-context updating, enabling adjustments to behavior, language, and even analytical strategies in seconds.

Learning from context could become as important as formal training — paving the way for self-improving models and truly adaptive AI.

#EphemeralLearning  #InContextAI #AdaptiveIntelligence

📚 **Sources:**

• Google Research - Learning without training: https://arxiv.org/html/2507.16003v1
• Ricardo Trevisan - In Context Learning Simulation: https://github.com/ricardotrevisan/incontext-learning