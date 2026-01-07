### Title 

Reducing Tool Hallucination via Reliability Alignment 

### Summary
- Tool Hallucination is either inappropriate tool selection or misuse tool
- Tool Hallucination leads to errorneous task execution, increase computation cost, reduced system reliability
- This paper suggest novel metric to access task success and efficiency 
- This paper systematically define and categorize tool hallucination.  
- Tool type hallucination, content hallucination occur more frequently 

- Limitation and challenges in terms of Tool utilization 
(in terms of Tool Selection) 
 Tool type hallucination - Fabricated Tool name, Irrelevant Tool
 Timing Hallucination - Duplicated Tool calling   

(in terms of Tool using) 
Format Hallucination
Content Hallucination 

(Evaluation process of Tool hallucination) 
Rule based checking
LLM based checking 

- Adding more training data doesn't help to reduce the hallucination

- Having bigger model helps for better performance and hallucination reduction 

- To mitigate the hallucination: 
	1. improve pre-training data
	2. Fine-Tuning with curated dataset
	3. Designing better decoding strategy and estimating uncertainty 


### Terminology to learn 

1. in-context learning

2. Stable Tool Bench

3. DPO (Direct Preference Optimization) Algorithm 
