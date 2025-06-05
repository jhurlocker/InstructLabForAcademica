# Hints and tips for tuning:

:bulb:Only a few Question-and-Answer (Q&A)seed pairs are required, thse will be amplified to create many (100's to 100,000s) of Question-and-Answer pairs for tuning during the Synthetic Data Generation (SDG) process.

Always think carefully about the seed Q&A files that you add as these are examples that the model will use to base it SDG on. 

# Reminder of the files that are required

**qna.yaml file**
- **Knowledge** required a minimum of 5 contexts each context must have 3 Q&A Examples 
- **Ungrounded Skills** require a minimum of 5 Q&A pairs 
- **Grounded Skills** require a minimum of 5 contexts each context must have 1 Q&A examples 

**Knowledge files** when adding knowledge, these are either pdf or markdown files \
**Attribution file** provides the providence information for the knowledge or skill you are adding. 

Best practice details for qna.yaml files is available on [Github.com](https://github.com/instructlab/docs.instructlab.ai/pull/3/files)





