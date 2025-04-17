# Example of a Compositional Skills qna file

Link to [The skills files](https://docs.instructlab.ai/taxonomy/skills/file_structure/#__tabbed_4_1)

## Ungrounded compositional skill: YAML example

version: 2 \
task_description: 'Teach the model how to rhyme.' \
created_by: juliadenham \
seed_examples: \
  question: What are 5 words that rhyme with horn? \
  answer: warn, torn, born, thorn, and corn. \
  question: What are 5 words that rhyme with cat? \
  answer: bat, gnat, rat, vat, and mat. \
  question: What are 5 words that rhyme with poor? \
  answer: door, shore, core, bore, and tore. \
  question: What are 5 words that rhyme with bank? \
  answer: tank, rank, prank, sank, and drank. \
  question: What are 5 words that rhyme with bake? \
  answer: wake, lake, steak, make, and quake. \

---

## Grounded compositional skill: YAML example

version: 2 \
task_description:This skill provides the ability to read a markdown-formatted table. \
created_by: mairin # Use your GitHub username; only one creator supported \
seed_examples: \
context: \
  | **Breed** &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | **Size** &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;      | **Barking** &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | **Energy** &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | \
  |----------------|--------------|-------------|------------| \
  | Afghan Hound &nbsp; | 25-27 in  &nbsp; &nbsp; &nbsp; | 3/5   &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;       | 4/5   &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;      | \
  | Labrador &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  | 22.5-24.5 in &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  | 3/5&nbsp; &nbsp; &nbsp; &nbsp; &nbsp;     | 5/5 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | \
  | Cocker Spaniel  | 14.5-15.5 in &nbsp; &nbsp; &nbsp; &nbsp;  | 3/5 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  | 4/5 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp;  | \
  | Poodle (Toy) &nbsp; &nbsp;  | <= 10 in&nbsp; &nbsp; &nbsp; | 4/5 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | 4/5 &nbsp; &nbsp; &nbsp; &nbsp; &nbsp; | \
    question: \
      Which breed has the most energy?\
    answer: \
      The breed with the most energy is the Labrador. \
  context:  \
      | **Name** | **Date** | **Color** | **Letter** | **Number** |
      |----------|----------|-----------|------------|------------|
      | George   | Mar 5    | Green     | A          | 1          |
      | Gráinne  | Dec 31   | Red       | B          | 2          |
      | Abigail  | Jan 17   | Yellow    | C          | 3          |
      | Bhavna   | Apr 29   | Purple    | D          | 4          |
      | Rémy     | Sep 9    | Blue      | E          | 5          |
    question: \
      What is Gráinne's letter and what is her color? \
    answer: \
      Gráinne's letter is B and her color is red. \
  context:  \
      | Banana | Apple      | Blueberry | Strawberry |
      |--------|------------|-----------|------------|
      | Yellow | Red, Green | Blue      | Red        |
      | Large  | Medium     | Small     | Small      |
      | Peel   | Peel       | No peel   | No peel    |
    question:  \
      Which fruit is blue, small, and has no peel? \
    answer:  \
      The blueberry is blue, small, and has no peel. \
