# Compositional Skills Overview

Taken from [What is a "Skill"](https://docs.instructlab.ai/taxonomy/skills/#:~:text=When%20you%20create%20a%20skill%20for%20the,types%20of%20compositional%20skills%2C%20freeform%20and%20grounded.&text=Core%20or%20foundational%20skills¶%20Core%20skills%20are%20foundational%20skills%20like%20math%2C%20reasoning%2C%20and%20coding.)

## Compositional Skills:
Skills are performative. When you create a skill for the model, you're teaching it how to do something such as "write me a song," "rearrange words in a sentence" or "summarize an email."

There are two types of compositional skills, freeform and grounded.

- **Freeform skills**: Tasks that require **open-ended responses**, like writing a song or summarizing an email. 

Freeform compositional skills are performative and do not require additional context. An example of a freeform skill is teaching the model words that rhyme. You could provide examples of "words that rhyme with 'tool'". By providing those examples, you're essentially using the latent knowledge of the LLM. In our example, you're enabling the LLM to be able to identify words that rhyme in its latent knowledge.

---

- **Grounded skills**: Tasks that require the model to answer **questions based on specific data or knowledge**. 

Grounded skills are performative and do require additional context. Examples of a grounded skill would be to read the value of a cell in a table layout or to parse a JSON file. To create a grounded skill to read a Markdown-formatted table layout, the additional context could be an example table layout. This additional context is including in the YAML for the skill and not external to it.









