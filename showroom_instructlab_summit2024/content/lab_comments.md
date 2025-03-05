# InstructLabForAcademica - Lab Tutorials - issues and comments
InstructLab workshop for Academia - Lab Tutorials - issues and comments

**3 Lab sections:**


1.  InstructLab RH catalog item - https://github.com/taylorjordanNC/showroom_instructlab_summit2024/blob/v19-updates-instructlab-classic/content/modules/ROOT/pages/index.adoc

2.  InstructLab UI - https://developer.ibm.com/tutorials/awb-contributing-llm-granite-instructlab-ui/?utm_source=ibm_developer&utm_content=in_content_link&utm_id=tutorials_awb-contributing-knowledge-instructlab-granite

3.  Getting Started with Podman AI Lab - https://developers.redhat.com/articles/2024/05/07/podman-ai-lab-getting-started#



### 1.  InstructLab RH catalog item lab ###

This is a good lab, and easy to follow and provides an excellent overview of InstructLab.  There were only a few issues to resolve.

**Issue 1 - ilab model download hugging face token**

A Hugging Face token needed when downloading models from this website and this must be added to the ilab model download command using `--hf-token` 

The instructor will need to talk students through creating a Hugging Face Token and copying that token so it can be used to run this part of the lab. 

*The command shown is:*
ilab model download --repository instructlab/granite-7b-lab-GGUF --filename=granite-7b-lab-Q4_K_M.gguf

*The command should be*
ilab model download --repository instructlab/granite-7b-lab-GGUF --filename granite-7b-lab-Q4_K_M.gguf --hf-token <your-huggingface-token>


**Issue 2 - typo**

In the section serving the new model
"Due to the time constraints of this lab, we will not actually be training the model! This would require a full-scale synthetic data generation process and a training run that could take many hours. You probably have **smoewhere** else you need to be, so we are going to show you the end results without making you wait"


**Issue 3 - Viewing the Synthetic Data is challenging** 

We may want to add a screen shot to the notes or make it so you can copy the text from the terminal window
When you are in the lab and try to view the synthetically generated data it is shown as one big long string; if we can cut and paste here then we can put the text into visual studio and format so it is readable. 


### 2.  InstructLab UI ###

The GUI lab is good to show how you create knowledge qna.yaml files, attribution.txt, and the md file.  This lab does involve a lot of typing and students have to think about the text they are entering - it would be easier to provide the input for them as part of this lab otherwise they are more focused on typing rather than concentrating on the lab. Here are the examples I used which we could made available in a text file for the students to cut and paste from. 

Seed Example 1
`IBM Granite is a series of decoder-only AI foundation models created by IBM. It was announced on September 7, and an initial paper was published 4 days later. `

Q&A Pair 1
`What is IBM Granite?`
`IBM Granite is a series of decoder-only AI foundation models created by IBM`

Q&A Pair 2
`When was IBM Granite announced`
`September 7, 2023`

Q&A Pair 3
`When was the first paper about Granite published `
`On September 11, 2023, four days after Granite was announced.`


Seed Example 2
`Granite's first foundation models were Granite.13b.instruct and Granite.13b.chat. The "13b" in their name comes from 13 billion, the amount of parameters they have as models, lesser than most of the larger models of the time. Later models vary from 3 to 34 billion parameters.`

Q&A Pair 1
`What was IBM's first foundation models?`
`IBM's first foundation model were Granite.13b.instruct and Granite.13b.chat.`

Q&A Pair 2
`What does the 13b stand for in the Granite name?`
`It stands for 13 billion, the amount of parameters the model has.`

Q&A Pair 3
`How many parameters do Granite models have today?`
`Today's Granite models have between 3 and 24 billion parameters.`




Seed Example 3
`On May 6, 2024, IBM released the source code of four variations of Granite Code Models under Apache 2, an open source permissive license that allows completely free use, modification and sharing of the software, and put them on Hugging Face for public use. According to IBM's own report, Granite 8b outperforms Llama 3 on several coding related tasks within similar range of parameters.`

Q&A Pair 1
`Are the IBM Granite LLMs free to use?`
`Yes, IBM has made their Granite Code Models available as open source`

Q&A Pair 2
`What type of licence does IBM Granite have?`
`IBM Granite has an open source permissive Apache 2 licence that means it is completely free to use.`

Q&A Pair 3
`Where can you get a copy of IBM Granite?`
`On Hugging Face`


Seed Example 4
`Granite vision model is a pre-trained model specialised on vision tasks for document and image understanding, supporting a range of file types and resolutions, and designed for efficient deployment in enterprise environments. It can be used by individuals or large corporates. `

Q&A Pair 1
`Does IBM Granite have a vision model?`
`Yes, IBM Granite has a vision model, called Granite vision model`

Q&A Pair 2
`What can the IBM Granite vision model do?`
`The IBM Granite model is trained on vision tasks for document and image understanding, supporting a range of file types and resolutions, and designed for efficient deployment in enterprise environments.`

Q&A Pair 3
`Is the IBM Granite vision model for use by individuals or organisations?`
`IBM Granite is designed for enterprise environments, but can be used by individuals or companies. `



Seed Example 5
`You can safeguard AI with Granite Guardian, ensuring enterprise data security and mitigating risks across a variety of user prompts and LLM responses, with top performance in 15+ safety benchmarks.`

Q&A Pair 1
`What is Granite Guardian?`
`Granite Guardian safeguards your user prompts and LLM responses ensuring enterprise data security and mitigating risks`

Q&A Pair 2
`How many safety benchmarks has IBM Granite been rated in `
`15+`

Q&A Pair 3
`What is the name of IBM Granites safeguarding capability?`
`Granite Guardian`



I think once we have got the students to create the qna.yaml files which they download and view in Visual Studio we then end this lab as they will have already gone through SDG in the first lab. 


*The only minor issue is the labs are on two different topics - which hopefully is not confusing*



### 3. Getting Started with PodMan AI Lab ###