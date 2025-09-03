
# InstructLab results and significance 

The significance of InstructLab lies in its ability to achieve state-of-the-art performance using publicly available teacher models instead of relying on proprietary models. In [benchmarks](https://arxiv.org/pdf/2403.01081), the InstructLab methodology has shown promising results. For example, when applied to Llama-2-13b (resulting in [Labradorite-13b](https://huggingface.co/ibm/labradorite-13b)) and Mistral-7B (resulting in [Merlinite-7B](https://huggingface.co/ibm/merlinite-7b)), the LAB-trained models outperformed current best models fine-tuned on their respective base models in terms of [MT-Bench](https://klu.ai/glossary/mt-bench-eval) scores. They also maintained strong performance across other metrics, including [MMLU](https://en.wikipedia.org/wiki/MMLU) (testing multitask language understanding), [ARC](https://github.com/fchollet/ARC-AGI) (evaluating reasoning capabilities) and [HellaSwag](https://rowanzellers.com/hellaswag/) (assessing common sense inference), among others.

*:bulb:The bottom-line is that InstructLab provides a cost effective, community-driven solution for improving the alignment of Language Models.*

## Areas where InstructLab excels are

for more details [How InstructLab’s synthetic data generation enhances LLMs](https://www.redhat.com/en/blog/how-instructlabs-synthetic-data-generation-enhances-llms)
by [Cedric Clyburn](https://www.redhat.com/en/authors/cedric-clyburn), and [Legare Kerrison](https://www.redhat.com/en/authors/legare-kerrison)

# Comparing InstructLab to Fine Tuning

There is not much written on the direct comparisson, however the following article does provide a great insight and comparison between InstructLab and Fine Tuning. 

[How IBM’s InstructLab Differs from Traditional Fine-Tuning](https://medium.com/@luke.major/how-ibms-instructlab-differs-from-traditional-fine-tuning-8eaa38b643a5) by [Luke Major](https://medium.com/@luke.major?source=post_page---byline--8eaa38b643a5---------------------------------------) in collaboration with [Manav Gupta](https://medium.com/u/40b408c51fd3?source=post_page---user_mention--8eaa38b643a5---------------------------------------).

[Luke Major](https://medium.com/@luke.major?source=post_page---byline--8eaa38b643a5---------------------------------------) and [Manav Gupta](https://medium.com/u/40b408c51fd3?source=post_page---user_mention--8eaa38b643a5---------------------------------------) provide a great comparison of the two approaches.

"To summarize, consider the analogy of someone with a high-quality suit who wants to add some flair to it through custom designs. Traditional fine-tuning is like buying a sewing machine, thread, needles, fabrics, and doing the alterations and customizations yourself. If done correctly, this will produce the best result as you know exactly what you are looking to be done, with the vision coming directly from your mind to your hands. However, most people won’t be able to achieve this and will produce a subpar result. Using InstructLab is akin to sending the suit to a tailor. Since the tailor can’t read your mind he must interpret what your desires are based on your instructions, however, in the vast majority of cases, you will be left with an excellent result."