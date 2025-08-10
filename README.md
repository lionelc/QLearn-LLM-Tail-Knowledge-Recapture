# QLearn-LLM-Tail-Knowledge-Recapture
This is the code repo for the work done for paper "RL-Assisted Agentic Retrieval and Verification for Tail Knowledge Recapture from LLMs".

**(to be updated after the release of the paper)**

To address some questions on its methodology and choice of specific techniques:

1. **Q:** Agentic information retrieval, including agents using reinforcement learning, is the recent trend. Why do you apply this approach on "tail knowledge recapture from LLMs"?
A: Information retrieval is a broad area, and we consider how to apply reinforcement learning may not be a "one-size-fit-all" scenario. So, the narrower field of "tail knowledge recapture" has good suitability for the following reasons:

- Tail knowledge retrieval is something that LLMs obviously couldn't do well enough by themselves.
- To answer tail knowledge questions (focusing on those entities and their attributes): once you find the knowledge from the right source (just that the source is not easy to figure out), then the question should be answered in a straightforward manner. Compared to fact verification with LLMs, which is also an active field, it actually removes one layer where LLMs may hallucinate, and makes the problem more interpretable.
- Tail knowledge recapture clearly has potential in real-world applications towards knowledge graph construction.


2. **Q:** Why Q-Learning? Q-Learning seems to be an outdated approach.
**A:** The work here serves as a baseline and puts an emphasis on interpretability too. In this work, Q-Learning is compared against an iterative approach from a recent publication. The argument is that this problem space is not super complex and Q-Learning with a few states would adequately work in the research scope. Plus, by tracking the state transition with Q-Learning, the advantage of RL-assisted approach is illustrated with real examples. Of course, the RL used could be, and should be more sophisticated when being applied in scale.
