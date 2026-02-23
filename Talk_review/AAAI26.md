# Talk : IAAI Invited Talk: Agentic AI at Enterprise Scale: Three Production Cases from Automotive
by Bryan Goodman (Executive Director of AI @ Ford) 

## Learning from building multi-agent systems 
### 1. Multi-Agents works at scale 
   It matters that breaking down the problem into specialized agents, really was important here. So we have agents that work on discovery, some that work on generating the queries, and so on.

### 2. Hybrid Search Outperforms than single method approach 
Combining search here. So, semantic search with vector database, works very well in some cases, but in other cases, when we need, just keyword search is exactly what's needed. High precision, that,
a plain old text-based keyword search was very good. So, by combining the two, we got even better results. 

### 3. Memory System Enables Personalization
Having a memory system was very important. 
We found that users didn't just go in and ask one question, they're often interacting over longer periods of time with this system, and they're asking related questions, 
and so we were able to reduce clarifying questions from users by 40% by implementing a robust memory system into this agent system.

### 4. Comprehensive Evaluation Framework is critical 
Having an evaluation framework up front. So again, this is like test-driven development. Really important. 
Having those robust evaluations, we would just not have been able to do this without building those evaluations up front, and then continually billing on them and adding to them.
And allowed us to find a lot of things early on, and even just enabled solving a lot of things that would not have been possible without it. 
Evaluations, within an agentic system and testing of the agentic systems were fairly difficult.

### 5. Evaluation and Testing of LLM Agents is extremely complex  
Evaluations, within an agentic system and testing of the agentic systems were fairly difficult.
Because, of course, they're non-deterministic and can take many complex paths, sometimes to the same solution, that made doing traditional testing, of course, very difficult, and so having an ability to trace through and robust evaluations that were

### 6. Debugging Agent Behavior is extremely challenging 
Because, of course, they're non-deterministic and can take many complex paths, sometimes to the same solution, that made doing traditional testing, of course, very difficult, and so having an ability to trace through and robust evaluations that were
Often using AI as the evaluator, or AI as the judge.
enabled them to be more flexible evaluations. And then related to that was, having this very complex system made debugging very hard. So, again, having the ability to trace through, was, was really important. And, because
We often had non-reproducible errors.
So, being able to step through, much like a debugger, was critical.

### 7. Agent Coordination and Hands-off require careful design
handing off between different agents was something that we had to make very robust, and also a lot of our testing and evaluation involved checking for the handoffs between different tools and different sub-agents.
If one tool is expecting a certain level of input, and the other tool asking it is not always

### 8. Country Filtering & Access Control Adds Significant Complexity
maintaining data security was very important. Not everyone in the company has access to all of the data, and so these tools had to respect that and act on behalf of the user, but with the user's permissions, and enforce those as well, 
so that building in that security Was required.

### 9.Metadata quality directly impacts agent performance 
 I already talked a bit about the importance of the metadata. Having high-quality metadata was, was really the key here, the secret.

### 10. Prompt Engineering is critical and requires constant iteration
prompt engineering was, I call it really important, and a good example of that was the word important. So, putting in all caps the word important in the prompt, increased, or actually, increased compliance by over 30%. So, we did an awful lot of, prompt engineering throughout, the work on all of these agents, and, 

### 11. Performance vs. Accuracy trade off are constant
I think this is my last learning, and that's the trade-off between speed and accuracy. Because we found that, of course, people always require a certain level of accuracy and want as accurate as possible.
But they're also impatient. And so, oftentimes we had a trade-off between, speed and accuracy, and had things like a thinking budget.
And so we found some parts we could have a very small thinking budget. It didn't matter. We could reduce the thinking budget and get much faster responses, where in other times, we needed to increase the thinking budget to make sure we were getting very high
Accuracy in the results, and then really balance between the two.
And in some cases, even try a fast path, and then see if that worked, and if not, then fall back to a slower path.
