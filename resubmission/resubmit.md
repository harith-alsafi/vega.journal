Reviewer 1:
This paper presents a Vega system that leverages large language models (LLMs) to enable intuitive, natural language control and interrogation of IoT devices. The system consists of a physical circuit with input and output devices, a Raspberry Pi (RPi) integrating a control server, and a web application that incorporates LLM logic via multi-agent systems. The process works as follows: users interact with the system through natural language, which the LLM interprets to remotely send appropriate commands to the RPi. The RPi then executes these instructions on the connected physical circuit, with the results communicated back to the user through LLM-generated responses. While this work is significant, there are several suggestions for improvement

[x] 1. This paper emphasizes that Vega provides natural language interfaces for IoT control, however, LLMs often require more specialized prompts to function effectively. This may hinder users who lack experience in prompt engineering or interacting with LLMs (e.g., ChatGPT).
[add this in IV.A]

[x] 2. In the proposed Vega system, the LLM is accessed via OpenAI’s API rather than through a locally trained or fine-tuned model. Therefore, the LLM may lack specific expertise in IoT hardware control. Could this lead to errors when interpreting more complex commands? 
[mention this in IV.C] cost to benefit ratio 

[x] 3. Although this paper demonstrates a functioning system, it relies on the integration of existing devices and third-party applications, which may lack originality and innovation. [mention in IV.A]

[x] 4. In proposed the multi-agent intelligent chatbot, there are few descriptions of the agents. The author may consider introducing their technical principle, implementation schemes, etc. 
[mention in III.E]

[x] 5. In the conclusion, the authors might consider discussing the limitations of the proposed system and potential directions for future research. 
[Move limitations and future work to conclusion]

[x] 6. Related work is inadequate. For example, there are many recent studies related to LLMs, e.g.,
[1] Large language model enhanced multi-agent systems for 6G communications. IEEE Wireless Communications, 2024. [replace [19]] jiang2023largelanguagemodelenhanced
[2] Large ai model-based semantic communications. IEEE Wireless Communications, 2024, 31(3): 68-75.


Reviewer 2:
[x] The use of technical jargon, while necessary, should be balanced with explanations to ensure accessibility for a broader audience. For instance, briefly explaining terms like “LLM” (Large Language Models) and “multiagents” could help non-experts understand better.
[Explain in II.A] 

[x] Basically, this work is simply text-controlled IoT. In fact, voice-controlled IoT is already mature, e.g., Google Home, etc. The authors make a simple thing complicated with an overkill solution. You just need to use a powerful LLM (and this is not the authors’ contribution) to translate human commands to IoT instructions. This is a fairly trivial task for an average LLM.

-----------------------TODO---------------------------
- 40 vs 38 ---> remove one [x]
- 46 vs 1  ---> remove one [x]
- 22 vs 13 ---> replace one with jiang2023largelanguagemodelenhanced [x]
- rewrite  ---> conclusion; remove redundant info [x]
- rewrite  ---> real life case study [] 
