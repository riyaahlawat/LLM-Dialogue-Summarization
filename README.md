# LLM-Dialogue-Summarization

This repository focuses on enhancing the dialogue summarization capabilities of the FLAN-T5 model. The project is divided into three tasks, each aimed at improving the performance, efficiency, and safety of the summaries generated:

1. **Dialogue Summarization using Original FLAN-T5**: Establishing a baseline by using the pre-trained FLAN-T5 model for dialogue summarization.
2. **Fine-Tuning vs PEFT (LoRA) for Dialogue Summarization**: Reducing computational overhead while improving summarization performance by comparing standard fine-tuning with Parameter-Efficient Fine-Tuning (PEFT) using LoRA.
3. **RLHF (PPO) for Reducing Toxicity in Summaries**: Applying Reinforcement Learning with Human Feedback (RLHF) using Proximal Policy Optimization (PPO) to reduce the toxicity of the generated summaries.

## Evaluation Metrics

To ensure the generated summaries are both high-quality and aligned with desired ethical standards, we utilize the following evaluation metrics:

- **ROUGE (Recall-Oriented Understudy for Gisting Evaluation)**: This metric is commonly used for evaluating automatic summarization. It compares the overlap between the generated summary and reference summaries by measuring precision, recall, and F1-score across n-grams (usually unigrams, bigrams, and longest common subsequence). ROUGE helps us assess how well our model captures the essential content of the dialogues.

- **Toxicity Score**: To gauge the ethical quality of the summaries, we calculate a toxicity score using tools like the Perspective API. This score helps us determine the extent to which the generated text contains harmful or offensive language. By focusing on reducing the toxicity score, we aim to produce summaries that are safe, inclusive, and positive.

These metrics are crucial for evaluating the improvements introduced through PEFT with LoRA and RLHF with PPO, as they allow us to quantify not only the accuracy but also the ethical impact of the summaries produced by the model.

So, this version reflects our approach to improving dialogue summarization by enhancing performance, reducing compute, and minimizing toxicity.


