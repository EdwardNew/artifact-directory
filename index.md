---
title: "Demystifying Privacy: Building Tools for Clear and Accessible Data Security Practices"

description: "By: Edward New, David Yonemura, Adalina Ma; Mentored by Haojian Jin"
---

### Project Link:

-   [Github](https://github.com/DataSmithLab/PrIDE-web/tree/survey)
-   [Report](https://github.com/DataSmithLab/PrIDE-web/tree/survey)
-   [Poster](https://github.com/DataSmithLab/PrIDE-web/tree/survey)
-   [About](https://github.com/DataSmithLab/PrIDE-web/tree/survey)

## Introduction

Qualitative coding or the assigning of labels/codes to qualitative data is a difficult and expensive process in all social science fields; however, it is particularly difficult in our domain of interest: data privacy. This is because the two main traditional methods of qualitative coding in this field involve either a multiple choice of pre-defined answers written by the researchers or free-text response by partcipants. The first method runs into the issues of: 
- An unwiedly amount of answers to cover for all possible privacy preferences.
- A failure to capture the nuance and subjective nature of privacy preferences.
- Participant survey fatigue caused by an overwhelming number of responses required for each question.  

For the second method involving free-text responses, this method runs into issues such as: 
- Participants stuggling to articulate their own privacy preferences. 
- Participants writing what they perceive to be their privacy preferences, even if it doesn't match their online behavior. 
- Participant survey fatigue from having to write out a thoughtful and informative response for each question. 
- Time-consuming, expensive, and error-prone manual labeling of free-text by researchers or crowdworkers. 

This project aims to explore novel ways to make the qualitative coding of user privacy preferences more efficient and specific, particularly through the use of large language models such as ChatGPT. By using LLMs to generate context-specific survey response options, we seek to combine the two traditional approaches to qualitative coding to obtain the benefits of both without their respective drawbacks. Our goal is to streamline the qualitative coding process, enhance the specificity of the results, and ultimately provide more accurate insights into what users truly care about when it comes to their privacy.

Through this work, we aim to bridge the gap between the qualitative nature of user privacy preferences and the quantitative analysis required for effective privacy policy implementation. By improving the efficiency and specificity of qualitative coding, we hope to empower organizations to better understand and address user privacy concerns, fostering a stronger sense of trust and alignment with users' expectations. Additionally, this project has the potential to contribute to the broader field of privacy research, helping to shape more effective privacy policies and tools that are in line with the needs of today's digital society. Beyond privacy, the techniques explored in this system can be generalized and applied to any domain requiring qualitative coding, offering valuable insights and a new approach to qualitative coding.

## Methods

### Paradigms

![Paradigms](/artifact-directory/docs/assets/Paradigms.png)  
  
Our project explores four different paradigms of qualitative coding using LLMS.
- A. Human Responses + Human Labeling
    - Particpants provide open-ended responses and human coders manually analyze and label the data.
    - This is the baseline for comparison on how well the other paradigms perform.
- B. LLM Responses + Human Labeling
    - An LLM generates responses to a privacy scenario and a human choses which option best matches their privacy preference. 
- C. Human Responses + LLM Labeling
    - Participants provide open-ended responses and an LLM labels the data.
- D. LLM Responses + LLM Labeling
    - An LLM generates responses to a prviacy scenario and another LLM (or the same one) categorizes and labels the responses.  
  
We will explore these four paradigms through an informal study utilizing three participants who will contribute to paradigm A and C through their responses. It is important to note that the intention of this exploration is not to draw a conclusion about which paradigm is the best since we do not have enough data to draw such a conclusion. Rather, the point of this exploration is to see whether or not LLMs have the potential to produce results similar to traditional methods. If there is potential, then further and more rigrous investigation into these four different paradigms can be undertaken.

### Labeling
For labeling, we will be using the privacy concern labels found through the traditional human to human paradigm of qualitative coding from the paper "Lean Privacy Review: Collecting Users' Privacy Concerns of Data Practices at a Low Cost". The link to this paper is referenced below. Additionally, knowing the specifics of the label is not neccessary for understanding the results of our exploration; however, they can be viewed below if interested. 

<details>
  <summary>Lean Privacy Review Labels</summary>
  <ul>
    <li>Invasive monitoring</li>
    <li>Violation of expectations/social norms</li>
    <li>Lack of respect for autonomy</li>
    <li>Lack of informed consent</li>
    <li>Deceptive or misleading data practice</li>
    <li>Lack of protection for vulnerable populations</li>
    <li>Lack of an alternative choice</li>
    <li>Insufficient data security</li>
    <li>Insufficient anonymization</li>
    <li>Too high potential risks</li>
    <li>Bias or discrimination</li>
    <li>Lack of trust for algorithms</li>
    <li>Lack of control of personal data</li>
    <li>A company profits from users' data but provides little value to the users (i.e., data commodification)</li>
  </ul>
</details>

### Metrics of Evaluation
To compare these paradigms, we chose survey reponse time and quality of response as metrics of evaluation. Both varaiables are crucial as we seek to improve the experience for both researchers and participants without jeopardizing result quality. Survey response time is clearly defined, but quality of response, specifically for LLMs, will be compared with human responses, and as long as the LLM gives human-like responses and reasoning, we can mark it as a good quality response. With these four paradigms and metrics, we generated a hypothesis of which paradigm would perform well in each metric. 

### Hypothesis
![Paradigms](/artifact-directory/docs/assets/Hypothesis.png)  
  
Our hypothesis comes from our belief in the phrase "LLMs are good generators, humans are good differentiators", or in essence,  




### Exploration Details
The overarching theme for the privacy scenarios given to the participants for this preliminary study will be about checkout-free retail stores or stores that allow customers to walk out with their products without having to directly pay in store. 


## Results

### Comparison of Paradigms

#### Human Responses + Human Labeling

Participants expressed strong concerns about the potential lack of transparency and ethical issues associated with the data collection process. For example, Participant 1 questioned how the company could track online purchases and whether sensitive information like bank details would be accessed. Both Participant 2 and Partcipant 3 raised concerns about how companies might use this data to promote specific products, with Partcipant 3 noting that this approach could be seen as an invasion of privacy. The main advantage of this method is that it preserves human agency both with responses and labeling, ensuring that subtle meanings and context are accurately captured. However, the method is most notably time consuming as the average response time for filling out the survey was around 14 minutes for only a three question scenario.

#### LLM Responses + LLM Labeling

In this fully automated paradigm, both responses and labeling are generated by an LLM. While this method gave fast responses and labeling While this method is highly scalable and efficient, participants expressed concerns about the lack of human touch in the interpretation of responses. The absence of human judgment in labeling leads to potential loss of nuance and misinterpretation of more complex ideas. Moreover, participants like Participant 1 and Participant 2 were uneasy about how such a system could handle the subtleties of human concerns, particularly privacy-related issues. The primary benefit of this paradigm lies in its efficiency, making it suitable for large-scale surveys. However, it may not fully capture the depth of human concern or provide the interpretability necessary for ethical decision-making.

#### Human Responses + LLM Labeling

This hybrid approach combines human input with automated labeling. Participants appreciated the authenticity of human responses but expressed concerns about the efficiency and consistency of the labeling process. While the LLM can provide quicker and more consistent labeling than manual coders, the lack of human oversight means there is still a risk of misinterpretation. Participant 3 voiced concerns about the ethical implications of profiling, while Participant 2 worried about how much personal data would need to be accessed for accurate labeling. This paradigm offers a balance between human nuance and AI efficiency, making it a strong candidate for scenarios where human input is vital, but scalability is still important.

#### LLM Responses + Human Labeling

The novel approach explored in this study involves generating context-specific survey responses using an LLM, which participants then select from. This method aims to reduce ambiguity in responses and ensure that qualitative coding is structured and efficient. Participants seemed to appreciate the clarity and structure provided by the LLM-generated options but expressed concerns regarding the lack of flexibility in capturing their full range of perspectives. Participant 2, for example, felt that there was potential for bias in the AI-generated options, as the system could present choices based on past behavior rather than a true reflection of current preferences. However, compared to the other paradigms, this method appears to have the advantage of reducing ambiguity and ensuring that qualitative coding is more efficient and accurate. It also allows for human judgment in the final selection, which may mitigate the risk of AI-driven biases.

### Comparison of Participant Reactions

Across the four paradigms, participants showed a preference for models that offered a balance between human input and AI efficiency. In particular, the \textit{Human Responses + LLM Labeling} and \textit{LLM Responses + Human Labeling} paradigms seemed to offer the most promise, as they allowed for human nuance while maintaining the efficiency of AI-driven labeling or response generation. However, both paradigms were also critiqued for their ethical implications, with concerns about privacy and data collection remaining prominent.

### Which Paradigm is Best?

Based on the participants' feedback, the \textit{LLM Responses + Human Labeling} paradigm stands out as the most promising approach. This paradigm combines the efficiency and scalability of AI-generated responses with the interpretive power of human labeling. It mitigates many of the concerns raised about privacy and data collection by reducing the amount of sensitive information required for the coding process, while still maintaining human oversight in the final decision-making process. Although participants expressed some concerns about the rigidity of AI-generated options, they generally appreciated the structured nature of the approach, which minimized ambiguity and improved consistency in the coding process.

On the other hand, the \textit{Human Responses + Human Labeling} approach, while offering deep insights into user concerns, is time-consuming and difficult to scale. The \textit{LLM Responses + LLM Labeling} paradigm, while highly efficient, risks losing the subtlety and interpretability necessary for ethical decision-making. Finally, the \textit{Human Responses + LLM Labeling} paradigm, while retaining human input, struggles with consistency and accuracy in labeling, particularly in addressing the ethical concerns that arise from profiling.


## Conclusion

This project has laid the groundwork for a novel approach to qualitative coding, focusing on the specific challenge of capturing and analyzing user privacy preferences. By combining AI-driven generative surveys with structured response filtering, the system offers a scalable and efficient alternative to traditional methods, which are often labor-intensive and or lead to vague, general answers. The dynamic generative survey system, powered by survey-react-ui and ChatGPT, demonstrates the potential to improve the specificity and accuracy of qualitative coding while reducing manual effort.

However, as an exploratory effort, this project is admittedly limited in its scope and lacks rigorous experimentation and user testing. Further research is essential to validate the effectiveness of this approach. Future studies should benchmark the system against traditional manual labeling of free-text responses and a modified approach using an LLM to label free-text responses. These comparisons will help determine the relative advantages and limitations of each method, providing a clearer understanding of how this novel approach can be refined and applied more broadly.

Ultimately, this project highlights the potential of AI-driven tools to transform qualitative coding processes, particularly in the context of privacy research. By continuing to build on this foundation, future work can contribute to the development of more effective privacy policies and tools, fostering greater trust and alignment between users and organizations in the digital age.

## References

-   [Lean Privacy Review](https://www.haojianj.in/resource/pdf/LeanPrivacyReview.pdf)
-   [link2]()
