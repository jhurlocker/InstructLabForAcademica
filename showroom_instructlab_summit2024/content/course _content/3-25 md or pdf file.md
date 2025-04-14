# Knowledge/Context Files


When generating Question and Answer pairs InstructLab uses your provided **PDF or Markdown** files as its source of truth.

The "reading" you give your model is the context file (containing the Knowledge) which should be a **Markdown or pdf file**. It is most effective if it uses a variety of paragraphs, tables, bullet points, and lists. The model learns best when it sees diverse formats, just like we do. 

If you are pulling this information from somewhere other than your brain, copy the original source verbatim for best results. Make sure to remove any links. 

Any code or preformatted text in the Markdown document should be enclosed in the corresponding Markdown block using backticks for the cli command or triple ‘ ‘ ‘ for multi-line formatted outputs or code blocks. 

Taken from ["Best Practices for InstructLab instruction datasets"](https://developers.redhat.com/articles/2024/11/21/best-practices-instructlab-instruction-datasets#)  by [Legare Kerrison](https://developers.redhat.com/author/legare-kerrison)


## Contributing skills and knowledge

[for more details follow this link](https://github.com/instructlab/taxonomy/blob/main/CONTRIBUTING.md#ways-of-contributing-to-the-taxonomy-repository)

You can contribute to the taxonomy in the following two ways:

**Adding new examples to existing leaf nodes:**

Go to the corresponding leaf node / end of the branch and modify the YAML
Add a new example to the qna.yaml files as a new entry to the list

**Adding new branches/skills corresponding to the existing domain:**

You can add new folders under the corresponding category (replace any spaces with underscores _)
Create a new qna.yaml file containing examples for the new skill
