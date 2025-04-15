# Knowledge/Context Files


When generating Question and Answer pairs InstructLab uses your provided **PDF or Markdown** files as its source of truth.

The "reading" you give your model is the context file (containing the Knowledge) which should be a **Markdown or pdf file**. It is most effective if it uses a variety of paragraphs, tables, bullet points, and lists. The model learns best when it sees diverse formats, just like we do. 

If you are pulling this information from somewhere other than your brain, copy the original source verbatim for best results. Make sure to remove any links. 

Any code or preformatted text in the Markdown document should be enclosed in the corresponding Markdown block using backticks for the cli command or triple ‘ ‘ ‘ for multi-line formatted outputs or code blocks. 

Taken from ["Best Practices for InstructLab instruction datasets"](https://developers.redhat.com/articles/2024/11/21/best-practices-instructlab-instruction-datasets#)  by [Legare Kerrison](https://developers.redhat.com/author/legare-kerrison)

