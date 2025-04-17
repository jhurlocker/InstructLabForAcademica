# Example of a Compositional Skills qna file

Link to [The skills files](https://docs.instructlab.ai/taxonomy/skills/file_structure/#__tabbed_4_1)

## Ungrounded compositional skill: YAML example

version: 2 \
task_description: 'Teach the model how to rhyme.' \
created_by: juliadenham \
seed_examples: \
 &nbsp;&nbsp; question: What are 5 words that rhyme with horn? \
 &nbsp;&nbsp; answer: warn, torn, born, thorn, and corn. \
 &nbsp;&nbsp; question: What are 5 words that rhyme with cat? \
 &nbsp;&nbsp; answer: bat, gnat, rat, vat, and mat. \
 &nbsp;&nbsp; question: What are 5 words that rhyme with poor? \
 &nbsp;&nbsp; answer: door, shore, core, bore, and tore. \
 &nbsp;&nbsp; question: What are 5 words that rhyme with bank? \
 &nbsp;&nbsp; answer: tank, rank, prank, sank, and drank. \
 &nbsp;&nbsp; question: What are 5 words that rhyme with bake? \
 &nbsp;&nbsp; answer: wake, lake, steak, make, and quake. \

---

## Grounded compositional skill: YAML example

version: 2 \
task_description:This skill provides the ability to read a markdown-formatted table. \
created_by: mairin # Use your GitHub username; only one creator supported \
seed_examples: \
context: \
 &nbsp; &nbsp;  | **Breed** &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | **Size** &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  &nbsp;      | **Barking** &nbsp; &nbsp;  | **Energy** &nbsp; &nbsp; &nbsp;  | \
 &nbsp; &nbsp;  |---------------|--------------|------------|------------| \
  &nbsp; &nbsp; | Afghan Hound | 25-27 in  &nbsp; &nbsp; &nbsp; &nbsp;  | 3/5   &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;| 4/5   &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | \
 &nbsp; &nbsp;  | Labrador &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  | 22.5-24.5 in | 3/5&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;&nbsp; &nbsp; &nbsp;  | 5/5 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  | \
  &nbsp; &nbsp; | Cocker Spaniel  | 14.5-15.5 in &nbsp;  | 3/5 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | 4/5 &nbsp; &nbsp;  &nbsp; &nbsp; &nbsp; | \
 &nbsp; &nbsp;  | Poodle (Toy) &nbsp; &nbsp;  | <= 10 in&nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | 4/5 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | 4/5 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | \
    question: \
  &nbsp; &nbsp;     Which breed has the most energy?\
    answer: \
 &nbsp; &nbsp;      The breed with the most energy is the Labrador. \
  context:  \
     &nbsp;&nbsp;| **Name** &nbsp; &nbsp;&nbsp; | **Date** &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| **Color** &nbsp;&nbsp;&nbsp;&nbsp;| **Letter**&nbsp;&nbsp;&nbsp;&nbsp; | **Number**&nbsp;&nbsp;&nbsp; | \
     &nbsp;&nbsp; |----------|---------|----------|----------|-----------| \
     &nbsp;&nbsp; | George&nbsp; &nbsp;| Mar 5 &nbsp;&nbsp;&nbsp; &nbsp;| Green &nbsp;&nbsp; &nbsp;| A &nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| 1 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| \
     &nbsp;&nbsp; | Gráinne&nbsp;&nbsp;| Dec 31&nbsp;&nbsp;&nbsp;&nbsp;| Red&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| B &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp; &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| 2 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| \
     &nbsp;&nbsp; | Abigail&nbsp;&nbsp;&nbsp;| Jan 17 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Yellow &nbsp;&nbsp;&nbsp;&nbsp;| C &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| 3 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| \
     &nbsp;&nbsp; | Bhavna&nbsp;&nbsp;| Apr 29&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Purple&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| D &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| 4 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| \
     &nbsp;&nbsp; | Rémy &nbsp;&nbsp;&nbsp;&nbsp;| Sep 9 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Blue &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| E &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| 5 &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| \
    question: \
     &nbsp;&nbsp; What is Gráinne's letter and what is her color? \
    answer: \
     &nbsp;&nbsp; Gráinne's letter is B and her color is red. \
  context:  \
     &nbsp;&nbsp; | Banana&nbsp; | Apple &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Blueberry&nbsp; | Strawberry | \
     &nbsp;&nbsp; |---------|------------|-----------|------------| \
     &nbsp;&nbsp; | Yellow &nbsp;&nbsp;| Red, Green | Blue &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Red &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| \
     &nbsp;&nbsp; | Large &nbsp; &nbsp;| Medium&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Small &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| Small &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| \
     &nbsp;&nbsp; | Peel &nbsp;&nbsp; &nbsp;&nbsp; | Peel &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| No peel&nbsp;&nbsp;&nbsp;| No peel &nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;&nbsp;| \
    question:  \
   &nbsp;&nbsp;   Which fruit is blue, small, and has no peel? \
    answer:  \
    &nbsp;&nbsp;  The blueberry is blue, small, and has no peel. 
