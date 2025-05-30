# Skills qna.yaml file format

The chart illustrates the type of data that is required in the qna.yaml file. 


Link to [more details on Skills in InstructLab documentation](https://docs.instructlab.ai/taxonomy/skills/file_structure/#__tabbed_4_1)

    qna.yaml
    
    1   version: # ...
    2   task_description: # ...
    3   created_by: # ...
    4   seed_examples:
    5     - question: # ...
    6       answer: # ...
    7     - question: # ...
    8       answer: # ...
    9     - question: # ...
    10      answer: # ...
    11    - question: # ...
    12      answer: # ...
    13    - question: # ...
    14      answer: # ...

    version: 2
       
    task_description: 'Teach the model how to rhyme.' 
    created_by: juliadenham 
    seed_examples: 
    -  question: What are 5 words that rhyme with horn? 
        answer: warn, torn, born, thorn, and corn. 
    -  question: What are 5 words that rhyme with cat? 
        answer: bat, gnat, rat, vat, and mat. 
    -  question: What are 5 words that rhyme with poor? 
       answer: door, shore, core, bore, and tore. 
    -  question: What are 5 words that rhyme with bank? 
       answer: tank, rank, prank, sank, and drank. 
    -  question: What are 5 words that rhyme with bake? 
       answer: wake, lake, steak, make, and quake. 


| Field | Type | Required | Constraints|
|------|-----|------|-----|
| version | integer | yes | - |
| task_description| string | yes |  |
| created_by| string | yes |   |
| seed example | array | yes | :bulb:at least 5 sets|
| context | string | only for grounded skills | each context requires 3 sets of Q&A - max 500 tokens|
| question | string | yes | max 250 tokens |
| answer | string | yes | max 250 tokens |
