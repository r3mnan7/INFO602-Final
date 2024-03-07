# INFO 602 Final Project - InfoSec Open Source Intelligence (OSINT) Categorization

**Interact with the project in Google Colab using [this link](https://colab.research.google.com/drive/1-KOhatAd2c-ESuqJDZ_76vUH2q4TNbhU?usp=sharing)**

## Executive Summary
### Purpose and Objective
The project aimed to develop an automated model to categorize information security news articles efficiently. This endeavor was propelled by the necessity to stay abreast of the latest cybersecurity threats, vulnerabilities, and industry updates within a limited daily research window. The primary goal was to streamline the process of identifying relevant news, thereby saving time and enhancing the capability to respond promptly to emerging cybersecurity threats.

### Methodology
The project commenced with an exploration of zero-shot classification models, specifically evaluating the bart-large-mnli model for its potential to categorize articles without requiring labeled training data. Despite its innovative approach, zero-shot classification yielded limited success, with an average accuracy rate of 44% and significant prediction confidence issues, as indicated by a Cross-Entropy Loss ranging from 2.42 to 13.55.

Subsequently, the focus shifted towards traditional NLP techniques, implementing a Bag of Words model with TF-IDF weighting. This transition marked a significant improvement in model performance, especially with the integration of the MLPClassifier, achieving a precision of 73%, recall of 71%, and a weighted average F1-score of 72%. The model's Cross-Entropy Loss was notably reduced to 0.774, underscoring enhanced prediction confidence.

Further advancements were realized through the incorporation of sentence and document embeddings, utilizing SBERT and OpenAI's embeddings. This approach provided more nuanced text representations, capturing semantic relationships more effectively. The MLPClassifier, combined with OpenAI Embeddings, emerged as the most effective model, showcasing a precision of 76%, recall of 75%, and a weighted average F1-score of 74%, along with the lowest observed Cross-Entropy Loss of 0.7255. These metrics highlighted the model's superior performance in accurately categorizing cybersecurity content.

### Conclusion
The iterative refinement and adoption of advanced NLP techniques culminated in the development of a highly effective categorization model, significantly outperforming initial expectations and methodologies. The final model, an MLPClassifier with OpenAI Embeddings, demonstrated exceptional accuracy and efficiency, providing a robust solution to the challenge of sifting through vast quantities of cybersecurity news. This project not only achieved its objective of streamlining the information review process for cybersecurity professionals but also set a new standard in the application of machine learning and AI for cybersecurity information management.

### Future Opportunities
Ongoing efforts will concentrate on refining the model, incorporating additional contextual information, and expanding the dataset to encompass a wider array of cybersecurity topics. Ensuring the model's adaptability and accuracy in the dynamically evolving cybersecurity landscape remains a priority, with continuous evaluation and adaptation being key to sustaining its effectiveness and relevance.

