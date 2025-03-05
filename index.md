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

This project aims to explore novel ways to make the qualitative coding of user privacy preferences more efficient and specific, particularly through the use of large language models such as ChatGPT. By using LLMs to generate context-specific survey response options, we seek to combine the two traditional approaches to qualitative coding to obtain the benefits of both without their drawbacks. Our goal is to streamline the qualitative coding process, enhance the specificity of the results, and ultimately provide more accurate insights into what users truly care about when it comes to their privacy.

Through this work, we aim to bridge the gap between the qualitative nature of user privacy preferences and the quantitative analysis required for effective privacy policy implementation. By improving the efficiency and specificity of qualitative coding, we hope to empower organizations to better understand and address user privacy concerns, fostering a stronger sense of trust and alignment with users’ expectations. Additionally, this project has the potential to contribute to the broader field of privacy research, helping to shape more effective privacy policies and tools that are in line with the needs of today’s digital society. Beyond privacy, the techniques explored in this system can be generalized and applied to any domain requiring qualitative coding, offering valuable insights and a new approach to qualitative coding.

## Methods

### Generative Choice Survey

This is a sample paragraph under Heading 2. You can add more details here.

-   **Survey Component Integration:** Edward contributed significantly by integrating the ‘survey-react-ui‘ package, which forms the backbone of the survey generation functionality. This package provides an intuitive way to programmatically generate and customize surveys in React, a critical step in enabling interactive survey flows for users. This integration also involved adjusting the survey structure to support dynamic content, eventually allowing the survey to change based on user responses.

-   **Development of Survey Generation:** Once the new survey package had been successfully integrated, David worked on adapting the current survey data schema to the new survey structure of ‘survey-react-ui’, allowing us to generate a unique survey for each decoupled privacy diagram data path.

-   **Survey Page Routes and Export Functionality:** Edward, alongside David, implemented new dynamic routes to handle survey/data path-specific pages. We leveraged session cookies to uniquely identify each user session, allowing developers to send privacy surveys to users with one generalized link. This new direct survey deployment workflow for developers means developers can have immediate access to survey responses, completely eliminating the reliance on third-party systems such as Qualtrics for survey distribution and response collection.
-   **Database and Backend Enhancements:** We redesigned the database schema to support multi-session storage, enabling longitudinal analysis of user responses and improving the adaptability of future surveys.

-   **Generative Survey Options:** We utilized the ChatGPT API to generate adaptive survey response options tailored to users' previous answers, enabling a more efficient and precise identification of their privacy preference profiles.

## Results

The project resulted in the development of an integrated platform that combines the two traditional approaches to qualitative coding, resulting in a novel system that leverages the power of advanced large language models to dynamically generate context-specific survey response options for each question. The key outcomes include:

1. ### Dynamic Survey Integration:

    - A survey system powered by the `survey-react-ui` package that adapts questions based on user inputs.
    - Metadata-enriched survey nodes for tracking and documenting data interactions.
    - Features for exporting survey results and linking responses to backend storage for transparency.
    - Automation of survey creation steps, eliminating reliance on external tools like Qualtrics by using our own programs to dynamically generate and manage surveys.

2. ### Deliverables:

    - **Generative Survey Platform:** Overhauled survey generation, distribution, and collection system allowing for future development of dynamic surveys.

## Discussion

The ideas and frameworks explored in this project represents a significant step forward in addressing the challenges of understanding and categorizing user privacy preferences. By leveraging AI-driven generative surveys and structured response filtering, we have created a system that not only streamlines the qualitative coding process but also enhances the specificity and accuracy of the insights derived from user responses. This approach directly tackles the limitations of traditional methods, such as manual coding of free text responses and static surveys, which are often time-consuming, inconsistent, and fail to capture the nuanced nature of privacy concerns.

One of the key achievements of this project is the ability to bridge the gap between qualitative user privacy preferences and quantitative analysis. By automating the generation of survey options and refining response specificity, the system reduces the manual effort required for qualitative coding while improving the depth and accuracy of the results. This not only benefits researchers and developers but also empowers users by ensuring their privacy concerns are more accurately captured and addressed.

Despite these advancements, further research is still needed to more rigorously benchmark the effectiveness of this novel approach against established baselines. Specifically, future work should compare the performance of our system to a few key alternatives: (1) the traditional method of manual labeling of free-text responses, (2) a modified approach where a Large Language Model (LLM) is used to directly label free-text responses, and (3) the traditional exhaustive survey. Such comparisons would provide valuable insights into the relative strengths and limitations of each method, particularly in terms of accuracy, efficiency, scalability, and the quality of data collected.

## Conclusion

This project has laid the groundwork for a novel approach to qualitative coding, focusing on the specific challenge of capturing and analyzing user privacy preferences. By combining AI-driven generative surveys with structured response filtering, the system offers a scalable and efficient alternative to traditional methods, which are often labor-intensive and or lead to vague, general answers. The dynamic generative survey system, powered by survey-react-ui and ChatGPT, demonstrates the potential to improve the specificity and accuracy of qualitative coding while reducing manual effort.

However, as an exploratory effort, this project is admittedly limited in its scope and lacks rigorous experimentation and user testing. Further research is essential to validate the effectiveness of this approach. Future studies should benchmark the system against traditional manual labeling of free-text responses and a modified approach using an LLM to label free-text responses. These comparisons will help determine the relative advantages and limitations of each method, providing a clearer understanding of how this novel approach can be refined and applied more broadly.

Ultimately, this project highlights the potential of AI-driven tools to transform qualitative coding processes, particularly in the context of privacy research. By continuing to build on this foundation, future work can contribute to the development of more effective privacy policies and tools, fostering greater trust and alignment between users and organizations in the digital age.

## References

-   [Lean Privacy Review](https://www.haojianj.in/resource/pdf/LeanPrivacyReview.pdf)
-   [link2]()
