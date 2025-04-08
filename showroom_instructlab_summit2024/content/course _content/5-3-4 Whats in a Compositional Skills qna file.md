#Skills Overview


Link to [The skills files](https://docs.instructlab.ai/taxonomy/skills/file_structure/#__tabbed_4_1)

| Field | Type | Required | Constraints|
|------|-----|------|-----|
| version | integer | yes | - |
| task_description| string | yes |  |
| created_by| string | yes |   |
| seed example | array | yes | at least 5 sets|
| context | string | only for grounded skills | max 500 tokens|
| question | string | yes | max 250 tokens |
| answer | string | yes | max 250 tokens |
