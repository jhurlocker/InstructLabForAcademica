
# Multi-phase tuning framework


:bulb:InstructLab implements a multiphase training process to incrementally improve the model's performance whilst preserving previously learned. This phased approach helps maintain training stability and a replay buffer of the data prevents catastrophic forgetting, allowing the model to continuously learn and improve. 


Training happens in 2 phasees 
1. **Knowledge** - which is split into two steps:
    - Knowledge with short responses
    - knowledge with long responses

This phase integrates new factual information, divided into training on short responses followed by long responses and foundational skills

2. **Compositional Skills**
This phase enhances the model's ability to apply knowledge across various tasks and contexts for compositional skills

![Multiphase Tuning](graphics/multiphasetuning.png)

**:bulb:Replay buffers** are ued to replay training data from previous steps during the current training step **to avoid catastrophic forgetting**

---

### The framework uses small learning rates, extended warm-up periods and a large effective batch size for stability.

### Iterative improvement cycle

The synthetic data generation process is designed to be iterative. As new contributions are made to the taxonomy, they can be used to generate additional synthetic data, which further enhances the model. This continuous cycle of improvement helps make sure that the model remains up-to-date and relevant.


for more details [How InstructLab’s synthetic data generation enhances LLMs](https://www.redhat.com/en/blog/how-instructlabs-synthetic-data-generation-enhances-llms)
by [Cedric Clyburn](https://www.redhat.com/en/authors/cedric-clyburn), and [Legare Kerrison](https://www.redhat.com/en/authors/legare-kerrison)
