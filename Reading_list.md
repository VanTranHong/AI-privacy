## Meeting notes
https://docs.google.com/document/d/1NKpv5Re0yXqZaFWxRFmIhT06RiXt-i4_gvV0v3WzYIQ/edit?tab=t.bmlre6yr5m3a

## Research Questions:

Context: 
- The Hamburg DPA, however, concluded that LLM outputs“do not store the texts used for training in their original form, but process them insuch a way that the training data set can never be fully reconstructed from themodel.”
- The Assembly Floor analysis from August 31 suggests that organizations could comply with deletion requests by preventing their systems from outputting personal information through methods like:
  a)  Filtering and suppressing the system’s inputs and outputs.
  b) Excluding the consumer’s personal information from the system’s training data.
  c) Fine-tuning the system’s model in order to prevent the system from outputting personal information.
  d) Directly manipulating model parameters in order to prevent the system from outputting personal information.
- While some models are closed-sourced, many others are open sourced

1. whether and to what degree personal information exists within AI systems?
2. What is the extent of personal information leak in different types of AI system?
3. What are the safeguards of different AI systems to prevent leaking AI? how effective are the safeguards?
4. What are SOTA mitigation strategy to remove PII from outputs? How effective is each strategy and what is the tradeoff?
5. How effective are PII leakage for different model access?

## AB1008 (CCPA)
1. Definition of sale/sharing
  - selling, renting, releasing, disclosing, disseminating, making available, transferring, or otherwise communicating orally, in writing, or by electronic or other means, a consumer’s personal information by the business to a third party for monetary or other valuable consideration.
2. Clarification of personal information

“Personal information” can exist in various formats, including, but not limited to, all of the following:
- Physical formats, including paper documents, printed images, vinyl records, or video tapes.
- Digital formats, including text, image, audio, or video files.
- Abstract digital formats, including compressed or encrypted files, metadata, or artificial intelligence systems that are capable of outputting personal information.
  
## Articles about AI privacy
1. Exploring privacy issues in the age of AI [https://www.ibm.com/think/insights/ai-privacy]
   
   Why is privacy issue concerning in the AI era:
   - Overcollection of various types of information available in the web for model training, including text, audio, video. Some may contain highly sensitive iinformation such as health, biometric, finance data ..
   - Colleciton of data without consent
   - Use of data without permission
   - Unchecked surveillence and bias
   - Data exfiltration: AI models contain a lot of personal information which can be exploited by attacker via attack such as prompt injection attacks

2. Lasso Research Reveals 13% of Generative AI Prompts Contain Sensitive [https://www.lasso.security/blog/lasso-research-reveals-13-of-generative-ai-prompts-contain-sensitive-organizational-data]

   - Code and Token Sharing (4%), exposed credentials, secrets, or proprietary code.
   - Network Information Exposure (5%)  internal URLs, IPv4 addresses, and MAC addresses.
   - PII and PCI Data Exposure (1.4%) ersonal data were flagged, often including email addresses and payment info.
  
3. Gen AI and LLM Data Privacy Ranking 2025 [https://blog.incogni.com/ai-llm-privacy-ranking-2025/]
   - Le Chat by Mistral AI is the least privacy-invasive platform, with ChatGPT and Grok following closely behind. These platforms ranked highest when it comes to how transparent they are on how they use and collect data, and how easy it is to opt out of having personal data used to train underlying models.
   - Platforms developed by the biggest tech companies turned out to be the most privacy invasive, with Meta AI (Meta) being the worst, followed by Gemini (Google) and Copilot (Microsoft). DeepSeek was also indicated as one of the most privacy invasive.
   - Gemini, DeepSeek, Pi AI, and Meta AI don’t seem to allow users to opt out of having prompts used to train the models.
   - ChatGPT turned out to be the most transparent about whether prompts will be used for model training and had a clear privacy policy.
   - All investigated models collect users’ data from “publicly accessible sources, ” which could include personal information.

## Research papers related to PII leakage
1. Analyzing Leakage of Personally Identifiable Information in Language Models [https://arxiv.org/pdf/2302.00539]
2. ProPILE: Probing Privacy Leakage in Large Language Models [https://arxiv.org/pdf/2307.01881]
3. Privacy Leakage Overshadowed by Views of AI:
A Study on Human Oversight of Privacy in Language Model Agent [https://arxiv.org/pdf/2411.01344]
4. PII-Scope: A Comprehensive Study on Training Data PII
Extraction Attacks in LLMs [https://arxiv.org/pdf/2410.06704]
5. A Little Leak Will Sink a Great Ship: Survey of Transparency for Large
Language Models from Start to Finish [https://arxiv.org/pdf/2403.16139]

