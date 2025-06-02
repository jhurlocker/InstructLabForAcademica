# Step 1 - Collate Knowledge files

# Step 2 - Create seed data in the Knowledge qna.yaml file format

Below is an illustration of the information that goes into the qna.yaml file

---

 **`version`**: The version of the qna.yaml file, this is the format of the file used for SDG. The value must be the number 3. \
 **`created_by`**: Your GitHub username. \
 **`domain`**: Specify the category of the knowledge. \
 **`seed_examples`**: :bulb: A collection of key/value entries (**you must have at least 5**) \
     **`context`**: A chunk of information from the knowledge document. Each qna.yaml needs five context blocks and has a maximum word count of 500 words. \
     **`questions_and_answers`**: The parameter that holds your questions and answers (**for each context there should be 3 q&a examples**) \
         **`question`**: Specify a question for the model. Each qna.yaml file needs at least three question and answer pairs per context chunk with a maximum word count of 250 words. \
         **`answer`**: Specify the desired answer from the model. Each qna.yaml file needs at least three question and answer pairs per context chunk with a maximum word count of 250 words. \
 **`document_outline`**: Describe an overview of the document your submitting. \
 **`document`**: The source of your knowledge contribution. \
 **`repo`**: The URL to your repository that holds your knowledge markdown files. \
 **`commit`**: The SHA (hash) of the commit in your repository with your knowledge markdown files. \
 **`patterns`**: A list of glob patterns specifying the markdown files in your repository. Any glob pattern that starts with *, such as *.md, must be quoted due to YAML rules. For example, *.md. \

---

    # :bulb: Other requirements

   
There is a minimum requirement to have 5 'context' - which will have an associated minimum of 3 'questions and answer' pairs.  The 'question and answer' pairs must relate to the context. 