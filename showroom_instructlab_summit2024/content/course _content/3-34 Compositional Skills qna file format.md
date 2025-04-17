# Skills qna.yaml file format

The chart illustrates the type of data that is required in the qna.yaml file. 


Link to [The skills files](https://docs.instructlab.ai/taxonomy/skills/file_structure/#__tabbed_4_1)

| Field | Type | Required | Constraints|
|------|-----|------|-----|
| version | integer | yes | - |
| task_description| string | yes |  |
| created_by| string | yes |   |
| seed example | array | yes | :bulb:at least 5 sets|
| context | string | only for grounded skills | each context requires 3 sets of Q&A - max 500 tokens|
| question | string | yes | max 250 tokens |
| answer | string | yes | max 250 tokens |
