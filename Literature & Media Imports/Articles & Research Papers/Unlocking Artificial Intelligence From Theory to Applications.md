**

Christopher Mutschler 

Christian Münzenmayer 

Norman Uhlmann 

Alexander Martin   Editors 

Unlocking  Artificial  Intelligence From Theory to Applications  

Unlocking Artificial Intelligence

Christopher Mutschler • Christian Münzenmayer Norman Uhlmann • Alexander Martin Editors 

Unlocking  

Artificial 

Intelligence  

From Theory to Applications

Editors 

Christopher Mutschler Christian Münzenmayer  Division Positioning and Networks Division Smart Sensing and Electronics  Fraunhofer IIS, Fraunhofer Institute Fraunhofer IIS, Fraunhofer Institute  for Integrated Circuits IIS for Integrated Circuits IIS  Nürnberg, Germany Erlangen, Germany  

Norman Uhlmann Alexander Martin  

Division Development Center Fraunhofer IIS, Fraunhofer Institute  X-Ray Technology for Integrated Circuits IIS  Fraunhofer IIS, Fraunhofer Institute Nürnberg, Germany  for Integrated Circuits IIS  

Fürth, Germany 

ISBN 978-3-031-64831-1 978-3-031-64832-8 (eBook)  

https://doi.org/10.1007/978-3-031-64832-8  

This work was supported by Fraunhofer Institut für Integrierte Schaltungen IIS 

© The Editor(s) (if applicable) and The Author(s) 2024. This book is an open access publication.  Open Access This book is licensed under the terms of the Creative Commons Attribution 4.0 International  License (http://creativecommons.org/licenses/by/4.0/), which permits use, sharing, adaptation, distribution  and reproduction in any medium or format, as long as you give appropriate credit to the original author(s)  and the source, provide a link to the Creative Commons license and indicate if changes were made.  The images or other third party material in this book are included in the book’s Creative Commons  license, unless indicated otherwise in a credit line to the material. If material is not included in the  book’s Creative Commons license and your intended use is not permitted by statutory regulation or  exceeds the permitted use, you will need to obtain permission directly from the copyright holder.  The use of general descriptive names, registered names, trademarks, service marks, etc. in this publication  does not imply, even in the absence of a specific statement, that such names are exempt from the  relevant protective laws and regulations and therefore free for general use.  

The publisher, the authors, and the editors are safe to assume that the advice and information in this  book are believed to be true and accurate at the date of publication. Neither the publisher nor the authors or  the editors give a warranty, expressed or implied, with respect to the material contained herein or for  any errors or omissions that may have been made. The publisher remains neutral with regard to  jurisdictional claims in published maps and institutional affiliations.  

This Springer imprint is published by the registered company Springer Nature Switzerland AG  The registered company address is: Gewerbestrasse 11, 6330 Cham, Switzerland  

If disposing of this product, please recycle the paper.  

Preface 

In recent years it has become apparent that the deep integration of artifcial intelli gence (AI) methods in product and services is essential for companies in Germany and world-wide to stay competitive. The use of AI allows large volumes of data to be analyzed, patterns and trends to be identifed, and well-founded decisions to be made on an informative basis. It also enables the optimization of workfows, the au tomation of processes and the development of new services, thus creating potential for new business models and signifcant competitive advantages. 

The use of AI in industry ofers new opportunities to increase productivity, im prove quality, reduce costs and generate new, innovative solutions. Customer satisfac tion can also be increased through improved customer interaction and personalized oferings. The use of AI ofers signifcant potential in terms of quality, efciency and competitiveness - not only for multinational enterprises but also for the small and medium-sized enterprises (SME) which are the industrial backbone of the European economy. On the one hand, the quality of products and services can be increased through the use of suitable tools and methods, which minimizes the susceptibility to errors, optimizes processes and thus increases customer satisfaction. The automa tion of recurring tasks enables resources to be freed up and can lead to increased efciency and productivity. On the other hand, the use of AI enables SMEs to better implement customer requirements, ofer innovative solutions, stand out from the competition and remain competitive in an increasingly globalized and digitalized economy. 

However, the use of AI in SMEs and industry also brings new requirements, such as building up specialist knowledge and mastering technological complexity. The rapid development and the in-depth knowledge required to implement and support suitable methods and tools currently pose major challenges for SMEs in particular. 

To meet the above-mentioned challenges and support the adoption and integration of AI in industry and SMEs, structural measures are required. One suitable measure, for example, would be the fnancing of transfer structures such as the ADA Lovelace Center. Such a targeted development of transfer structures facilitates the transfer of knowledge between research institutions and companies and provides industry and 

v  

vi

Preface   

SMEs with low-threshold access to specialist knowledge and resources in order to exploit the full potential of these technologies. 

The ADA Lovelace Center is a pioneering competence center for AI in Bavaria, the establishment of which was funded by the Bavarian State Ministry of Economic Af fairs, Regional Development and Energy. A central focus of the ADA Lovelace Center is on the development of AI-based solutions for industrial applications in sectors of outstanding importance for Bavaria. These include transportation and trafc, produc tion and Industry 4.0, rail transport, fnancial services and insurance, logistics and healthcare as well as sports. Concepts and solutions for specifc issues are researched and implemented in close cooperation with the application partners. A wide range of AI skills are applied and further developed to promote the targeted and sustainable development of AI skills within partner companies. In addition to scientifc research, particular attention is paid to the promotion of young scientists, who are integrated into industrial research at an early stage. The ADA Lovelace Center bundles and expands the AI expertise and infrastructure of the Friedrich-Alexander-University Erlangen-Nürnberg, Ludwig-Maximilians-University Munich, the Fraunhofer Insti tute for Integrated Circuits IIS, the Fraunhofer Institute for Integrated Systems and Device Technology IISB and the Fraunhofer Institute for Cognitive Systems IKS. Thus, the ADA Lovelace Center has signifcant expertise in all relevant AI processes. 

The center has created an internationally visible network for the Bavarian econ omy, which is dedicated to the fundamental issues of data collection and analysis using AI methods, taking into account data protection and data security. The ADA Lovelace Center supports companies in the Bavarian economy by researching, devel oping and implementing concrete solutions for issues in the feld of AI and enables them to transform their business processes and develop new data-driven business models. This book presents an excerpt from various application areas and method ologies and research areas of AI and explains how those methods and processes can be used successfully in practice. 

Nuremberg, Fürth, Erlangen The Editors 

Acknowledgements 

First of all the Editors want express their greatest thank to Nadine Chrobok-Pensky and her team for their excellent, professional and also human-focused project man agement, motivation, organization, and friendly reminders with a huge amount of commitment and patience. Your work and support of the whole team during the project was outstanding and highly appreciated. 

We would like to express our sincere gratitude to all the authors for their valuable contribution to this book. The expertise and dedication have flled the book with high value content in the feld of artifcial intelligence and its applications, making it a valuable resource for readers in this feld. Your thorough research before and within our joint research project, your insightful analysis, and clear writing style have undoubtedly played a crucial role in the success of this fantastic book. Your commitment to delivering high-quality content is commendable and greatly appre ciated. We, the editors, thank you for your outstanding work. Your contribution will undoubtedly make a signifcant impact on the readers and researchers in the feld. 

On behalf of the entire team and authors, we would like to express our profound thank you to the Bavarian Ministry of Economic Afairs, Regional Development and Energy for your generous support of the ADA Lovelace Center project. Without the fnancial funding, it would not have been possible to successfully execute this project. Your support has allowed us to conduct important research and gain valuable insights. Through your funding, we were able to provide resources and materials that were essential to our work for scientifc community and local, national and international industry. We say thank you to you for your trust in our project and your support across all its stages. Your fnancial support has not only contributed to the realization of this project but will also have a lasting impact on research in this feld. 

It is also very important to mention that such a piece of work can not be done in such excellent quality without the support and advice of an highly rated advisory board consisting of industry and scientifc experts, who were always reachable and willing to give advice, support and direction of research and development. The complete ADA team says thank you for your contribution, enthusiasm and work in all phases of the project. 

vii

viii Acknowledgements

The editors also want to say thank you to all the people "behind the scenes" for management, calculations, administrative tasks, organization of meetings and some food, rooms, projectors, hot and cold drinks, good words of support, fexible and agile management. Thank you for been with the complete team. Your work was highly appreciated. 

The entire team would like to express our sincere appreciation for the invaluable collaboration and support of our cooperation partners. The expertise and dedication have been instrumental in the success of this endeavor. The commitment to our shared goals and your willingness to work together have greatly contributed to the progress and achievements of the project. We are truly grateful for the opportunity to collaborate with such a dedicated group of cooperation partners. 

We also want to thank Ralf Gerstner from Springer Verlag for his patience and continuous support, and the reviewer and proofreaders who helped us improve the book. 

Last but not least, the complete team wants to say thank you to all the cofee machines all around which were able at all times during day and night to provide everybody in need with excellent cofee to keep the work and innovation up and running. 

Nuremberg, Germany Christopher Mutschler Erlangen, Germany Christian Münzenmayer Fürth, Germany Norman Uhlmann Nuremberg, Germany Alexander Martin 

February 2024 

Contents 

Part I Theory 

1 Automated Machine Learning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3 Florian Karl, Janek Thomas, Jannes Elstner, Ralf Gross, Bernd Bischl 1.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 3 1.2 Components of AutoML Systems . . . . . . . . . . . . . . . . . . . . . . . . . . . . 5 

1.2.1 Search Space . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6 1.2.2 Optimization . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 6 1.2.3 Ensembling . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 9 1.2.4 Feature Selection and Engineering . . . . . . . . . . . . . . . . . . . 9 1.2.5 Meta-Learning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 10 1.2.6 A Brief Note on AutoML in the Wild . . . . . . . . . . . . . . . . . 11 

1.3 Selected Topics in AutoML . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 12 1.3.1 AutoML for Time Series Data . . . . . . . . . . . . . . . . . . . . . . . 12 1.3.2 Unsupervised AutoML . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 13 1.3.3 AutoML Beyond a Single Objective . . . . . . . . . . . . . . . . . . 14 1.3.4 Human-In-The-Loop AutoML . . . . . . . . . . . . . . . . . . . . . . . 15 

1.4 Neural Architecture Search . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 16 1.4.1 A Brief Overview of the Current State of NAS . . . . . . . . . 16 1.4.2 Hardware-aware NAS . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 17 

1.5 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 17 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 19 

2 Sequence-based Learning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 27 Christofer Loefer, Felix Ott, Jonathan Ott, Maximilian P. Oppelt, Tobias Feigl 

2.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 27 2.2 Time Series Processing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 29 2.2.1 Time Series Data Streams . . . . . . . . . . . . . . . . . . . . . . . . . . 30 2.2.2 Pre-Processing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 32 2.2.3 Predictive Modelling . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 32 

ix

Contents 

x

2.2.4 Post-Processing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 33 2.3 Methods . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 33 2.3.1 Temporal Convolutional Networks . . . . . . . . . . . . . . . . . . . 33 2.3.2 Recurrent Neural Networks . . . . . . . . . . . . . . . . . . . . . . . . . 34 2.3.3 Transformer . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 36 2.4 Perspectives . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 38 2.4.1 Time Series Similarity . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 38 2.4.2 Transfer Learning & Domain Adaptation . . . . . . . . . . . . . . 40 2.4.3 Model Interpretability . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 41 2.5 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 43 Acknowledgments . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 43 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 44 

3 Learning from Experience . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 49 Christopher Mutschler, Georgios Kontes, Sebastian Rietsch 

3.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 49 3.2 Concepts of Reinforcement Learning . . . . . . . . . . . . . . . . . . . . . . . . . 50 3.2.1 Markov Decision Processes (MDPs) . . . . . . . . . . . . . . . . . . 50 3.2.2 Dynamic Programming . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 51 3.2.3 Model-free Reinforcement Learning . . . . . . . . . . . . . . . . . . 52 3.2.4 General Remarks . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 52 3.3 Learning purely through Interaction . . . . . . . . . . . . . . . . . . . . . . . . . . 53 3.3.1 Exploration-Exploitation . . . . . . . . . . . . . . . . . . . . . . . . . . . 53 3.4 Learning with Data or Knowledge . . . . . . . . . . . . . . . . . . . . . . . . . . . 57 3.4.1 Model-based RL with continuous Actions . . . . . . . . . . . . . 57 3.4.2 MBRL with Discrete Actions: Monte Carlo Tree Search . 59 3.4.3 Ofine Reinforcement Learning . . . . . . . . . . . . . . . . . . . . . 60 3.4.4 Hierarchical RL . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 63 3.5 Challenges for Agent Deployment . . . . . . . . . . . . . . . . . . . . . . . . . . . 65 3.5.1 Safety through Policy Constraints . . . . . . . . . . . . . . . . . . . . 65 3.5.2 Generalizability of Policies . . . . . . . . . . . . . . . . . . . . . . . . . 66 3.5.3 Lack of a Reward Function . . . . . . . . . . . . . . . . . . . . . . . . . . 67 3.6 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 69 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 70 

4 Learning with Limited Labelled Data . . . . . . . . . . . . . . . . . . . . . . . . . . 77 Christofer Loefer, Rasmus Hvingelby, Jann Goschenhofer 

4.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 77 4.2 Semi-Supervised Learning. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 79 4.2.1 Classical Semi-Supervised Learning . . . . . . . . . . . . . . . . . . 80 4.2.2 Deep Semi-Supervised Learning . . . . . . . . . . . . . . . . . . . . . 80 4.2.3 Self-Training and Consistency Regularization . . . . . . . . . . 83 4.3 Active Learning. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 84 4.3.1 Deep Active Learning (DAL) . . . . . . . . . . . . . . . . . . . . . . . . 85 4.3.2 Uncertainty Sampling . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 85 4.3.3 Diversity Sampling . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 86   

Contents 

xi

4.3.4 Balanced Criteria . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 87   

4.4 Active Semi-Supervised Learning . . . . . . . . . . . . . . . . . . . . . . . . . . . 88 4.4.1 How can SSL and AL Work Together? . . . . . . . . . . . . . . . . 88 4.4.2 Are SSL and AL Always Mutually Benefcial? . . . . . . . . . 89 

4.5 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 90 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 91 

5 The Role of Uncertainty Quantifcation for Trustworthy AI . . . . . . . . 95 Jessica Deuschel, Andreas Foltyn, Karsten Roscher, Stephan Scheele,† 5.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 95 5.2 Towards Trustworthy AI . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 96 

5.2.1 The EU AI Act . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 97 5.2.2 From Uncertainty to Trustworthy AI . . . . . . . . . . . . . . . . . . 98 5.3 Uncertainty Quantifcation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 99 5.3.1 Sources of Uncertainty . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 100 5.3.2 Methods for Quantifcation of Uncertainty and Calibration103 5.3.3 Evaluation Metrics for Uncertainty Estimation . . . . . . . . . 107 5.4 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 110 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 111 

6 Process-aware Learning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 117 Christian M.M. Frey, Simon Rauch, Oliver Stritzel, Moike Buck 6.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 117 6.2 Overview of Process Mining . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 119 

6.2.1 Process Mining - Basic Concept . . . . . . . . . . . . . . . . . . . . . 120 6.2.2 Process Mining - Types . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 120 6.2.3 Event Log . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 122 6.2.4 Four Quality Criteria . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 125 6.2.5 Types of Processes . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 125 

6.3 Process-Awareness from Theory to Practice . . . . . . . . . . . . . . . . . . . 126 6.3.1 Predictive Analysis in Process Mining . . . . . . . . . . . . . . . . 127 6.3.2 Predictive Process Mining with Bayesian Statistics . . . . . . 128 6.3.3 Process AI . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 131 

6.4 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 133 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 134 

7 Combinatorial Optimization . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 137 Jan Krause, Tobias Kuen, Christopher Scholl 

7.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 137 7.2 Solving Methods . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 139 7.2.1 Heuristics . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 139 7.2.2 Exact Methods . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 140 7.3 Modeling Techniques . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 142 7.3.1 Graph Theory. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 142 

7.3.2 Mixed Integer Programs and Connections to Machine Learning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 145 

Contents 

xii

7.3.3 Pooling . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 148 7.4 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 150 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 151 

8 Acquisition of Semantics for Machine-Learning and Deep-Learning based Applications. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 153 Thomas Wittenberg, Thomas Lang, Thomas Eixelberger, Roland Gruber 8.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 154 8.2 Approaches to Acquire Semantics . . . . . . . . . . . . . . . . . . . . . . . . . . . 155 

8.2.1 Manual Annotation and Labeling . . . . . . . . . . . . . . . . . . . . 156 8.2.2 Data Augmentation Techniques . . . . . . . . . . . . . . . . . . . . . . 157 8.2.3 Simulation and Generation . . . . . . . . . . . . . . . . . . . . . . . . . . 159 8.2.4 High-End Reference Sensors . . . . . . . . . . . . . . . . . . . . . . . . 163 8.2.5 Active Learning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 164 8.2.6 Knowledge Modeling Using Semantic Networks. . . . . . . . 166 8.2.7 Discussion . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 168 

8.3 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 170 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 171 

Part II Applications 

9 Assured Resilience in Autonomous Systems – Machine Learning Methods for Reliable Perception . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 179 Gereon Weiss, Jens Gansloser, Adrian Schwaiger, Maximilian Schwaiger 

9.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 179 9.1.1 The Perception Challenge . . . . . . . . . . . . . . . . . . . . . . . . . . . 180 9.2 Approaches to reliable perception . . . . . . . . . . . . . . . . . . . . . . . . . . . . 181 9.2.1 Choice of Dataset . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 181 9.2.2 Unexpected Behavior of ML Methods . . . . . . . . . . . . . . . . 181 9.2.3 Reliable Object Detection for Autonomous Driving . . . . . 182 9.2.4 Uncertainty Quantifcation for Image Classifcation . . . . . 183 9.2.5 Ensemble Distribution Distillation for 2D Object 

Detection . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 184 

9.2.6 Robust Object Detection in Simulated Driving 

Environments . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 189 

9.2.7 Out-of-Distribution Detection . . . . . . . . . . . . . . . . . . . . . . . 191 9.3 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 195 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 195 

10 Data-driven Wireless Positioning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 199 Maximilian Stahlke, Tobias Feigl, Sebastian Kram, Jonathan Ott, Jochen Seitz, Christopher Mutschler 

10.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 200 10.2 AI-Assisted Localization . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 201 10.3 Direct Positioning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 202   

Contents 

xiii

10.3.1 Model . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 202 10.3.2 Experimental Setup . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 203 10.3.3 Evaluation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 206 10.3.4 Hybrid Localization . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 207 10.3.5 Zone Identifcation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 207 10.3.6 Experimental Setup . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 208 10.3.7 Environments . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 209 10.3.8 Evaluation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 209   

10.4 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 211 Acknowledgements . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 211 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 211 

11 Comprehensible AI for Multimodal State Detection . . . . . . . . . . . . . . 215 Andreas Foltyn, Maximilian P. Oppelt 

11.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 215 11.1.1 Cognitive Load Estimation . . . . . . . . . . . . . . . . . . . . . . . . . . 216 11.1.2 Challenges in Afective Computing . . . . . . . . . . . . . . . . . . . 217 

11.2 Data Collection . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 218 11.2.1 Annotation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 219 11.2.2 Data Preprocessing . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 220 

11.3 Modeling . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 220 11.3.1 In-Domain Evaluation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 221 11.3.2 Cross-Domain Evaluation . . . . . . . . . . . . . . . . . . . . . . . . . . 221 11.3.3 Interpretability . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 222 11.3.4 Improving ECG Representation Learning . . . . . . . . . . . . . 223 11.3.5 Deployment and Application . . . . . . . . . . . . . . . . . . . . . . . . 225 

11.4 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 226 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 226 

12 Robust and Adaptive AI for Digital Pathology . . . . . . . . . . . . . . . . . . . 229 Michaela Benz, Petr Kuritcyn, Rosalie Kletzander, Volker Bruns 12.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 229 12.2 Applications: Tumor Detection and Tumor-Stroma Assessment . . . 230 

12.2.1 Generation of Labeled Data Sets . . . . . . . . . . . . . . . . . . . . . 232 12.2.2 Data Sets for Tumor Detection . . . . . . . . . . . . . . . . . . . . . . . 234 12.2.3 Data Set for Tumor-Stroma Assessment . . . . . . . . . . . . . . . 236 

12.3 Prototypical Few-Shot Classifcation . . . . . . . . . . . . . . . . . . . . . . . . . 237 12.3.1 Robustness through Data Augmentation . . . . . . . . . . . . . . . 238 12.3.2 Out-of-Distribution Detection . . . . . . . . . . . . . . . . . . . . . . . 242 12.3.3 Adaptation to Urothelial Tumor Detection . . . . . . . . . . . . . 242 12.3.4 Interactive AI Authoring with MIKAIA® . . . . . . . . . . . . . . 243 

12.4 Prototypical Few-Shot Segmentation . . . . . . . . . . . . . . . . . . . . . . . . . 245 12.4.1 Tumor-Stroma Assessment . . . . . . . . . . . . . . . . . . . . . . . . . . 246 12.5 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 247 Acknowledgements . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 248 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 248   

xiv

Contents   

13 Safe and Reliable AI for Autonomous Systems . . . . . . . . . . . . . . . . . . . 251 Axel Plinge, Georgios Kontes, Sebastian Rietsch, Christopher Mutschler 13.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 251 

13.1.1 Reinforcement Learning . . . . . . . . . . . . . . . . . . . . . . . . . . . . 252 13.1.2 Reinforcement Learning for Autonomous Driving . . . . . . 253 13.2 Generating Environments with Driver Dojo . . . . . . . . . . . . . . . . . . . 255 13.2.1 Method . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 256 13.3 Training safe Policies with SafeDQN . . . . . . . . . . . . . . . . . . . . . . . . . 258 13.3.1 Method . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 258 13.3.2 Evaluation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 259 13.4 Extracting tree policies with SafeVIPER . . . . . . . . . . . . . . . . . . . . . . 260 13.4.1 Training the Policy . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 261 13.4.2 Verifcation of Decision Trees . . . . . . . . . . . . . . . . . . . . . . . 261 13.4.3 Evaluation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 262 13.5 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 264 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 266 

14 AI for Stability Optimization in Low Voltage Direct Current Microgrids . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 269 Georg Roeder, Rafael Schwanninger, Peter Wienzek, Moritz Kerscher, Bernd Wunder, Martin Schellenberger 

14.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 269 14.2 Low Voltage DC Microgrids . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 270 14.2.1 Control of Low Voltage DC Microgrids . . . . . . . . . . . . . . . 270 14.2.2 Stability of Low Voltage DC Microgrids . . . . . . . . . . . . . . 272 14.3 AI-based Stability Optimization for Low Voltage DC Microgrids . 274 14.3.1 Overview . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 274 14.3.2 Digital Network Twin and Generation of Labels to 

Describe the Stability State . . . . . . . . . . . . . . . . . . . . . . . . . 275 

14.3.3 LVDC Microgrid Surrogate Model Applying Random Forests . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 275 

14.3.4 Stability Optimization Applying Decision Trees . . . . . . . . 277 14.4 Implementation and Assessment . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 278 14.4.1 Measurement of Grid Stability . . . . . . . . . . . . . . . . . . . . . . . 278 14.4.2 Experimental Validation . . . . . . . . . . . . . . . . . . . . . . . . . . . . 280 14.5 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 282 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 283 

15 Self-Optimization in Adaptive Logistics Networks . . . . . . . . . . . . . . . . 287 Julius Mehringer, Ursula Neumann, Friedrich Wagner, Christopher Scholl 

15.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 287 15.2 A Brief Overview of Relevant Literature on Predicting the All-Time Buy Quantity . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 288 15.3 Predicting the All-Time Buy . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 289 15.4 A Probabilistic Hierarchical Growth Curve model . . . . . . . . . . . . . . 291   

Contents 

xv  

15.5 Determining the Optimal Order Policy . . . . . . . . . . . . . . . . . . . . . . . . 294 15.5.1 Modeling Non-Linear Costs . . . . . . . . . . . . . . . . . . . . . . . . . 295 15.5.2 Robust Optimization . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 296 

15.6 Pooling . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 298 15.7 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 299 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 300 

16 Optimization of Underground Train Systems . . . . . . . . . . . . . . . . . . . . 303 Lukas Hager, Tobias Kuen 

16.1 Optimization of DC Railway Power Systems . . . . . . . . . . . . . . . . . . . 304 16.1.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 304 16.1.2 Optimal Power Flow and mathematical MIQCQP model . 304 16.1.3 Case Studies . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 309 

16.2 Energy-Efcient Timetabling applied to a German Underground System . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 313 16.2.1 Industrial Challenge and Motivation . . . . . . . . . . . . . . . . . . 313 16.2.2 Mathematical Research . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 313 16.2.3 Implementation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 317 

16.3 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 318 Acknowledgements . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 319 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 319 

17 AI-assisted Condition Monitoring and Failure Analysis for Industrial Wireless Systems . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 321 Ulf Wetzker, Anna Richter, Vineeta Jain, Jakob Wicht 

17.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 321 17.2 Verifying Data Source Accuracy in Protocol Analysis . . . . . . . . . . . 323 17.2.1 System Concept . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 325 17.2.2 Autoencoder Architecture for Anomaly Detection. . . . . . . 326 17.2.3 Dataset and Performance Evaluation . . . . . . . . . . . . . . . . . . 327 17.3 Automated and User-friendly Spectral Analysis . . . . . . . . . . . . . . . . 328 17.3.1 ML-based Spectrum Analysis . . . . . . . . . . . . . . . . . . . . . . . 329 17.3.2 Generation of Training and Validation Data . . . . . . . . . . . . 329 17.3.3 Model Validation Using Artifcial and Measurement Data 330 17.3.4 System Architecture . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 331 17.4 Cross-layer Analysis . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 332 17.4.1 Variable Adaptive Dynamic Time Warping: A Novel 

Approach . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 333 

17.4.2 Experimental Results and Discussion . . . . . . . . . . . . . . . . . 334 17.4.3 Implications for Research and Beyond . . . . . . . . . . . . . . . . 336 17.5 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 336 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 337   

xvi

Contents   

18 XXL-CT Dataset Segmentation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 339 Roland Gruber, Stefen Rüger, Moritz Ottenweller, Norman Uhlmann, Stefan Gerth 

18.1 Introduction . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 340 18.2 XXL-CT Dataset Acquisition . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 341 18.3 Annotation Pipelines . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 343 

18.3.1 3D Instance Labelling Pipeline . . . . . . . . . . . . . . . . . . . . . . 344 18.3.2 3D Semantic Labelling Pipeline . . . . . . . . . . . . . . . . . . . . . 345 18.4 Training Infrastructure and Segmentation Results. . . . . . . . . . . . . . . 347 18.4.1 Instance Segmentation . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 347 18.4.2 Semantic Segmentation . . . . . . . . . . . . . . . . . . . . . . . . . . . . 349 18.5 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 353 Acknowledgments . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 355 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 355 

19 Energy-Efcient AI on the Edge . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 359 Nicolas Witt, Mark Deutel, Jakob Schubert, Christopher Sobel, Philipp Woller 

19.1 AI on the Edge . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 360 19.2 Energy-Efcient Classical Machine Learning . . . . . . . . . . . . . . . . . . 362 19.2.1 Classifcation of Time Series Data . . . . . . . . . . . . . . . . . . . 362 19.2.2 Multi-Objective Optimization . . . . . . . . . . . . . . . . . . . . . . . 363 19.2.3 Energy Prediction for Classical Machine Learning . . . . . . 364 19.2.4 EA-AutoML Tool . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 366 19.2.5 Application Example . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 367 19.3 Energy-Efcient Deep Learning . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 369 19.3.1 Deep Compression . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 370 19.3.2 Efcient Design Space Exploration . . . . . . . . . . . . . . . . . . . 373 19.3.3 Benchmarking Edge AI . . . . . . . . . . . . . . . . . . . . . . . . . . . . 375 19.4 Conclusion and Outlook. . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 376 References . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . . 378 

Part I 

Theory

Chapter 1 

Automated Machine Learning 

Florian Karl1,2,4, Janek Thomas2, Jannes Elstner1, Ralf Gross3, Bernd Bischl1,2,4 

Abstract In the past few years automated machine learning (AutoML) has gained a lot of traction in the data science and machine learning community. AutoML aims at reducing the partly repetitive work of data scientists and enabling domain experts to construct machine learning pipelines without extensive knowledge in data science. This chapter presents a comprehensive review of the current leading AutoML methods and sets AutoML in an industrial context. To this extent we present the typical components of an AutoML system, give an overview over the state of-the-art and highlight challenges to industrial application by presenting several important topics such as AutoML for time series data, AutoML in unsupervised settings, AutoML with multiple evaluation criteria, or interactive human-in-the-loop methods. Finally, the connection to Neural Architecture Search (NAS) is presented and a brief review with special emphasis on hardware-aware NAS is given. 

Key words: AutoML, Neural Architecture Search, Black-box Optimization 

1.1 Introduction 

Machine learning (ML) has achieved remarkable results across a number of domains in many diferent applications. However, this success highly depends on the identi fcation of a good model and its integration with suitable preprocessing procedures, feature engineering, and other stages within an ML pipeline. Furthermore, even upon 

1Fraunhofer Institute for Integrated Circuits IIS, Fraunhofer IIS, Nuremberg, Germany 2Ludwig-Maximilians-Universität München, Munich, Germany 

3Siemens Digital Industries, Nuremberg, Germany 

4Munich Center for Machine Learning, Munich, Germany 

Corresponding author: Florian Karl 

e-mail: florian.karl@iis.fraunhofer.de 

© The Author(s) 2024 3 C. Mutschler et al. (eds.), Unlocking Artificial Intelligence,  

https://doi.org/10.1007/978-3-031-64832-8_1 

4 Florian Karl et al. 

identifying a suitable model, it still requires precise tuning, as model performance depends substantially on numerous hyperparameters. In short, ML experts must exert considerable manual efort and conduct extensive experimentation to achieve success in ML projects through hyperparameter optimization (HPO) and model selection. 

Automated machine learning (AutoML) can help alleviate this issue by automat ically identifying suitable models or even pipelines, which in turn frees experts up to devote themselves to more interesting and relevant work. However, ML projects should not be viewed merely as the search for an optimal model for a given dataset. The machine learning workfow CRISP-ML(Q), as outlined in [103], consists of six phases: (1) business and data understanding, (2) data engineering, (3) model engineering, (4) model evaluation, (5) model deployment, and (6) model monitoring and maintenance. While all of the described phases can proft from automation and reduction of manual efort, some are clearly better suited; in particular those centered around model development are most attainable as of now [70] and most of current AutoML research centers around this topic [62]. That is not to say AutoML does not 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXe9beoWaJXrp9AWPgFYvK0DzAo0dhyY1Uvb9C__1z0ZWd-MKqW4qYY5Tyoo_e7iI8RUSonSvV8pFykAF7G4pGyjK_5Mhu0N_KqKNYI-TD1mQV1WRoYpq_VYC7z_kaHz6ZQxQKZxzA?key=skTJliiOFdw0rGxL_HdaM5-J)

Fig. 1.1: An overview of what AutoML encompasses in the model engineering and evaluation of the ML workfow. Most elements can be found in the course of this chapter and core concepts are explained in the following subsections. 

extend to other phases: monitoring of data and models, also a relevant topic in the area of machine learning operations (MLOps) for example, provides plenty of oppor tunities for automation and has also been considered as closely connected to model building, which led to research in the area of online AutoML [18]. Furthermore, au tomated data science (AutoDS) is a movement aiming at automation of stages in the ML workfow focused around data, like data acquisition or EDA [31]. Independent of the relevant part of the ML workfow, the overall goal of AutoML is to reduce tedious tasks to a minimum and make ML engineers increasingly efcient in their

1 Automated Machine Learning 5 

work. For the reasons outlined above we will in this work focus on automation in the context of model development. An overview of the steps that can be automated and the topics related to AutoML in this phase can be found in Figure 1.1. 

In the model engineering phase it is usually assumed that a (mostly) clean dataset is available,1 that a performance measure as well as a validation scheme have been defned, and that possible constraints for deployment are known. 

The result of the model engineering phase is an optimized ML pipeline. An ML pipeline is a sequence of preprocessing, modeling and postprocessing operations that is trained on the available data and can be used to predict new observations. Since many ML algorithms are available, each with their unique hyperparameters, fnding an optimal pipeline is a complex and – since training an ML model can require a lot of computational efort – expensive black-box optimization problem. This is further complicated by the fact, that (1) the search space can be mixed (numerical and cat egorical) and involve dependencies or hierarchies, (2) observations, i.e., measured performance of evaluated pipelines, can be inherently noisy and (3) dependencies between pipeline steps and certain hyperparameters are mostly unknown. A consid erable amount of surveys on AutoML exist [121, 36, 126] as well as a textbook [62] to provide a general introduction into the topic. Additionally, recently surveys on subtopics of AutoML have been published, including e.g., neural architecture search (NAS) [115], AutoML for time series forecasting [6] and AutoML for unsupervised methods [8]. 

This chapter aims to provide a condensed overview over the domain of AutoML in the ML workfow phases related to modeling in a practical context, its current appli cations, existing solutions and limitations. After this brief introduction, Section 1.2 presents an evaluation on various AutoML components such as search space, opti mization methods or ensembling. Section 1.3 highlights several selected topics with relevance for industrial applications such as AutoML for time series data, AutoML in low supervision scenarios, multi-objective AutoML and the integration of human experts. After Section 1.4, which gives a brief introduction to NAS with emphasis on the topic of hardware-aware NAS, the chapter concludes with a critical look at challenges and open research topics in the feld of AutoML. 

1.2 Components of AutoML Systems 

In practice, a distinction is made within the feld of AutoML between automatically searching for optimal ML pipelines for “traditional” non deep learning ML methods, and the search for network architectures in deep learning, NAS. Despite its success and relevance, NAS is in literature classifed as a subfeld of AutoML [62]. Most of this section concerns the former, while in Section 1.4 the use and adaption of various methods for NAS is discussed. In general, AutoML systems consist of several 

1 Data cleaning is technically not a part of AutoML and we will exempt this matter from discussion here, though automation in this phase is an interesting topic in itself. We assume that standard procedures (e.g., removal of constant and duplicate features) are always utilized.

6 Florian Karl et al. 

diferent components: search space, optimization, ensembling, feature engineering and meta-learning. Diferent choices for all these components with their advantages and drawbacks are discussed in the following. 

1.2.1 Search Space 

The search space Λ defnes which algorithms, preprocessing and postprocessing operations are considered as well as the ranges of required hyperparameters. Usually, these spaces are defned in a single ML framework, e.g., scikit-learn [90],WEKA [35] or H2O [53]. Λ can be written as a directed acyclic graph, where each node can be associated with discrete, continuous and conditional hyperparameters. Numeric hyperparameters have a fnite range defned by a lower and upper bound. It may not be reasonable to optimize all numeric hyperparameters on a linear scale: The learning rate of neural networks, for example, is generally tuned on an exponential scale, e.g., 10−10, . . . , 10−1. Conditional hyperparameters are only active based on the values of other hyperparameters. For example, the � hyperparameter of a Support Vector Machine (SVM) is only meaningful when the kernel is set to Radial Basis Functions. For an SVM with Linear Basis Functions, � is inactive as it is not used by the model. 

The resulting hierarchical structure of Λ makes optimization with standard tech niques challenging. There is also a clear trade-of in the defnition of Λ. On the one hand, a too restrictive search space may exclude the optimal pipeline and thus cannot be found. On the other hand, a large search space will likely result in difcult and expensive optimization. Ideally the search space should consist of complementing operations, i.e., a method that works well if another method does not and vice-versa. This prevents creation of an unnecessarily vast search space and allocation of too much budget on several methods that are expected to produce similar results. Unfor tunately, it is very hard to learn such an optimal search space in a data-driven way. A large amount of meta-data is required to learn desirable behavior and general state ments are difcult to make over all possible datasets. Notions of transfer learning [91] and adaptive search spaces [54] exist within black-box optimization, but to the best of our knowledge, they have not been successfully integrated in AutoML solutions. Currently, the search space is usually defned in an ad-hoc manner by the developer of the respective AutoML framework with respect to his or her domain knowledge, ML expertise and intended applications as well as some benchmark experiments. 

1.2.2 Optimization 

In addition to the challenges that the structure of Λ pose, despite best design eforts, the search space can become quite large if many diferent operations and model families are considered. The optimization problem is also a black-box optimization

1 Automated Machine Learning 7 

problem, which means that no derivatives of performance with respect to hyperpa rameters are available. In many settings the problem is computationally expensive, as a single evaluation of the black-box typically requires a full cross-validation. Lastly, the optimization is also stochastic, as evaluations are only estimates of the pipeline’s true generalization performance. If those limitations are not taken into account, issues with overtuning can arise [17, 85]. 

Simple Optimization methods such as random or grid search can be quite com petitive [47, 48], as they are hard to misspecify: These approaches forego the use of complex algorithms and there is minimal risk for human error. More sophisticated optimization techniques can break if assumptions, e.g., on the optimization surface, do not hold. In general, random search is always preferable to grid search, as irrele vant hyperparameters do not force identical evaluations [11]. This is also shown in a benchmark study by Zöller et al. [126]. 

Bayesian Optimization is a sequential global optimization method [86, 69] that was developed for expensive black-box problems and is now widely used in HPO and AutoML [99, 60]. The basic idea is to approximate the optimization surface with a probabilistic model, most commonly a Gaussian process; this surrogate is cheap to evaluate and analyze. Optimization is usually initiated by evaluating a certain number of points in a (pseudo-)random manner after which the surrogate model is ft. An infll criterion (or acquisition function) is optimized over the surrogate to select the next optimal point to evaluate; examples include expected improvement or probability of improvement [99]. Typically, an infll criterion balances exploitation of regions with high performance and exploration of regions with high uncertainty [99]. The point obtained through the optimization procedure is then evaluated and the surrogate model is retrained. Applying the method to AutoML poses a challenge, as Bayesian optimization in its original formulation requires a fully numeric confguration space. This is not the case for almost all AutoML systems and applications. A possible solution is to use an appropriate surrogate like a Random Forest instead of a Gaussian process and impute inactive hyperparameters [60]; Neural Networks have also shown promise in combination with a suitable Bayesian treatment like adding a Bayesian linear regressor to the last hidden layer [100]. Another approach is to use a Gaussian process surrogate, but learn lower dimensional numeric embeddings [88]. 

Bayesian optimization is quite fexible and can be extended to optimize multiple performance measures concurrently [58, 71] as well as to handle the stochasticity of the underlying AutoML problem [93]. Letham et al. [76] propose a way to handle noisy or unknown constraints [51], i.e., constraints where it is not (immediately) clear if the proposed ML pipeline is feasible or not. Local Bayesian optimization has been implemented by Eriksson et al. [39] to deal with challenging high dimensionality and large sample budgets. In its original sequential formulation Bayesian optimization is an iterative algorithm that evaluates one point at a time, which can be problematic when trying to parallelize it. It is therefore desirable to adapt Bayesian optimization to generate multi-point or batch proposals, which can be achieved through certain infll criteria [61, 24].

8 Florian Karl et al. 

Evolutionary Algorithms are population-based and stochastic methods inspired by evolution in biology. Evolutionary algorithms generally follow the same pro cedure: After an initial population is sampled and ftness of each individual (an ML pipeline constitutes an individual) is assessed, a sub-population is chosen as parents for the next generation of ofspring. Mutation (random perturbation of an individual) and crossover (combination of attributes of two individuals) operations are employed to generate ofspring. These steps are repeated until a given stopping condition is met, when the best performing pipeline is returned as the fnal result. While requiring a substantial number of evaluations, evolutionary algorithms are a popular choice due to their ability to handle complex search spaces,2 ease of imple mentation, straightforward possibilities for parallelization and the low probability of getting stuck in local optima [4]. Other population based approaches such as particle swarm optimization follow a similar idea. In particle swarm optimization, units of a population of candidate solutions (i.e., particles) traverse the search space based on information about their own respective known states and the behavior of the entire population. In general, these population based optimization techniques are not as efcient as Bayesian optimization and require a larger amount of iterations to fnd good solutions. 

Multi-Fidelity Approaches aim to optimize budget allocation by stopping poor performing pipelines or models early, so as to not waste available budget. Instead of exploiting optimal selection of pipelines to evaluate like the previously presented methods, multi-fdelity methods attempt to fnd good solutions by allocating available budget in an optimal manner. Evaluating ML pipelines (and mainly deep learning architectures) can be expensive and the underlying assumption is, that with less budget, i.e., on a lower fdelity, one can already determine with confdence which pipelines will perform best. Suitable budget types are, for instance, epochs trained, size of training set, or image resolution. 

The simplest implementation of this is successive halving [66]. With successive halving, an amount of randomly sampled confgurations is trained on a low fdelity. The worse performing half of models is then discarded, while the better performing half of models is trained on a higher fdelity and the procedure is repeated. Hyper band [79] is an extension of successive halving to solve the problem of determining the amount of sampled pipelines and the initial fdelity by conducting several suc cessive halving processes from diferent starting conditions. It is not entirely clear, which type of budget (if multiple are a sensible choice) is best for which application so that high rank correlation between fdelities is achieved [34]; the budget is gen erally chosen by the practitioner in an ad-hoc manner. Multi-fdelity approaches can be used in conjunction with many other optimization methods: The simple random sampling in Hyperband can, e.g., be upgraded to Bayesian optimization [40]. 

2 One simply has to defne suitable operations for mutation and crossover. While not always trivial, proper operations have been defned for several elements across the ML pipeline [89].

1 Automated Machine Learning 9 

While these methods constitute arguably the most popular optimizers for Au toML, HPO, and NAS, other methods have been applied successfully to such tasks, including iterative racing, Monte-Carlo Tree Search (MCTS), and gradient-based op timization methods. The interested reader shall be referred to [121, 36, 126, 62, 115] among others. 

1.2.3 Ensembling 

An additional tool used by many AutoML frameworks is model ensembling (in the context of AutoML mostly done through stacking) [16]. In the optimization process, many candidate pipelines are proposed until the budget is used up or a diferent termination criterion is reached. Finally, the best � pipelines can be combined in a powerful ensemble. This can be achieved by simple (weighted) averaging of the pipeline predictions [16] or by training a model using the predictions of the pipelines as new features [117, 106]. Some successful AutoML tools include post-hoc stacking to further boost performance [43], others have ensemble methods as an integral part of the underlying algorithms [19]. Wistuba et al. [116] even use multiple levels of this stacking approach of hundreds of pipelines to achieve very strong predictive performance outperforming 3000 out of 3500 ML expert teams in 12 hours in an ML competition. Similarly, one of the best-performing AutoML tools [47], AutoGluon, relies largely on ensembling and stacking of models in multiple layers [38]. While in many cases ensembling helps boosting the performance of an AutoML tool [52], considerable drawbacks in terms of model size, inference time and general model complexity are apparent. The trade-of between complexity of the solution and its predictive performance needs to be quantifed and a conscious decision has to be made [71]. 

1.2.4 Feature Selection and Engineering 

Feature selection and feature engineering are two important preprocessing steps in an ML pipeline. 

Feature Selection flters relevant features, that are then presented to the ML model. This serves the purpose of reducing model complexity, reducing costs of data acquisition and improving performance by eliminating noisy variables. Including feature selection into AutoML produces the search space {0, 1}� × Λ, where � is the number of initially available features. While often done in a separate step, there is a lot of merit in combining feature selection and the remaining parts of the ML pipeline into one optimization problem [13]. 

Feature Engineering is the process of extracting features from raw data, i.e., multiple data sources. Simple examples of such extractions are sums or averages with an � − 1 relation (combining � sources into one feature) to the target. The amount of

10 Florian Karl et al. 

possible extractions grows immensely with a growing number of relations and variety of extractor functions. This space will quickly become impossible to exhaustively search, so smart search heuristics need to be employed. Kanter et al. [72] propose a greedy exploration strategy to progressively optimize predictive accuracy. If the data is stored in entity-relation-entity format, Cheng et al. [23] propose an efcient way to extract features from the graph that can be used for general ML algorithms. It should be noted, that if automated feature engineering is included in the AutoML framework, we see the input not as a single cleaned data source as discussed in the introduction, but as multiple linked sources. 

1.2.5 Meta-Learning 

In meta-learning, the information on how machine learning models perform on many diferent datasets is used to approach new datasets more efciently [108]. Many diferent tasks such as few-shot [9, 112] or multi-task [15] learning are closely related to meta-learning, but in the context of AutoML a distinction can be made. Meta-learning can be seen as a fundamental concept of AutoML and refers to methods that can leverage information from previous tasks and recommend pipelines or architectures and warm start the AutoML process, thus aiding model selection. In contrast, methods such as transfer learning or few-shot learning produce a fxed architecture and improve only model training (see Figure 1.2). To utilize meta 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdtNYS5Rk3HW56bNeYzlRb1bXjPUQIJOFlsR2caIV2b42PcTaKILXb5gdCz6Sxokmz6T6H9N8TQSbFP7eREw4_daEgWe25UhJSIgGCoFQmHk_DR1GbLMg9JCIEqO0ejHQW8BJKGIA?key=skTJliiOFdw0rGxL_HdaM5-J)

Fig. 1.2: Meta-learning can be divided into two approaches: Some methods support model selection, while others produce a fxed architecture and support model train ing. 

learning for AutoML, it is possible to discretize the search space Λ and create a matrix of datasets � ∈ � and ML pipelines � ∈ Λ where entries in the matrix correspond to the estimated generalization performance of � on �; a technique often utilized in general algorithm selection and confguration. Such data can be collected

1 Automated Machine Learning 11 

from online ML databases like OpenML [109]. This matrix will most likely be very sparse, as not all combinations of datasets and pipelines are evaluated. The estimation of the performance of � on a new dataset �new corresponds to a recommender system in which datasets are users and ML pipelines are items. Recommender systems like collaborative fltering can be used as meta-learning AutoML tools to predict which pipelines to try out next [44, 120]. 

Additional information about the datasets such as size, number and type of fea tures can help to improve the recommendation by calculating the similarity between datasets. Instead of a random or space flling initialization of the search, the best work ing confgurations on similar datasets are used, which can speed up the optimization. Van Rĳn et al. [107] have even used meta-learning to compute symbolic defaults that work well across a large number of datasets. Many meta-learning approaches are limited to examining and comparing confgurations from the same search space. The inclusion of transformers however can allow for utilizing information across diferent search spaces for meta-learning in the context of HPO and AutoML [22]. Taking the notion of meta-learning even one step further, recent approaches to AutoML or NAS, that require a lot of computation on (sometimes synthetic) datasets beforehand, can produce models or architectures for a variety of datasets [75] or even do inference for new datasets out of the box and in a “one-shot manner” [57]. 

1.2.6 A Brief Note on AutoML in the Wild 

Various AutoML tools have been developed and published over the last years - both open source and commercial. However, few success stories of AutoML in real world applications and industry are known, even though AutoML often performs very well on the benchmark data frequently used in scientifc publications and ML competitions. One possible reason for this could be that the application of AutoML is not necessarily made public by users. Nevertheless, the large amount of commercial solutions strongly indicates that a market for AutoML tools exists. AutoML has also been included in major ML platforms from companies such as Microsoft or Amazon. 

In general, there is no single AutoML framework that is suitable for all use cases, since there exists a trade-of between the fexibility and stability of pipeline creation. Compared to frameworks developed by research groups, most frameworks developed in industry limit themselves to shorter pipelines as well as simpler search spaces and optimization strategies, c.f. H2O AutoML. This makes them quite robust and very desirable for users who are looking to harness the power of ML with limited ML knowledge, but not as fexible and powerful as some open source alternatives that ofer more functionality. If the ML task at hand becomes more difcult, e.g., by a larger number of observations, higher dimensionality, or number of classes, some frameworks will experience crashes or produce unsatisfactory results. In particu lar, many AutoML frameworks have issues handling high cardinality categorical features, i.e., categorical features with an extensive amount of possible values. In Gĳsberger et al. [48] H2O AutoML was found to be the most stable framework,

12 Florian Karl et al. 

whereas Zöller et al. [126] report crashes as well as memory and time constraint vi olations for all considered frameworks. The overall diferences between frameworks can be marginal, and a more complex search space does not necessarily guarantee improved results. Both benchmarks [48, 126] are limited to specifc hardware con fgurations. Gĳsberger et al. [48] conduct their benchmark on machines with 32 GB memory and 8 vCPUs with time limits of 1 and 4 hours per run. Zöller et al. [126] conduct their benchmark on almost identical machines for 1.25 hours per run. A second iteration of the AutoML benchmark conducted in [48] has recently been released by Gĳsbers et al. [47]. While this ofers up additional insights into various time limits for AutoML, more benchmarking is required as it remains unclear how AutoML frameworks behave under diferent conditions, for example in large scale distributed systems. 

All the referenced benchmarks give an overview over current open source frame works and attempt a side-by-side comparison incorporating diferent criteria, which present a good resource for further reference. Finally, a recent trend towards targeted AutoML solutions ofers a new trade-of between generalization and functionality by focusing on certain use cases that share common properties in the data or set-up. One example is an AutoML tool targeted at predictive maintenance of expensive ma chinery that has been introduced by German company Weidmüller [1]. The search space of such frameworks is designed to include operations that domain experts deem useful, e.g., certain feature extraction methods for sensor data or proven model classes. Meta-learning in such a focused domain is also considerably easier, as task similarity can be assumed to be much higher [62]. 

1.3 Selected Topics in AutoML 

1.3.1 AutoML for Time Series Data 

While AutoML approaches are often benchmarked on and targeted towards tabular data, NAS publications tend to highlight a lot of applications on image data. When moving to diferent data types like text data, time series data or even multi-modal data, AutoML methods are not as proven and may require substantial modifcations or additions. 

Time series data is especially prevalent in real-world industry applications, which is the reason we choose it to highlight why AutoML methods that work on tabular data can not simply be transferred to other types of data, unique scenarios, and ML tasks other than classifcation or regression. In terms of ML solutions for the typical time series tasks - time series forecasting and time series classifcation - we can divide approaches into three groups [6]: Feature engineering in combination with “traditional” ML approaches, deep learning, and solutions specifc to time series. A more detailed taxonomy can be found in [84]. The sheer number of possible tasks on time series data and the abundance of available methods to solve them make creating an appropriate search space a complicated task.

1 Automated Machine Learning 13 

Feature engineering can be also especially daunting for time series tasks, yet including it in the AutoML framework can be very helpful for users [26]. Several popular packages exist to automate feature construction, among the most used are tsfuse [32] and tsfresh [26]. 

Despite the popularity of deep learning methods and their successful application to both time series forecasting [81] and classifcation [65] it might be better to opt out of expensive deep learning solutions for several applications in industrial settings such as anomaly detection or predictive maintenance [7]. However, plenty of applications are suitable for deep learning; in terms of commercial deep learning tools for time series tasks, e.g., Amazon Web Services has launched GluonTS, which operates with probabilistic methods and deep learning [5]. Solutions specifc to time series tasks are quite diverse. One such example, that has garnered some interest in the past years is the Matrix Profle, which was frst introduced by Yeh et al. in [122]. The Matrix Profle is a metric – essentially achieved by folding a univariate time series with itself – that indicates for each step in the time series how far the most similar pattern is located in the series. This information can be leveraged for a variety of time series and pattern mining tasks like motif detection or anomaly detection among others. In terms of AutoML, many previously discussed techniques can be carried over to certain time series tasks. The need to tackle various tasks based on time series data has led to several tools adapting to support those tasks recently [6]. Specifcally, the AutoML framework Driverless AI from H2O ofers specialized time series tools [3] and AutoGluon from Amazon supports a number of time series applications [2]. NAS for time series tasks, in particular forecasting, has recently shown some success: Wu et al. in [118] discuss the importance of hyperparameter tuning in deep learning approaches for time series and Deng et al. in [34] have developed a NAS framework that can outperform “traditional” time series approaches on a variety of forecasting tasks from diferent application domains. 

1.3.2 Unsupervised AutoML 

While most research focuses on AutoML for supervised learning, there is a growing body of work that applies AutoML to unsupervised learning. Unsupervised learning is a type of ML where algorithms identify patterns and structures within data with out the use of labeled examples. The methods for unsupervised ML are also often highly dependent on critical hyperparameters or even appropriate pre-processing. The biggest challenge in AutoML for unsupervised tasks is that performance eval uation is not as clear as in the supervised case, and defning a single, appropriate metric to evaluate performance of a model is not straightforward [8]. We aim to provide a brief introduction to AutoML for unsupervised ML and its challenges and highlight the important tasks of anomaly detection and clustering. Anomaly detection deals with detecting data points that difer signifcantly from the training distribution, and can be useful for tasks like identifying rare events, e.g., fraud detec tion or intrusion detection [8]. Unsupervised anomaly detection methods often use

14 Florian Karl et al. 

meta-learning to learn from other detection models and datasets to build their own detection model [125], or use human-in-the-loop strategies to train the model [124] (see also Section 1.3.4). Clustering is a task that especially struggles with appropri ate evaluations; often, internal clustering validation criteria are used to ascertain the quality of a model. Many such metrics exist, it is often hard for users to interpret these metrics and using these criteria for model selection and tuning is a challenge. Meta-learning approaches have been shown to utilize these metrics in a meaningful way and have demonstrated good results in AutoML for clustering [33, 67] (c.f. Section 1.2.5). Some AutoML frameworks that rely heavily on meta-learning have been proposed as well [29, 95]. Another AutoML component, that has proven useful for clustering is ensembling [45, 49, 50] (c.f. Section 1.2.3). For a comprehensive overview of AutoML methods for unsupervised settings we refer to Bahri et al. [8]. 

1.3.3 AutoML Beyond a Single Objective 

Existing AutoML approaches mainly fnd an optimal pipeline with respect to one evaluation criterion. In many real-world applications, however, practitioners are usually interested in other objectives as well. There can be multiple metrics that measure the performance of an ML model, and there may also be interest in includ ing secondary objectives such as model complexity, energy efciency, robustness, interpretability or sparseness, which makes the AutoML problem a multi-objective optimization problem [71, 87]. 

A simple solution to this is scalarization, i.e., turning the multi-objective problem into a single objective problem, for example by instead optimizing a weighted sum of the objectives [71]. This however not only requires extensive a priori knowledge about the optimization problem and an idea about possible trade-ofs, but one solu tion cannot comprehensively describe a multi-objective optimization problem with conficting objectives. Therefore, it may be sensible to use multi-objective optimiza tion methods, which usually try to approximate the pareto-front, i.e., to fnd solutions where no single objective can be further improved without trade-ofs in other objec tives and thus present a decision maker (DM) with a set of non-dominated options from which a suitable solution can be chosen. 

Several concepts and optimization methods presented in Section 1.2 can be adapted for the multi-objective case [71],3 but multi-objective AutoML comes with its own set of challenges. In practice it can be hard to judge if an objective identifed in the business understanding phase should be formulated as an objective or a con straint for the ML problem (e.g., should a model be as energy efcient as possible or should energy consumption lie under a certain threshold). The AutoML problem can also be alternatively formulated as a quality diversity optimization problem, i.e., identifying optimal confgurations for each of a set of constrained regions at the same 

3 For an introduction to these methods for HPO and AutoML we refer to [71, 87].

1 Automated Machine Learning 15 

time. This formulation has also shown a lot of promise and presents yet another way to tackle this issue [97]. 

It is often unclear which optimization method to choose for such a multi-objective AutoML problem as benchmarking and evaluation is notoriously hard [71, 42]. Another weakness of multi-objective methods is that approximating the pareto front becomes increasingly difcult or even impossible as the number of objectives increases [77, 64], especially when their interactions are unknown. Yet another approach, that respects the complexity of real world problems, is to involve a DM or domain expert to interact with the optimization algorithm. This addresses some problems, such as objectives that may be hard to quantify or even unknown a priori. We will explore some of these interactive methods in the next section. 

1.3.4 Human-In-The-Loop AutoML 

The goal of automation in ML is not to exclude the – often extremely valuable – human infuence altogether, but more so to reduce tedious, manual tasks as much as possible. How to include domain experts, DMs and ML experts to draw from their knowledge with minimal manual efort for them is very much a vision for AutoML and NAS [59]. How to integrate key human stakeholders in the ML process and specifcally into AutoML during the model phase is a key topic in current AutoML research. Often, trade-ofs cannot be specifed a priori or it is hard to quantify certain objectives; there may also be some hidden objectives that are not formulated at all. Moreover, even if objectives can be specifed, it may not be necessary to explore the entire Pareto-front as is often done in multi-objective optimization, but rather the search for pipelines should be focused around regions preferred by a DM. In such situations, including the preferences of the DM in the optimization process is most often benefcial [78]. Instead of specifying DM preferences in advance, preferences are best included interactively. This essentially puts humans back into the AutoML loop, but instead of confguring ML pipelines, they adjust the search process based on their preferences and expertise. 

There are many ways by which to include DM preferences into the search process. Hakanen et al. [55] show intermediate solutions to the DM and adjust the search by asking for preferred ranges for the objective functions. Gibson et al. [46] allow the DM to set aspirational targets in the objective space that the DM would like to explore. Wang et al. [113] built an interactive visualization tool that allows the DM to modify search space, budget and model selection in an end-to-end workfow. 

Overall, human-in-the-loop AutoML is in some sense contrary to the spirit of Au toML, and it is challenging to fnd the right amount of balance between automation and human intervention. Human-in-the-loop methods also rely on high quality feed back from the DM [78] and the preferences of DMs are always biased to some extent and can even change over time. This can be especially challenging with approaches like preferential Bayesian optimization, when a DM may pick one confguration over another and make a diferent decision under diferent circumstances.

16 Florian Karl et al. 1.4 Neural Architecture Search 

As discussed previously, NAS is a sub-feld of AutoML solely focusing on the architectural design of deep neural networks [127]. Deep learning – among other reasons – has celebrated great success, because it ofers end-to-end solutions for ML, no longer requiring practitioners to build pipelines and carefully select pre-processing operations. However, the choice of architecture as well as hyperparameters like learning rate can have great infuence on the overall performance of a deep learning model. One constraint in terms of applicability of NAS is available data for training and validation. Deep learning itself requires an abundance of data [98] and NAS even more so.4 Shorten and Khoshgoftaar [98] allude to the lack of sufcient data in some domains, suggesting that the same may be true for several industrial use cases. 

1.4.1 A Brief Overview of the Current State of NAS 

The majority of NAS focuses on convolutional neural networks for computer vi sion, but approaches for audio [111], video [94], text [101], time series [34], and tabular [73] data exist. Various architectural designs, such as skip-connections [56], inception modules [104], and more generally multi-branch networks [37] are em ployed frequently. These design choices determine the search space just as the set of preprocessing operations and model families compose the search space for AutoML. Commonly, NAS works with cells, i.e., basic building blocks similar to inception modules that are stacked to make up the network [128], but search spaces are some times also hierarchical or chain-structured. The fnal composition of these cells can be predefned or searched with meta-architecture optimization to choose the number of cells and the confguration of their connections. This already creates an additional hierarchical structure in the optimization procedure by itself [82]. 

While design choices and their hyperparameters are optimized jointly in Au toML, hyperparameters of deep neural networks like regularization, learning rate and schedules are often not considered in NAS. Joint NAS and HPO exists [123], but further increases the computational complexity of NAS. 

The optimization given the search space is very similar to AutoML and while early NAS approaches were centered around reinforcement learning, [127] almost all AutoML optimization techniques introduced so far have been successfully applied to NAS, including random search [80], Bayesian optimization [68, 114], gradient based methods [83], multi-fdelity approaches [74], and evolutionary algorithms [63] among others. Some adaption in the optimizers is required, though. For Bayesian optimization, e.g., a suitable distance function or kernel is required to measure simi larity of architectures. For evolutionary algorithms, mutation and crossing operations for architectures need to be defned. 

4 This is somewhat emphasized by Cui et al. in [30], who consider CIFAR10 a small dataset in the context of NAS.

1 Automated Machine Learning 17 

A big issue in NAS is its enormous computational cost. NAS can require thou sands of GPU hours to fnd state-of-the-art solutions, even for rather simple prob lems. With the trend to larger and larger models, e.g., transformers [110], NAS has become prohibitively expensive [102], which make multi-fdelity methods an important algorithmic component for utilized optimization procedures. In addition, many approaches to reduce the computational cost further exist, e.g., by sharing weights between proposed architectures [92] or by starting from small architectures and learning how to scale them [105]. Another issue with current NAS methods and research is that it is often hard to trust published results due to a lack of shared exper imental protocols and missing ablation studies [119]. New results oftentimes only report little performance gain, that could very well be only due to certain “tricks” in the evaluation protocol [119]. 

1.4.2 Hardware-aware NAS 

In practice, neural networks are deployed on diferent hardware platforms, including GPUs, CPUs, mobile phones and other edge devices and are therefore subject to hardware constraints. Energy efciency and model size are of special concern when deploying deep learning models on edge devices. Hardware performance is also crucial for many real world applications, for example low latency for autonomous driving [10]. This has inspired the subfeld of hardware-aware NAS, which involves taking into account hardware metrics such as latency, memory footprint, etc. in the NAS search process [10]. For this, the standard single-objective NAS problem can, e.g., be altered to a constrained optimization problem or a multi-objective optimization problem that includes appropriate hardware metrics. 

Hardware metrics are either hardware-agnostic such as the number of model pa rameters or hardware-dependent such as latency. During the NAS search, hardware dependent metrics are usually drawn from look-up tables or estimated using a predic tion model [25]. Some hardware-aware NAS methods also jointly optimize hardware design and architecture [41], for example by including the bufer size of FPGA chips in their search [20]. One additional challenge for NAS is the fact that efcient ar chitectures for one specifc hardware are often not necessarily efcient on diferent hardware [14]. To solve this, approaches that guarantee optimal performance on a variety of diferent platforms have been proposed [27]. 

1.5 Conclusion and Outlook 

While AutoML can be useful in many applications and could help increasing the efciency of data scientists, its practical use arises not without its challenges. One common approach is to apply AutoML tools as a quick and automated baseline to see if, for a given dataset, any learning progress can be made [120]. However, in

18 Florian Karl et al. 

some benchmarks of open source AutoML systems, it was shown that for many publicly available datasets the improvement over a simple random forest might be very small [48] – especially on tasks, that are easy to solve. Furthermore, existing AutoML solutions are not necessarily usable out-of-the-box for several applications. For one, most AutoML tools optimize a single performance measure, but for many real-world problems multiple competing performance measures exist. While we discussed the current research in this area in Section 1.3.3, it is evident that a lot of work still needs to be done before these methods can be applied productively on a wider scale, as existing solutions lack in maturity compared to single-objective AutoML tools. 

A related area of future work is human-in-the-loop AutoML (as discussed in Section 1.3.4); the utopian vision for (Automated) ML should not exclude human experts, but rather integrate them into ML processes as efciently as possible. Along the same lines, when applying AutoML to real world problems, the fexibility of AutoML solutions is restricted in the type of problems to which they can be applied. Many AutoML tools can only solve fully supervised regression and classifcation tasks and other data types and ML tasks have only recently been explored. Similarly, AutoML for unsupervised or semi-supervised learning still holds a lot of potential for future work. 

For many data science projects, the main difculty is not the modeling itself but to properly map the underlying business question to a data science problem, acquire the required (labeled) data as well as the general readiness and capability for ML [12, 28]. Bringing automation into other stages of the ML workfow seems daunting as, e.g., business understanding or deployment seem hard to automate, but at the same time ofer great potential for further research. Recent trends to combine AutoML with Large Language Models have sparked a lot of ideas in this direction, as these models could provide a good interface to help facilitate automation across the ML workfow. 

Another open challenge for AutoML is budget selection. It is often unclear to users how much budget to allow for the AutoML process for fnding a suitable pipeline. Stopping the search prematurely could result in a suboptimal pipeline, whereas prolonging the search excessively may waste resources or, in the worst case scenario, lead to overftting [85]. Some frameworks like H2O AutoML include rudimentary early stopping mechanisms which help alleviate this problem, but they have shown to not be optimal [85]. Finally it should be noted that AutoML does not aim to and for the foreseeable future will not be able to replace ML experts and researchers: AutoML is not intended to discover new methods or model types. While publications have played around this idea by showing that an AutoML system based on a search space only including basic operations can indeed “discover” deep learning architectures or methods like back-propagation [96], this is not really feasible for discovery of new methods at the moment – and furthermore is extremely expensive [96]. A follow-up publication showed that along the same lines, it is

1 Automated Machine Learning 19 

possible to discover new algorithmic components through this type of procedure like fnding an improved version of the optimization algorithm Adam5 [21]. 

References 

1. Automated machine learning (industrial automl). https://www.weidmueller.de/de/ produkte/automatisierung_software/automated_machine_learning/index.jsp. Accessed: 2023-12-11. 

2. Time series forecasting - autoglion 1.0.0 documentation. https://auto.gluon.ai/stable/ tutorials/timeseries/index.html. Accessed: 2023-12-11. 

3. Time series in driverless ai. https://docs.h2o.ai/driverless-ai/latest-stable/ docs/userguide/time-series.html. Accessed: 2023-12-11. 

4. A. Abraham and L. Jain. Evolutionary multiobjective optimization. Springer, 2005. 5. A. Alexandrov, K. Benidis, M. Bohlke-Schneider, V. Flunkert, J. Gasthaus, T. Januschowski, D. C. Maddix, S. Rangapuram, D. Salinas, J. Schulz, L. Stella, A. C. Türkmen, and Y. Wang. Gluonts: Probabilistic time series models in python, 2019. 

6. A. Alsharef, K. Aggarwal, M. Kumar, and A. Mishra. Review of ml and automl solutions to forecast time-series data. Archives of Computational Methods in Engineering, 29(7):5297–5311, 2022. 

7. S. D. Anton, L. Ahrens, D. Fraunholz, and H. D. Schotten. Time is of the essence: Machine learning-based intrusion detection in industrial time series data. In 2018 IEEE International Conference on Data Mining Workshops (ICDMW), pages 1–6. IEEE, 2018. 

8. M. Bahri, F. Salutari, A. Putina, and M. Sozio. Automl: state of the art with a focus on anomaly detection, challenges, and research directions. International Journal of Data Science and Analytics, 14(2):113–126, 2022. 

9. E. Bart and S. Ullman. Cross-generalization: Learning novel classes from a single example by feature replacement. In 2005 IEEE Computer Society Conference on Computer Vision and Pattern Recognition (CVPR’05), volume 1, pages 672–679. IEEE, 2005. 

10. H. Benmeziane, K. E. Maghraoui, H. Ouarnoughi, S. Niar, M. Wistuba, and N. Wang. A comprehensive survey on hardware-aware neural architecture search. arXiv preprint arXiv:2101.09336, 2021. 

11. J. Bergstra and Y. Bengio. Random search for hyper-parameter optimization. Journal of Machine Learning Research, 13(Feb):281–305, 2012. 

12. L. Bernardi, T. Mavridis, and P. Estevez. 150 successful machine learning models: 6 lessons learned at booking. com. In Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining, pages 1743–1751, 2019. 

13. M. Binder, J. Moosbauer, J. Thomas, and B. Bischl. Multi-objective hyperparameter tuning and feature selection using flter ensembles. In Proceedings of the 2020 Genetic and Evolutionary Computation Conference, pages 471–479, 2020. 

14. H. Cai, L. Zhu, and S. Han. Proxylessnas: Direct neural architecture search on target task and hardware. In 7th International Conference on Learning Representations, ICLR, 2019. 15. R. Caruana. Multitask learning. Machine learning, 28(1):41–75, 1997. 16. R. Caruana, A. Niculescu-Mizil, G. Crew, and A. Ksikes. Ensemble selection from libraries of models. In Proceedings of the twenty-frst international conference on Machine learning, page 18. ACM, 2004. 

17. G. C. Cawley and N. L. Talbot. On over-ftting in model selection and subsequent selection bias in performance evaluation. Journal of Machine Learning Research, 11(Jul):2079–2107, 2010. 

5 Adam has been established as a standard optimizer when it comes to stochastic gradient descent in the context of training deep learning models.

20 Florian Karl et al. 

18. B. Celik, P. Singh, and J. Vanschoren. Online automl: An adaptive automl framework for online learning. Machine Learning, 112(6):1897–1921, 2023. 

19. B. Chen, H. Wu, W. Mo, I. Chattopadhyay, and H. Lipson. Autostacker: A compositional evolutionary learning system. In Proceedings of the genetic and evolutionary computation conference, pages 402–409, 2018. 

20. W. Chen, Y. Wang, S. Yang, C. Liu, and L. Zhang. You only search once: A fast automation framework for single-stage dnn/accelerator co-design. In 2020 Design, Automation & Test in Europe Conference & Exhibition (DATE), pages 1283–1286. IEEE, 2020. 

21. X. Chen, C. Liang, D. Huang, E. Real, K. Wang, Y. Liu, H. Pham, X. Dong, T. Luong, C.-J. Hsieh, et al. Symbolic discovery of optimization algorithms. arXiv preprint arXiv:2302.06675, 2023. 

22. Y. Chen, X. Song, C. Lee, Z. Wang, R. Zhang, D. Dohan, K. Kawakami, G. Kochanski, A. Doucet, M. A. Ranzato, S. Perel, and N. de Freitas. Towards learning universal hyperpa rameter optimizers with transformers. In Advances in Neural Information Processing Systems, volume 35, pages 32053–32068. Curran Associates, Inc., 2022. 

23. W. Cheng, G. Kasneci, T. Graepel, D. Stern, and R. Herbrich. Automated feature generation from structured knowledge. In Proceedings of the 20th ACM international conference on Information and knowledge management, pages 1395–1404. ACM, 2011. 

24. C. Chevalier and D. Ginsbourger. Fast computation of the multi-points expected improvement with applications in batch selection. In Learning and Intelligent Optimization - 7th International Conference, volume 7997 of Lecture Notes in Computer Science, pages 59–69. Springer, 2013. 

25. K. T. Chitty-Venkata and A. K. Somani. Neural architecture search survey: A hardware perspective. ACM Computing Surveys, 55(4):1–36, 2022. 

26. M. Christ, A. W. Kempa-Liehr, and M. Feindt. Distributed and parallel time series feature extraction for industrial big data applications. arXiv preprint arXiv:1610.07717, 2016. 27. G. Chu, O. Arikan, G. Bender, W. Wang, A. Brighton, P.-J. Kindermans, H. Liu, B. Akin, S. Gupta, and A. Howard. Discovering multi-hardware mobile models via architecture search. In Proceedings of the IEEE/CVF Conference on Computer Vision and Pattern Recognition, pages 3022–3031, 2021. 

28. M. Chui, J. Manyika, M. Miremadi, N. Henke, R. Chung, P. Nel, and S. Malhotra. Notes from the ai frontier: Insights from hundreds of use cases. McKinsey Global Institute, 2018. 29. N. Cohen-Shapira and L. Rokach. Automatic selection of clustering algorithms using super vised graph embedding. Information Sciences, 577:824–851, 2021. 

30. J. Cui, P. Chen, R. Li, S. Liu, X. Shen, and J. Jia. Fast and practical neural architecture search. In The IEEE International Conference on Computer Vision (ICCV), October 2019. 31. T. De Bie1, L. De Raedt, H. H. Hoos, and P. S. Wu. Automating data science. Report from Dagstuhl Seminar 18401, 2019. 

32. A. De Brabandere, P. Robberechts, T. Op De Beeck, and J. Davis. Automating feature con struction for multi-view time series data. In Proceedings of the ECML/PKDD Workshop on Automating Data Science, pages 16–20, 2019. 

33. M. C. De Souto, R. B. Prudencio, R. G. Soares, D. S. De Araujo, I. G. Costa, T. B. Ludermir, and A. Schliep. Ranking and selecting clustering algorithms using a meta-learning approach. In 2008 IEEE International Joint Conference on Neural Networks (IEEE World Congress on Computational Intelligence), pages 3729–3735. IEEE, 2008. 

34. D. Deng, F. Karl, F. Hutter, B. Bischl, and M. Lindauer. Efcient automated deep learning for time series forecasting. In Machine Learning and Knowledge Discovery in Databases: European Conference, ECML PKDD, pages 664–680. Springer, 2023. 

35. F. Eibe, M. A. Hall, and I. H. Witten. The weka workbench. online appendix for data mining: practical machine learning tools and techniques. In Morgan Kaufmann. Morgan Kaufmann Publishers, 2016. 

36. a. Elshawi, M. Maher, and S. Sakr. Automated machine learning: State-of-the-art and open challenges. arXiv preprint arXiv:1906.02287, 2019. 

37. T. Elsken, J. H. Metzen, and F. Hutter. Neural architecture search: A survey. The Journal of Machine Learning Research, 20(1):1997–2017, 2019.

1 Automated Machine Learning 21 

38. N. Erickson, J. Mueller, A. Shirkov, H. Zhang, P. Larroy, M. Li, and A. Smola. Autogluon tabular: Robust and accurate automl for structured data. arXiv preprint arXiv:2003.06505, 2020. 

39. D. Eriksson, M. Pearce, J. Gardner, R. D. Turner, and M. Poloczek. Scalable global optimization via local bayesian optimization. Advances in neural information processing systems, 32, 2019. 40. S. Falkner, A. Klein, and F. Hutter. Bohb: Robust and efcient hyperparameter optimization at scale. arXiv preprint arXiv:1807.01774, 2018. 

41. H. Fan, M. Ferianc, Z. Que, H. Li, S. Liu, X. Niu, and W. Luk. Algorithm and hardware co-design for reconfgurable cnn accelerator. In 2022 27th Asia and South Pacifc Design Automation Conference (ASP-DAC), pages 250–255. IEEE, 2022. 

42. M. Feurer, K. Eggensperger, E. Bergman, F. Pfsterer, B. Bischl, and F. Hutter. Mind the gap: Measuring generalization performance across multiple objectives. In Advances in Intelligent Data Analysis XXI: 21st International Symposium on Intelligent Data Analysis, pages 130–142. Springer, 2023. 

43. M. Feurer, A. Klein, K. Eggensperger, J. Springenberg, M. Blum, and F. Hutter. Efcient and robust automated machine learning. Advances in neural information processing systems, pages 2962–2970, 2015. 

44. N. Fusi, R. Sheth, and M. Elibol. Probabilistic matrix factorization for automated machine learning. In Advances in Neural Information Processing Systems, pages 3348–3357, 2018. 45. J. Ghosh and A. Acharya. Cluster ensembles. Wiley interdisciplinary reviews: Data mining and knowledge discovery, 1(4):305–315, 2011. 

46. F. J. Gibson, R. M. Everson, and J. E. Fieldsend. Guiding surrogate-assisted multi-objective optimisation with decision maker preferences. In Proceedings of the Genetic and Evolutionary Computation Conference, pages 786–795, 2022. 

47. P. Gĳsbers, M. L. Bueno, S. Coors, E. LeDell, S. Poirier, J. Thomas, B. Bischl, and J. Van schoren. Amlb: an automl benchmark. arXiv preprint arXiv:2207.12560, 2022. 48. P. Gĳsbers, E. LeDell, J. Thomas, S. Poirier, B. Bischl, and J. Vanschoren. An open source automl benchmark. In ICML AutoML workshop, 2019. 

49. A. Gionis, H. Mannila, and P. Tsaparas. Clustering aggregation. ACM transactions on knowl edge discovery from data, 1(1), 2007. 

50. K. Golalipour, E. Akbari, S. S. Hamidi, M. Lee, and R. Enayatifar. From clustering to clustering ensemble selection: A review. Engineering Applications of Artifcial Intelligence, 104:104388, 2021. 

51. R. B. Gramacy and H. K. Lee. Optimization under unknown constraints. In Bayesian Statistics 9, pages 229–256. Oxford University Press, 2011. 

52. I. Guyon, A. Safari, G. Dror, and G. Cawley. Model selection: Beyond the bayesian/frequentist divide. Journal of Machine Learning Research, 11(Jan):61–87, 2010. 

53. H2O.ai. H2O: Scalable Machine Learning Platform, 2023. version 3.42.0.3. 54. H. Ha, S. Rana, S. Gupta, T. Nguyen, S. Venkatesh, et al. Bayesian optimization with unknown search space. Advances in Neural Information Processing Systems, 32, 2019. 55. J. Hakanen and J. D. Knowles. On using decision maker preferences with parego. In Evolution ary Multi-Criterion Optimization: 9th International Conference, EMO 2017, pages 282–297. Springer, 2017. 

56. K. He, X. Zhang, S. Ren, and J. Sun. Deep residual learning for image recognition. In Proceedings of the IEEE conference on computer vision and pattern recognition, pages 770– 778, 2016. 

57. N. Hollmann, S. Müller, K. Eggensperger, and F. Hutter. Tabpfn: A transformer that solves small tabular classifcation problems in a second. In The Eleventh International Conference on Learning Representations, ICLR 2023, 2023. 

58. D. Horn, T. Wagner, D. Biermann, C. Weihs, and B. Bischl. Model-based multi-objective opti mization: taxonomy, multi-point proposal, toolbox and benchmark. In International Conference on Evolutionary Multi-Criterion Optimization, pages 64–78. Springer, 2015. 

59. F. Hutter. Automl | deep learning 2.0: Extending the power of deep learning to the meta-level. https://www.automl.org/ deep-learning-2-0-extending-the-power-of-deep-learning-to-the-meta-level/, March 2022. Accessed: 2023-05-12.

22 Florian Karl et al. 

60. F. Hutter, H. H. Hoos, and K. Leyton-Brown. Sequential model-based optimization for general algorithm confguration. In Learning and Intelligent Optimization, pages 507–523. Springer, 2011. 

61. F. Hutter, H. H. Hoos, and K. Leyton-Brown. Parallel algorithm confguration. In Learning and Intelligent Optimization: 6th International Conference, pages 55–70. Springer, 2012. 62. F. Hutter, L. Kotthof, and J. Vanschoren. Automated machine learning-methods, systems, challenges, 2019. 

63. W. Irwin-Harris, Y. Sun, B. Xue, and M. Zhang. A graph-based encoding for evolutionary convolutional neural network architecture design. In 2019 IEEE Congress on Evolutionary Computation (CEC), pages 546–553. IEEE, 2019. 

64. H. Ishibuchi, N. Tsukamoto, and Y. Nojima. Evolutionary many-objective optimization: A short review. In 2008 IEEE congress on evolutionary computation (IEEE world congress on computational intelligence), pages 2419–2426. IEEE, 2008. 

65. H. Ismail Fawaz, G. Forestier, J. Weber, L. Idoumghar, and P.-A. Muller. Deep learning for time series classifcation: a review. Data mining and knowledge discovery, 33(4):917–963, 2019. 66. K. Jamieson and A. Talwalkar. Non-stochastic best arm identifcation and hyperparameter 

optimization. In Artifcial Intelligence and Statistics, pages 240–248, 2016. 67. Y. Jiang and N. Verma. Meta-learning to cluster. arXiv preprint arXiv:1910.14134, 2019. 68. H. Jin, Q. Song, and X. Hu. Auto-keras: An efcient neural architecture search system. In 

Proceedings of the 25th ACM SIGKDD International Conference on Knowledge Discovery & Data Mining, pages 1946–1956. ACM, 2019. 

69. D. R. Jones, M. Schonlau, and W. J. Welch. Efcient global optimization of expensive black-box functions. Journal of Global optimization, 13(4):455–492, 1998. 

70. S. R. Kaminwar, J. Goschenhofer, J. Thomas, I. Thon, and B. Bischl. Structured verifcation of machine learning models in industrial settings. Big Data, 2021. 

71. F. Karl, T. Pielok, J. Moosbauer, F. Pfsterer, S. Coors, M. Binder, L. Schneider, J. Thomas, J. Richter, M. Lang, et al. Multi-objective hyperparameter optimization–an overview. arXiv preprint arXiv:2206.07438, 2022. 

72. U. Khurana, D. Turaga, H. Samulowitz, and S. Parthasrathy. Cognito: Automated feature engineering for supervised learning. In 2016 IEEE 16th International Conference on Data Mining Workshops (ICDMW), pages 1304–1307. IEEE, 2016. 

73. A. Klein and F. Hutter. Tabular benchmarks for joint architecture and hyperparameter opti mization. arXiv preprint arXiv:1905.04970, 2019. 

74. A. Klein, L. C. Tiao, T. Lienart, C. Archambeau, and M. Seeger. Model-based asynchronous hyperparameter and neural architecture search. arXiv preprint arXiv:2003.10865, 2020. 75. H. Lee, E. Hyung, and S. J. Hwang. Rapid neural architecture search by learning to generate graphs from datasets. In 9th International Conference on Learning Representations, ICLR 2021, 2021. 

76. B. Letham, B. Karrer, G. Ottoni, E. Bakshy, et al. Constrained bayesian optimization with noisy experiments. Bayesian Analysis, 14(2):495–519, 2019. 

77. K. Li, K. Deb, and X. Yao. R-metric: Evaluating the performance of preference-based evolu tionary multiobjective optimization using reference points. IEEE Transactions on Evolutionary Computation, 22(6):821–835, 2017. 

78. K. Li, M. Liao, K. Deb, G. Min, and X. Yao. Does preference always help? a holistic study on preference-based evolutionary multiobjective optimization using reference points. IEEE Transactions on Evolutionary Computation, 24(6):1078–1096, 2020. 

79. L. Li, K. Jamieson, G. DeSalvo, A. Rostamizadeh, and A. Talwalkar. Hyperband: A novel bandit-based approach to hyperparameter optimization. arXiv preprint arXiv:1603.06560, 2016. 80. L. Li and A. Talwalkar. Random search and reproducibility for neural architecture search. arXiv preprint arXiv:1902.07638, 2019. 

81. B. Lim and S. Zohren. Time-series forecasting with deep learning: a survey. Philosophical Transactions of the Royal Society A, 379(2194), 2021. 

82. H. Liu, K. Simonyan, O. Vinyals, C. Fernando, and K. Kavukcuoglu. Hierarchical representa tions for efcient architecture search. arXiv preprint arXiv:1711.00436, 2017.

1 Automated Machine Learning 23 

83. H. Liu, K. Simonyan, and Y. Yang. Darts: Diferentiable architecture search. arXiv preprint arXiv:1806.09055, 2018. 

84. M. Löning, A. Bagnall, S. Ganesh, V. Kazakov, J. Lines, and F. J. Király. sktime: A unifed interface for machine learning with time series. arXiv preprint arXiv:1909.07872, 2019. 85. A. Makarova, H. Shen, V. Perrone, A. Klein, J. B. Faddoul, A. Krause, M. Seeger, and C. Archambeau. Overftting in bayesian optimization: an empirical study and early-stopping solution. In 2nd Workshop on Neural Architecture Search (NAS 2021 collocated with the 9th ICLR 2021), 2021. 

86. J. Močkus. On bayesian methods for seeking the extremum. In Optimization Techniques IFIP Technical Conference, pages 400–404. Springer, 1975. 

87. A. Morales-Hernández, I. Van Nieuwenhuyse, and S. Rojas Gonzalez. A survey on multi objective hyperparameter optimization algorithms for machine learning. Artifcial Intelligence Review, pages 1–51, 2022. 

88. A. Nayebi, A. Munteanu, and M. Poloczek. A framework for Bayesian optimization in em bedded subspaces. In Proceedings of the 36th International Conference on Machine Learning, volume 97 of Proceedings of Machine Learning Research, pages 4752–4761. PMLR, 2019. 

89. R. S. Olson, N. Bartley, R. J. Urbanowicz, and J. H. Moore. Evaluation of a tree-based pipeline optimization tool for automating data science. Proceedings of the Genetic and Evolutionary Computation Conference 2016, pages 485–492, 2016. 

90. F. Pedregosa, G. Varoquaux, A. Gramfort, V. Michel, B. Thirion, O. Grisel, M. Blondel, P. Prettenhofer, R. Weiss, V. Dubourg, J. Vanderplas, A. Passos, D. Cournapeau, M. Brucher, M. Perrot, and E. Duchesnay. Scikit-learn: Machine learning in Python. Journal of Machine Learning Research, 12:2825–2830, 2011. 

91. V. Perrone, H. Shen, M. W. Seeger, C. Archambeau, and R. Jenatton. Learning search spaces for bayesian optimization: Another view of hyperparameter transfer learning. Advances in Neural Information Processing Systems, 32, 2019. 

92. H. Pham, M. Y. Guan, B. Zoph, Q. V. Le, and J. Dean. Efcient neural architecture search via parameter sharing. arXiv preprint arXiv:1802.03268, 2018. 

93. V. Picheny, D. Ginsbourger, Y. Richet, and G. Caplin. Quantile-based optimization of noisy computer experiments with tunable precision. Technometrics, 55(1):2–13, 2013. 94. A. Piergiovanni, A. Angelova, A. Toshev, and M. S. Ryoo. Evolving space-time neural archi tectures for videos. In Proceedings of the IEEE International Conference on Computer Vision, pages 1793–1802, 2019. 

95. Y. Poulakis, C. Doulkeridis, and D. Kyriazis. Autoclust: A framework for automated clustering based on cluster validity indices. In 2020 IEEE International Conference on Data Mining (ICDM), pages 1220–1225. IEEE, 2020. 

96. E. Real, C. Liang, D. So, and Q. Le. Automl-zero: Evolving machine learning algorithms from scratch. In International conference on machine learning, pages 8007–8019. PMLR, 2020. 97. L. Schneider, F. Pfsterer, P. Kent, J. Branke, B. Bischl, and J. Thomas. Tackling neural archi 

tecture search with quality diversity optimization. In International Conference on Automated Machine Learning, pages 9–1. PMLR, 2022. 

98. C. Shorten and T. Khoshgoftaar. A survey on image data augmentation for deep learning. Journal of Big Data, 6, 12 2019. 

99. J. Snoek, H. Larochelle, and R. P. Adams. Practical bayesian optimization of machine learning algorithms. Advances in neural information processing systems, 25, 2012. 100. J. Snoek, O. Rippel, K. Swersky, R. Kiros, N. Satish, N. Sundaram, M. Patwary, M. Prabhat, and R. Adams. Scalable bayesian optimization using deep neural networks. In International conference on machine learning, pages 2171–2180. PMLR, 2015. 

101. D. So, Q. Le, and C. Liang. The evolved transformer. In International conference on machine learning, pages 5877–5886. PMLR, 2019. 

102. E. Strubell, A. Ganesh, and A. McCallum. Energy and policy considerations for deep learning in NLP. In Proceedings of the 57th Conference of the Association for Computational Linguistics, ACL 2019, Florence, Italy, July 28- August 2, 2019, Volume 1: Long Papers, pages 3645–3650. Association for Computational Linguistics, 2019.

24 Florian Karl et al. 

103. S. Studer, T. Bui, C. Drescher, A. Hanuschkin, L. Winkler, S. Peters, and K.-R. Müller. Towards crisp-ml(q): A machine learning process model with quality assurance methodology. Machine Learning and Knowledge Extraction, 3(2):392–413, 2021. 

104. C. Szegedy, W. Liu, Y. Jia, P. Sermanet, S. Reed, D. Anguelov, D. Erhan, V. Vanhoucke, and A. Rabinovich. Going deeper with convolutions. In Proceedings of the IEEE conference on computer vision and pattern recognition, pages 1–9, 2015. 

105. M. Tan and Q. Le. Efcientnet: Rethinking model scaling for convolutional neural networks. In International conference on machine learning, pages 6105–6114. PMLR, 2019. 106. M. J. Van der Laan, E. C. Polley, and A. E. Hubbard. Super learner. Statistical applications in genetics and molecular biology, 6(1), 2007. 

107. J. N. van Rĳn, F. Pfsterer, J. Thomas, A. Muller, B. Bischl, and J. Vanschoren. Meta learning for defaults: Symbolic defaults. In Neural Information Processing Workshop on Meta-Learning, 2018. 

108. J. Vanschoren. Meta-learning: A survey. arXiv preprint arXiv:1810.03548, 2018. 109. J. Vanschoren, J. N. Van Rĳn, B. Bischl, and L. Torgo. Openml: networked science in machine learning. ACM SIGKDD Explorations Newsletter, 15(2):49–60, 2014. 

110. A. Vaswani, N. Shazeer, N. Parmar, J. Uszkoreit, L. Jones, A. N. Gomez, Ł. Kaiser, and I. Polosukhin. Attention is all you need. In Advances in neural information processing systems, pages 5998–6008, 2017. 

111. T. Véniat, O. Schwander, and L. Denoyer. Stochastic adaptive neural architecture search for keyword spotting. In ICASSP 2019-2019 IEEE International Conference on Acoustics, Speech and Signal Processing (ICASSP), pages 2842–2846. IEEE, 2019. 

112. O. Vinyals, C. Blundell, T. Lillicrap, D. Wierstra, et al. Matching networks for one shot learning. In Advances in neural information processing systems, pages 3630–3638, 2016. 113. Q. Wang, Y. Ming, Z. Jin, Q. Shen, D. Liu, M. J. Smith, K. Veeramachaneni, and H. Qu. Atm seer: Increasing transparency and controllability in automated machine learning. In Proceedings of the 2019 CHI conference on human factors in computing systems, pages 1–12, 2019. 114. C. White, W. Neiswanger, and Y. Savani. Bananas: Bayesian optimization with neural architectures for neural architecture search. In Proceedings of the AAAI Conference on Artifcial Intelligence, volume 35, pages 10293–10301, 2021. 

115. C. White, M. Safari, R. Sukthanker, B. Ru, T. Elsken, A. Zela, D. Dey, and F. Hutter. Neural architecture search: Insights from 1000 papers. arXiv preprint arXiv:2301.08727, 2023. 116. M. Wistuba, N. Schilling, and L. Schmidt-Thieme. Automatic frankensteining: Creating complex ensembles autonomously. In Proceedings of the 2017 SIAM International Conference on Data Mining, pages 741–749. SIAM, 2017. 

117. D. H. Wolpert. Stacked generalization. Neural networks, 5(2):241–259, 1992. 118. X. Wu, B. Shi, Y. Dong, C. Huang, L. Faust, and N. V. Chawla. Restful: Resolution-aware forecasting of behavioral time series data. In Proceedings of the 27th ACM International Conference on Information and Knowledge Management, CIKM ’18, page 1073–1082, 2018. 119. A. Yang, P. M. Esperança, and F. M. Carlucci. Nas evaluation is frustratingly hard. arXiv preprint arXiv:1912.12522, 2019. 

120. C. Yang, Y. Akimoto, D.W. Kim, and M. Udell. Oboe: Collaborative fltering for automl model selection. In Proceedings of the 25th ACM SIGKDD international conference on knowledge discovery & data mining, pages 1173–1183, 2019. 

121. Q. Yao, M. Wang, H. J. Escalante, I. Guyon, Y. Hu, Y. Li, W. Tu, Q. Yang, and Y. Yu. Taking human out of learning applications: A survey on automated machine learning. CoRR, abs/1810.13306, 2018. 

122. C.-C. M. Yeh, Y. Zhu, L. Ulanova, N. Begum, Y. Ding, H. A. Dau, D. F. Silva, A. Mueen, and E. Keogh. Matrix profle i: all pairs similarity joins for time series: a unifying view that includes motifs, discords and shapelets. In 2016 IEEE 16th international conference on data mining (ICDM), pages 1317–1322. Ieee, 2016. 

123. A. Zela, A. Klein, S. Falkner, and F. Hutter. Towards automated deep learning: Efcient joint neural architecture and hyperparameter search. arXiv preprint arXiv:1807.06906, 2018.

1 Automated Machine Learning 25 

124. D. Zha, K.-H. Lai, M. Wan, and X. Hu. Meta-aad: Active anomaly detection with deep reinforcement learning. In 2020 IEEE International Conference on Data Mining (ICDM), pages 771–780. IEEE, 2020. 

125. Y. Zhao, R. A. Rossi, and L. Akoglu. Automating outlier detection via meta-learning. arXiv preprint arXiv:2009.10606, 2020. 

126. M.-A. Zöller and M. F. Huber. Benchmark and survey of automated machine learning frameworks. Journal of artifcial intelligence research, 70:409–472, 2021. 127. B. Zoph and Q. V. Le. Neural architecture search with reinforcement learning. In 5th International Conference on Learning Representations, ICLR 2017, Toulon, France, April 24- 26, 2017, Conference Track Proceedings, 2017. 

128. B. Zoph, V. Vasudevan, J. Shlens, and Q. V. Le. Learning transferable architectures for scalable image recognition. In Proceedings of the IEEE conference on computer vision and pattern recognition, pages 8697–8710, 2018. 

Open Access This chapter is licensed under the terms of the Creative Commons Attribution 4.0  International License (http://creativecommons.org/licenses/by/4.0/), which permits use, sharing, adaptation,  distribution and reproduction in any medium or format, as long as you give appropriate credit to the  original author(s) and the source, provide a link to the Creative Commons license and indicate if  changes were made.  

The images or other third party material in this chapter are included in the chapter’s Creative Commons license, unless indicated otherwise in a credit line to the material. If material is not included in the chapter’s Creative Commons license and your intended use is not permitted by statutory regulation  or exceeds the permitted use, you will need to obtain permission directly from the copyright holder. 

Chapter 2 

Sequence-based Learning 

Christofer Loefer1,2, Felix Ott2, Jonathan Ott2, Maximilian P. Oppelt2, Tobias Feigl2 

Abstract Learning from time series data is an essential component in the AI landscape given the ubiquitous time-dependent data in real-world applications. To motivate the necessity of learning from time series data, we frst introduce diferent applications, data sources, and properties. These can be as diverse as irregular and (non-)continuous time series data as well as streaming and spatio-temporal data. To introduce the mechanics of learning from time series data, we elaborate on the most renowned convolutional, recurrent and transformer architectures for learning from time series. Then, we discuss essential characteristics of learning with time series. Therefore, we explain deep metric learning, which learns feature representations that capture the similarity between time series data. We further describe time series simi larity learning to extract representations that allow comparison between sequences of spatio-temporal data. In addition, we discuss the interpretability of learning methods on time series data that target safety, non-discrimination, and fairness. 

Key words: Time series data, classifcation, regression, forecasting, spatio-temporal networks, deep metric learning, time series similarity, model interpretability 

2.1 Introduction 

As humans, we live in a world where (any kind of) events and interactions occur in a specifc causal order. For instance, when we talk to other people, words form sentences, and sentences form stories. When we walk, run or drive, our position in space changes depending on our current position and the change over time. 

1Escuela de Ingeniería Informática, Pontifcia Universidad Católica de Valparaíso, Valparaíso, Chile 2Fraunhofer Institute for Integrated Circuits IIS, Fraunhofer IIS, Nuremberg, Germany 

Corresponding author: Tobias Feigl 

e-mail: tobias.feigl@iis.fraunhofer.de 

© The Author(s) 2024 27 C. Mutschler et al. (eds.), Unlocking Artificial Intelligence,  

https://doi.org/10.1007/978-3-031-64832-8_2    

28 

Christofer Loefer et al.  

During physical exercise, our heart and breathing rates increase depending on the level of exertion. Even during mental stress or cognitive load, the conductivity of our skin, the variability of our heart rate, or the movement patterns of our pupils may change over time [44]. If all these sequential changes and past, current, and future observations were recorded, their data points would not be independent and identically distributed anymore, a fundamental statistical assumption that simplifes the application of machine learning. Thus, suitable learning paradigms would require specialized methods for handling such time series. 

Hence, time series analysis describes patterns that occur over time. Research on this topic has gained momentum in recent years as sensor data streams become ubiquitously available. Many applications in health [44, 42], industry [39], educa tion [49, 48] or entertainment [24, 40] process high-dimensional time series and raise new and interesting challenges for classical methods. Here, the tasks of clas sifcation, regression, forecasting or anomaly detection of sequential events (time series) are particularly noteworthy, as they contribute important information with real-world impact [59]. Historically, methods like autoregressive integrated moving average (ARIMA) [9] or the vector autoregressive (VAR) model [9] analyze lower dimensional time series based on the principle of automatic regression. However, complex multivariate time series (MTS) with correlated random variables that are typical for signal processing or economics applications, pose an impossible challenge for such classic statistical approaches. By contrast, modern methods based on deep learning (DL) have demonstrated remarkable performance, especially with complex, high-dimensional data. They model natural stochastic noise to reduce the informa tion complexity and can directly predict tasks. Alternatively, they can be combined with, e.g., Bayesian methods, to form more robust hybrid models [23]. The family of DL models for time series data include recurrent neural networks (RNNs) [21] or temporal convolutional networks (TCNs) [3] and are considered revolutionary [29]. Such models can, e.g., automatically learn time dependencies or handle temporal structures such as trends and seasonality directly from the data. Furthermore, they can extract patterns over very long periods of time and largely eliminate the need for manual feature engineering, data scaling and stationary data. Thereby, they provide more abstract, high-level features for downstream tasks. This holds even if the MTS is irregular or complex [49]. 

Throughout this chapter, we use the following notation from [46] to describe an MTS X = {x1, . . . , x� } ∈ R�× �, which is an ordered sequence of � ∈ N channels. Each channel x� = (��,1, . . . , ��, �), where � ∈ {1, . . . , �}, represents a series of observations with � ∈ N being the length of the time series. The training and test sets for MTS are a subset of the array X = {X1, . . . , X�} ∈ R�×�× �, where � represents the number of time series. We extend our annotation system for the classifcation task. We pre-defne a label set Θ that contains � classes and that is associated with a label �. The objective of this task is to determine the unknown class label � ∈ Θ for a given MTS. The training labels L = {l1, . . . , l�} ∈ Θ�×� correspond to the training MTS set X. Supervised sequential problems are formulated using input-label pairs {x�, y� }. 

2 Sequence-based Learning 29 

The rest of this chapter is structured as follows. Section 2.2 introduces time series processing using examples and explains the typical processing pipeline. Sec tion 2.3 then introduces the principles of the popular convolutional and recurrent architectures. Section 2.4 provides a concise review of the two important perspec tives of metric learning and model interpretability for time series analysis. Finally, Section 2.5 concludes and gives an outlook. 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdKBhDHLlQsFg0jb0rc3osSRONb6bv_W2FUwl2D2RM2jG-y0cEZ-kCn7L1DdJRS_jVp2efitW-XjhFsSsIStehvGpviS0CpvVoR6J67bb3hXekYFpKsHpS36yv_uEWHaq05Vh3lVA?key=skTJliiOFdw0rGxL_HdaM5-J)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdakbntq4wLxY2ihGoRoMk6YoQIfDgTpuCtH81kh61uJq4d9FjGHOL4vifdd2vjshu_Ku8nIrzhhhHOAaEAuMPN6GHqtAB5hMpZYUyIf3MOQ1SVwyyJkyYKRP4Rgf7MnhANFqxd?key=skTJliiOFdw0rGxL_HdaM5-J)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdVw2imjztITmfVoS0pS0BE4msVuT_5Uf2abAUuTEukK2bPqrDRrTywmP2ueHvPJoYC-GfgD9LezEopUxwr-tJkvym7--kf3psyuhit81D97XYGXIaomnQE7YqL8jWpNrf6VePojg?key=skTJliiOFdw0rGxL_HdaM5-J)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXfz3dbWJ6nh8buQejOS_xoATRnY1ez-jbWjXCufNv-FnRhvhElkzyqPe9JYEFGE-0V6LgTlc1FvY0wEi_jWONK0tlKkPusIhpBTfU6gfKDXGll43dZosdwBvpoEbqo957bD9uziiQ?key=skTJliiOFdw0rGxL_HdaM5-J)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXeQmxq9vfuTJMx7UXgFgo2tF-b2wg9tvNrKx88kle73TIUohlCPoFuuxZV94ol0AmbqXt9gqWaHxxagnUToIt_hOREFFxjvO3389uBBOOhNGI04jbtDYfFhh37mvg0OWsVutw3M?key=skTJliiOFdw0rGxL_HdaM5-J)![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXdPfKshT8fkf9Y8x52d-iKfN0cz8w1tF6gFr5wyYFwHivkiX488hQ2ktpnAzGjObmbqJKTV0ePGDWFMNki-A2FDc8eFKkF5BshTVyg1VyzPsZkmlbNSapkW3p5bfUg9-NJ0PQZCmQ?key=skTJliiOFdw0rGxL_HdaM5-J)  

(a) Driver state detection us ing sequential data from multi ple modalities: (1) electrophys iological signals, (2) facial ex pression from videos and (3) eye tracker data. (from [44], li censed under CC-BY 4.0) 

(b) Hand-held tool measuring inertial motion, magnetic feld and sound for quality assur ances. 

(c) Sensor augmented pencil measures 7 degrees of freedom: accelerometer, gyroscope, and pressure.   

Fig. 2.1: Applications for time series analysis are diverse. (a) The measurement setup depicted here is used to analyse cognitive load in a road driving secenario. (b) Qual ity assurance can be supported by sensor-augmented smart tools. (c) Handwriting recognition can be implemented via a sensor-augmented pen. 

2.2 Time Series Processing 

This section focuses on the signal-processing perspective of time series analysis, which fnds applications in a large variety of real-world use-cases [42, 39, 49, 48, 24, 40]. We consider the type of mining of time series data, that analyzes the shape of data sequentially sampled over time [22]. In contrast to sample-wise prediction, time series are captured over time and thus the samples are generally not identically and independently distributed [11]. Models may exploit that values in sequences may be correlated [11].  

30 

Application  

(example) 

Input Data streams  (sources) 

Pre-processing 

Christofer Loefer et al.

Prediction Post processing 

experianc 

„experianc“ „experience“ 

Synchronization Normalization Windowing 

Augmentation 

Feature  

Extraction 

Regression Forecasting Classification 

„x=5.0, y=1.5“ 

„x=7.5, y=1.5“ 

„experianc“🡪„experience“ 

Error  

propagation Uncertainty 

Outlier  

detection Smoothing   

User input 

Reference label   

Fig. 2.2: Time series processing pipeline. Data fow from the left to the right. 

We show the diferent characteristics of time series processing via exemplary tasks of domain-specifc signal-processing in Figure 2.1. First, Figure 2.1a shows a recording of biosignals, video and eye tracking data used for detecting the cognitive load of drivers [44]. Here, biosignals may show only short-term signal deformations and only a combination of sensors allows the detection of long-term variations [45]. In contrast, the application in Figure 2.1b classifes the activity of hand-held tools from shorter patterns in the sensors’ signal amplitude. The fnal application example in Figure 2.1c shows a combination of both characteristics. It predicts letters, words and whole sentences from spatio-temporal sensor data recorded using a smart pencil. Still, all applications have their ML pipeline in common. Figure 2.2 presents the peculiarities, that distinguish the pipeline for time series from other forms of data. The seasonality of time series data can be identifed in the orange curve, outliers in the blue curve, and autocorrelation between the orange and blue curves of the data streams. 

2.2.1 Time Series Data Streams 

For time series processing, a complete description of the data format is fundamental. The input data may be a continuous stream of several multi-dimensional sensors, for example, a writer’s force of pressure and a pen’s accelerations, or a hand-held tool’s vibrations. Time series data may be multi-variate, recorded at diferent sampling rates and levels of noise, and have gaps or other issues. Common sensors measure inertial motion, sound or radio frequencies. 

Figure 2.3 explains the data type’s characteristics using a simplifed sample of an inertial measurement unit (IMU) of the activity recognition application from Fig 2.1b. These properties diferentiate them from other types of data. Similarly to the augmented pen, the hand-held tool’s IMU collects signals from accelerome ters, gyroscopes, and a magnetic feld sensor. The sensors sample data along three orthogonal axes. We only show one axis of each. 

A recorded sensor data stream may be sampled at diferent sampling rates, see Figure 2.3 for a higher and lower rate. This has practical implications on the ob 

2 Sequence-based Learning 31 gap gap 

Fig. 2.3: Inertial measurements showing accelerometer and gyroscope data.Windows are shown as dashed rectangles. A window represents an application-specifc (pre- )selected set of data samples over time, which are processed by a learning algorithm at each inference step. Typically, sliding windows are applied with a specifc window length, which overlap at a specifc ofset and scroll over the data sequence. The top fgure presents two possible types of data loss: (1) complete loss and (2) partial loss of sensor data. The middle fgure presents two non-overlapping windows and the bottom fgure presents two overlapping windows. 

servability of phenomena, comparable to the diference in low and a high-resolution photography in computer vision tasks. However, it also entails similar costs and complexity. A higher sampling rate allows handwriting recognition algorithms to detect smaller movements of the writer and thus may lead to enhanced recognition, but also requires more processing power. 

A second dimension that infuences the density of data per unit of time is the di mensionality of the sensor streams. It can feature more dimensions and is analogous to the diference of monochrome and color photography. We simplify the visual ization of the recorded data and show only three of the nine recorded dimensions.  

32 

Christofer Loefer et al.  

However, for some applications it can be very valuable to add additional views to enable predictions for its use-case, such as the force sensor to detect the contact between a digital pen and the writing surface [49]. 

2.2.2 Pre-Processing 

Next, the pre-processing step for time series data of multiple sensors can require a synchronization of the data that may be streamed from separate sensors. In addition, raw sensory data can require normalization before any operations such as windowing, augmenting or even feature extraction can take place. Popular libraries for feature extraction and other time series specifc tasks, such asseglearn [12], are able to extract generic features like the "mean" for downstream usage. However, Deep Learning methods may not need such engineering eforts. 

We show the efects of generating windows in Figure 2.3. ML models may ingest a continuous stream of samples or subdivide the time series into windows of diferent sizes and with diferent fractions of overlap between each other. In contrast to sliding windows, which we show with approximately 50% overlap, tumbling windows have no overlap with each other. It depends on the model what approach is available, e.g., TCNs process fx-sized windows (see Section 2.3.1) and RNNs can process a sample at a time while memorizing the history internally (see Section 2.3.2). Furthermore, it may be crucial that window-based sampling captures all relevant features and does not cut of those that provide the relevant information to perform predictions. 

A common problem of time series processing is missing data, e.g., the complete loss of all sensor axes or only a partial loss of one sensor. A complete loss of data may not only occur in case of system defects, but could happen if a sensor edge device with little on-board memory is disconnected from processing in a cloud for a prolonged amount of time or its perception could be obscured. Some partial loss may be recovered from orthogonal sensors such as the gyroscope, and forecasting models may use additional information such as trends or seasonality efects to recover from imputed or missing data. 

2.2.3 Predictive Modelling 

In the main processing step, the models may perform predictions for diferent tasks based on extracted features or the data itself. For example, a decision tree classifer may classify the state of the pen for a windowed sub-sequence of input data based on the mean value of the force sensor as "writing". Upon ingesting character-level features, a forecasting model could predict the next character, e.g., after seeing the sequence "experienc_", the model could predict the next character to be an "e". A regression model could process the acceleration and rotation data of an inertial 

2 Sequence-based Learning 33 

measurement unit in order to predict the pen’s motion over the paper and help reconstruct its trajectory. 

2.2.4 Post-Processing 

A complete ML pipeline requires post-processing of the results for robustness. Post-processing of time series data involves applying additional techniques or trans formations to the data after initial analysis or modeling to improve its quality or inter pretability. This contains smoothing, fltering, resampling, detrending, diferencing, seasonal adjustment, denoising, scaling, and feature engineering. Some models, such as softmax-based classifcation, output their predictive uncertainty besides the predictions themselves. These likelihoods, together with prediction errors or the detection of outlier samples may be propagated to downstream processing logic or reported for review. 

2.3 Methods 

Time series analysis includes methods for performing inferences from time series data to predict statistical features and other abstract characteristics such as future developments. The assumption is that the current values of one or more dependent time series infuence the current value of another time series [58]. As time series data have a natural temporal order, stochastic regression models assume that observations that are close in time are more closely related than the ones that are further apart. In addition, stochastic regression models assume that observations of a certain period depend on past ones and that future values can be predicted solely from past observations [58]. This section presents TCNs in Section 2.3.1 and RNNs in Section 2.3.2. 

2.3.1 Temporal Convolutional Networks 

Feed forward neural networks (FFNNs) are nonlinear mappings, where each input is mapped to an output node by matrix multiplication. Although these networks are theoretically capable of learning any function, they lack this in practical terms due to their computational inefciency, as they require matrix multiplication for every input sample to each output sample. While these FFNNs can process time series data when the time dimension is fattened and a sequence represents the complete time series, this has signifcant disadvantages. FFNNs are not adaptable for sequences of arbitrary length [21]. Since the architecture only works with complete sequences, the entire relevant history must always be saved. Also, FFNNs are not computationally  

34 

Christofer Loefer et al. 

Output 

Dilation 4

Hidden 2 

Dilation 2 

Hidden 1 

Dilation 1 

Input   

Fig. 2.4: The structure of a temporal convolutional network (TCN) consists of layers of dilated causal convolutions. Each output learns over a large input window of past time steps. 

efcient when the sequence is a rolling window or when prediction is required at each time step, since the network then has to process the entire input sequence at each time step [21]. Since FFNNs have no inherent concept of time, time-delayed input sequences deliver completely diferent results [21]. Recall the example of cognitive load detection from Figure 2.1a. There it is essential to take the subjects’ past features to predict their present cognitive load. However, these biological readings are highly individual and the sequences of psycho-physiological data are very long. Therefore, FFNNs become infeasible. 

As a simple but efective network architecture, TCNs [3] are based on convolu tional operations and learn using a hierarchical representation of the time steps over several levels. Figure 2.4 shows this temporal structure, that uses dilation to create a sparse receptive feld for the output units, covering the whole fxed time sequence. With every layer, the receptive feld of the output neurons grows. This way, TCNs can process very long sequences. Due to their simple structure, TCNs can be op timized in parallel. They are much more resource-efcient than RNNs and enable efcient training for very large amounts of data if the time series are short and have a fxed, predefned length. However, during inference, the feed-forward structure of the TCNs requires expensive calculations of the entire history of the time series instead of only one sample at a time. As the sequence length increases, the breadth and depth of the architecture increases, and the sequence length cannot be changed. This makes it difcult to perform the calculations on resource-constrained embedded hardware. In contrast, RNNs [21, 27] compress the history into a fxed-size representation that requires minimal computation at each time step. 

2.3.2 Recurrent Neural Networks 

RNNs were proposed by Elman et al. [21] in 1990 and difer from FFNNs as they employ a special type of neural layer called a recurrent layer that allows the network to maintain state between layers of the network. This recurrent layer is a hidden 

2 Sequence-based Learning 35 

state vector and memory to store information about the past and current context. This hidden state is computed by the network at each time step and then fed back as input for the next time step. The network uses the hidden state to convert the relevant features from the input history into a more compact representation. This allows efcient computation of the output at each time step � and a representation limited only by the size of the hidden state vector. The assumption is that the model has a state and transition function that computes subsequent states from its predecessor and any model input. Therefore, RNNs are suitable for the processing of time series data [10]. 

y 

h 

RNN 

x 

Fig. 2.5: Simplifed representation of the basic structure of a RNN. RNNs are an adapted form of FFNNs that adopt a hidden state vector ℎ, a kind of memory, to store information � about the history and the current context. ℎ is computed at each time step and then passed as input for the next time step. The mesh uses ℎ to compress relevant features from the input history. This allows efcient computation of the output �, limited only by the size of ℎ. 

In an RNN, all neurons have both incoming connections, which emanate from all neurons of the previous layer, and outgoing connections, which lead to all neurons of the subsequent layer. In contrast to FFNNs, RNNs also have recurring connections in the recurrent layer, which pass on information between the neurons of the same layer, including the same neuron of a layer. A recurrent layer with � neurons has a total of �2recurrent connections [10]. 

With RNNs the lifetime of the network entity can be divided into discrete time steps. At each time step, the model is supplied with the next input sample. The feed-forward connections in an RNN represent the fow of information from one neuron to the next, with the transmitted data representing the computed neuronal activation of the current time step. Figure 2.6 represents the information fow of recurrent connections, where the data shows the stored neural activation from the previous time step, i.e., infuence from the left and from below. Thus, the activations of the neurons in an RNN represent the accumulating state of the network entity. The initial activations of the neurons in the recurrent layer are parameters of the model. When training RNNs, the optimal weights � are sought to approximate the network output � to the training target �ˆ, i.e., to minimize the error �. With a fxed lifetime, such as � time steps, an RNN instance can be represented as a unrolled irregularly structured FFNN. [10]  

36 

yt 

yt+1 

yt+2 

Christofer Loefer et al.yt+3   

ht-1 

x1 

ht 

tanh 

ht+1 

tanh 

x2 

tanh 

x3 

ht+2 

x4 

ht+3 

tanh   

Fig. 2.6: Simplifed representation of the fow of information through an unrolled RNN, resembles a FFNN. Forward pass: processing a series of inputs �1 to �4. A simplifed version of the cells is shown for a better overview. 

Vanishing and exploding gradients. To determine the gradient for a longer-term dependency, backpropagation through time (BPTT) is carried out several times. This optimization method "unfolds" the recurrent network’s temporal steps into copies of itself and then propagates the gradients back along the network "through time". This may lead to exploding or vanishing gradients for large sequences [5]. Both of these problems prevent learning weight matrices for long-term dependencies as the weight updates are based on this gradient information. Various methods are proposed to overcome these problems [4, 27, 70]. 

The long-short-term memory (LSTM) proposed by Hochreiter and Schmidhu ber [27] in 1997 uses a diferent cell design, developed to account for long-term dependencies and the problems of vanishing and exploding gradients. The LSTM cell uses structures called gates to manipulate and control the fow of the hidden state and is designed in such a way that useful information is efectively preserved in the memory cell over many time steps [10]. In contrast to the RNN, the LSTM cell structure enables a separation between this cell and the initial state. This sepa ration and the fact that the cell state is not directly afected by a nonlinear activation function reduces the vanishing gradients. 

2.3.3 Transformer 

A drawback of training recurrent networks with BPTT is that its graph cannot be parallelized during training and inference. Due to this, RNNs sufer from a compu tational complexity that cannot be optimized by parallelizing gradient operations on modern GPUs. Recent techniques such as Transformers use the so-called attention mechanism and combine the strenghts of FFNNs, i.e., extraction of characteristic features, and of RNNs, i.e., memory of causal relationships over long periods of time. Transformers are also used in AI frameworks such as ChatGPT [50]. 

The transformer neural network introduced by Vaswani et al. [67] is an encoder decoder architecture. It computes representations of time series solely by making use of attention layers. Hence, it signifcantly reduces the training time, compared to RNNs, by reducing the need for sequential computation. The ability to resolve 

2 Sequence-based Learning 37 

relationships between two distant points depends, among others, on the path between the position in the output representation and the position in the input sequence [26]. The attention mechanism used in the transformer has comparatively short paths, resulting in an increased performance for particularly long sequences. However, this comes at the cost of computational complexity, which grows by�(�2) as the sequence length increases. Recent research focuses on optimizing the attention mechanism to wards efciency by either reducing the number of computations [68] or by optimizing memory access [16]. Furthermore, the architecture requires a large amount of train ing data due to its tendency to overft [69]. As the transformer employs neither convolutional nor recurrent layers, it is not capable to detect the order of elements in a sequence. Thus, a positional encoding is added to the time series embedding (see Figure 2.7), which can be fxed or learned [69]. While the transformer architecture was originally introduced in the context of sequence transduction, it has been applied to various time series tasks such as forecasting [74] or classifcation [73]. 

![](https://lh7-rt.googleusercontent.com/docsz/AD_4nXf7OXPyvvzh8prCUpNxNuEr4RPOucuZTlE9C18k20HlOZ8bsf-fEsTNbvtndak7GqCFlZP7dFxnle4uhsLSPPeq-76eKCQ4gTP6AW6AlsaWFyXdE6CSzAERYBW4va9SHHjPQ2U3rA?key=skTJliiOFdw0rGxL_HdaM5-J)

Fig. 2.7: Simplifed overview of Transformer architecture. Depicted are a single encoder and a single decoder block. Several operations are neglected to show the overall concept of the architecture. 

The type of attention blocks used in the transformer architecture is called multi head attention. It computes multiple representations of the input data, projected via learned transformations, in parallel. This allows to attend to multiple positions as well as subspaces in the data. The transformer employs two variants of multi-head attention: (1) self-attention and (2) encoder-decoder-attention. (1) self attention is  

38 

Christofer Loefer et al.  

the frst layer in the encoder and decoder blocks. It computes the representation of a sequence by modeling dependencies in the sequence itself. (2) the decoder uses encoder-decoder-attention to incorporate the context information provided by the encoder. Figure 2.7 depicts self-attention as a blue box and encoder-decoder attention as an orange box. The fnal layers in the encoder and decoder blocks are position-wise feed-forward networks that apply a fully connected layer that shares its weights for all positions but is only applied to the embedding per position in the sequence. All layers are bypassed by a residual connection [67]. 

2.4 Perspectives 

The practical use of DL models like the TCNs, RNNs or LSTMs for time series analysis may quickly run into difculties, which we explore in this perspectives section. First, many techniques require a similarity (or distance) metric defned on the input data space, e.g., on trajectory data. Hence, Section 2.4.1 describes suitable functions for distance computation. Alternatively, deep metric learning (DML) learns these functions directly from data (see Section 2.4.1.1). The common issue of domain shift that appears between training and test data sources afects machine learning in general. Hence, we summarize the specifc domain adaption (DA) techniques for time series applications in Section 2.4.2. Lastly, safety, non-discrimination and fairness, and explanations are important but still open questions [18]. Accordingly, Section 2.4.3 discusses interpretability methods and their limitations for black-box time series models. 

2.4.1 Time Series Similarity   

In many applications, the distance between two time series is a crucial measure to compare the discrepancy. See for example Figure 2.9 where the goal is to reconstruct a trajectory of the pen tip of the sensor-enhanced pen of Figure 2.2 by 

0.0 Ground truth 

Prediction 

Loss: 0.008690 

0.2 

0.4 

0.6 

0.8 

1.0 

0.0 0.1 0.2 0.3 0.4 0.5 

Loss: 0.043547 

2.0 Ground truth 

Prediction 

1.5 

1.0 

0.5 

0.0 

0.5 

1.0 

1.5 

2.0 

1.5 1.0 0.5 0.0 0.5   

minimizing the distance between the ground truth and predicted trajectories. The distance (inverse of similarity) between two time series is mea sured as the cost of transforming one time series 

Fig. 2.9: Ground truth (red) and reconstructed (blue) trajectories [47].   

into another using a distance measure or function. The existing similarity measures can be classifed into two classes (see Figure 2.8): (1) Spatial similarity that focuses on fnding time series with similar geometric shapes that ignore the temporal dimen sion, and (2) spatio-temporal similarity that takes into account both the spatial and the temporal dimensions of time series data [41, 33]. 

2 Sequence-based Learning 39 Similarity measures 

Spatial similarity Spatio-temporal similarity   

Spatial data similarity 

Euclidean distance 

Movement  

direction-based similarity 

Trajectory 

match 

Edit distance on movement pattern strings

Geometric shape-based similarity 

Spatial 

assembling distance 

Hausdorff and Fréchet distance 

Angular  

metric for shape 

similarity 

Time series-based similarity 

Time warped 

distance 

Edit distance 

Dynamic time  warping 

Edit distance on  real sequences 

Longest common subsequence 

Movement speed based similarity 

DTW-based 

approaches   

Fig. 2.8: Overview of spatial and spatio-temporal similarity measures [41]. 

It is well-established to use a sum-of-square-based objective function to measure the average diference between all samples of two time series. A challenge that arises is the possibility of a varying number of data points between two time series. Partial curve mapping (PCM) [72] utilizes a combination of sub time series length and area to measure the similarity between two time series. The performance of PCM is adversely afected by the presence of noise in the data, as the noise leads to an artifcial increase in the arc length. The Area method [28] constructs quadrilaterals between two time series and calculates the area for each quadrilateral. It is necessary for the two time series to have the same number of points. 

The discrete Fréchet (DF) [19] distance preserves the time series order of data along the series. The DF distance refects the shortest possible path between two time series. If we consider a series A with � number of points and a series B with � number of points, the DF distance has a fxed quadratic run time of �(��). However, the Fréchet distance is sensitive to outliers. In contrast, dynamic time warping (DTW) [6] measures the similarity between to time series with varying time steps. It aligns the two sequences by warping their respective time axes to fnd the optimal alignment that minimizes the distance between corresponding points. 

The Hausdorf distance (HD) [65] is a popular dissimilarity metric used to com pare sets of points. HD is a max-min distance, which ofers an advantage in that it accounts for the spatial position of each individual point. HD has nearly-linear com plexity. For a comparison of trajectory popular distances for handwriting recognition, see [47], and for certain sports trajectory data, see [56].   

40 

2.4.1.1 Deep Metric Learning 

Christofer Loefer et al.  

To learn an optimal representation between data samples or models, DML techniques are required to compare distances of feature embeddings. DML is a sub-feld of ML that aims to learn a function that maps inputs into a feature space, where distances between data points correspond to semantic similarities, e.g., the semantic similarity between two pieces of text or two scenes of football [35] measures how close their meanings are. DML methods learn a feature by minimizing a loss function that takes into account the distances between pairs of data points and their corresponding labels. The main challenge of DML for time series is the variable length of samples, which can make it challenging to apply DML methods that require fxed-length inputs. In the following, we summarize the most common DML functions. The Euclidean loss has been shown to be efective in many tasks. Another commonly used metric is cross-correlation, which measures the similarity between two signals by sliding one of the signals over the other and computing the dot product at each position. Recently well established is maximum mean discrepancy (MMD) [8] that measures the distance between two probability distributions. MMD is a non-parametric metric that is able to capture complex patterns in data distributions. MMD has been used in tasks such as Domain Adaption (DA) and image generation. Correlation alignment (CORAL) [63] and higher-order moment matching (HoMM) [14] align the higher order moments of the features of two data points. The idea is to match the distributions of the features of two data points. The Sinkhorn [15] distance is based on optimal transport theory. Sinkhorn has the advantage of being able to handle discrete and continuous data, and has been applied to time series classifcation in [20, 46]. 

2.4.2 Transfer Learning & Domain Adaptation   

target domain source domain 

target domain source domain   (aligned) 

Distributiontarget domain source domain 

Distributiontarget domain source domain  

 (aligned)   

Fig. 2.10: Alignment of the source and target domain distributions, 3� � (before alignment) and 4� ℎ (after alignment) plot, to align their representations, 1�� (before) and 2�� plot (after) (from [46], licensed under CC-BY 4.0). 

For many applications, a domain shift appears between training and test data sources, for instance, between sensor data of right-handed and left-handed writers of the application presented in Figure 2.2 [46]. Domain adaption is a sub-category of transfer learning that adapts a predictive model trained on a source domain to a 

2 Sequence-based Learning 41 

target domain where the distribution of the data may be diferent. The characteristics of the time series data may have changed between the source and target domains (training and application data distributions). Additionally, the distribution of the time series data may shift over time due to changes in the underlying system or changes in the measurement process. DA approaches use techniques that focus on aligning the distributions of the source and target domains and aim to learn a shared representation of the data that is invariant to the diferences between the domains (see Figure 2.10). The common issue of shifting distributions between training data and real-world application is especially challenging for time series data, because it often has complex temporal dependencies that must be captured by the model. 

The following methods to mitigate the domain shift between data sources of ten make use of DML metrics presented in Section 2.4.1.1. For example, the ap proach known as minimum discrepancy estimation for deep DA (MMDA) [51] employs the minimization of conditional entropy as a means of integrating MMD and CORAL alignment functions. Deep domain confusion (DDC) [66] is based on the minimization of the MMD distance between domains. The domain-adversarial NN (DANN) [25] utilizes a gradient reversal layer to encourage the emergence of features that are discriminative for the source domain but indiscriminative w.r.t. the shift between the source and target domains. Further methods are the ones proposed by [34, 37, 57, 71]. 

2.4.3 Model Interpretability 

Deep Learning can outperform human experts in certain domains. Still, there are additional criteria besides raw performance [18]: safety, non-discrimination and fairness, and legal requirements such as the right to explain.1 These criteria are hard to quantify and thus also difcult to optimize for. One way to explain the reasoning of a model and verify its predictions is to make it interpretable [18]. This is especially difcult for time series analysis due to its often unintuitive data compared to, e.g., image data. 

The literature diferentiates methods into three broad categories [13, 43]. "Pre model" interpretability inspects the data, "in-model" refers to "intrinsically" inter pretable models [52], and "post-model" methods interpret models after training. These post-model (or post hoc) methods [13, 43] are either "model-specifc" or "model-agnostic", and may be global, local [18, 13, 43] or in between [43]. A global interpretation may comprehend the entire model at once, whereas a local method explains a single prediction from a small region of interest. 

1 General Data Protection Regulation, Regulation (EU) 2016/679 of the European Parliament and of the Council of April 27�ℎ 2016, recital 71 https://eur-lex.europa.eu/legal-content/ EN/TXT/HTML/?uri=CELEX:32016R0679&from=EN#d1e40-1-1, see also Chapter 5 for a deeper discussion on the EU AI act.  

42 

2.4.3.1 Interpretability for Time Series 

Christofer Loefer et al.  

Local interpretability methods are popular because widely applicable to many DL architectures such as TCNs or RNNs, even without intrusive changes, and directly visualize the relevance of input features for a model’s prediction. We distinguish gradient-based methods, e.g., Gradient [60], Backpropagation [62], Integrated Gra dients [64], SmoothGrad [61] or GradCAM [55], and perturbation-based methods (model agnostic) methods like LIME [52], that fts an interpretable surrogate to explain black box models, and Kernel SHAP [38], that uses concepts from Shapley values. 

Extending these approaches to time series data builds on insights of Schlegel et al. [54], who propose that saliency methods may explain patterns that underlie the time series data itself, such as temporal correlations. Subsequent work specifes these ideas further. Kusters et al. [31] propose patterns for a conceptual explanation for model-agnostic interpretations, that manipulate input data using transformations of the data, similarly to TCAV [30] that use hypothesis tests of concepts. The time series specifc patterns include ofset or trend removal, a moving average, low or high pass flters, and additive noise, but experts may additionally design more advanced flters. Similarly, Abanda et al. [1] propose time-dependent perturbations using warp, scale, noise and slice operations for post hoc perturbation-based explanations to visualize the relevance of sub-sequences of the input data. For example, warping the duration of an activity in a dataset can have semantic meaning, e.g., it diferentiates the classes of pulling a gun from its holster from pointing a fnger in the GunPoint dataset [17]. Abanda et al. [1] show that the construction of semantic perturbations to create interpretations of models shows to be valid for simple time series datasets from the UCR repository [17]. Perturbing important regions changes the prediction of the models, whereas perturbing unimportant regions has a smaller efect. 

2.4.3.2 Trusting Interpretations 

Recent studies question the efectiveness of interpretations of time series models w.r.t. their reliability. Still, no evaluation of interpretations answers all the possible doubts [36, 64, 32, 7]. On one hand, qualitative metrics are more user-targeted, e.g., towards the general public. On the other hand, quantitative metrics provide deeper insights for experts [53]. Quantitative evaluation metrics forgo a human who performs a qualitative evaluation of an explanation and uses a proxy metric for evaluation [18]. The faithfulness metric is generally seen as a foundational evaluation concept, and it was adapted for time series data [2, 54], e.g., it may perturb temporally connected segments. Faithfulness changes inputs with high relevance w.r.t. saliency, and uses its infuence on the model prediction, i.e., its accuracy, as a proxy for an explanation’s correctness. A high score in faithfulness means that the saliency is representative of input features that correlate with the model’s predictive accuracy. Overall, the choice of visual interpretation methods for time series and the trust in their explanations 

2 Sequence-based Learning 43 

depends on many factors, e.g., the choice of models and the dataset, and there is no "silver bullet" interpretation method [32]. 

2.5 Conclusion and Outlook 

Time series analysis reaches all aspects of our lives, such as our health, the way we work or learn, or how we spend time with our families. Our contribution focuses on a small set of applications that process time-dependent data, and describes essential properties of commonalities in the data and its diferences compared to a generic machine learning processing pipeline. Additionally, we also described the three DL models Temporal Convolutional Network, Recurrent Neural Network, and Trans formers that are foundational for many other use-cases as well, and have contrasting benefts and drawbacks. In the remainder, we addressed common difculties in ap plied research. The topic of similarity functions informs many learning approaches, and Deep Metric Learning specializes this feld further. Finally, we discussed expla nation and interpretation methods for predictions of black-box time series models and whether these may be trusted, raising important questions for applied machine learning. 

In this chapter, we have presented an overview of learning from time series data, covering a variety of data sources and properties such as streaming and spatio temporal data. ML models are becoming increasingly adept at capturing complex temporal patterns, accommodating the intricacies of time series data such as sea sonality, trends, and irregularities. Here prominent examples are foundation models such as ChatGPT for natural language processing. With the increasing importance of time-dependent data, the discussed methods ofer a valuable foundation for fur ther exploration and implementation in various domains. With the advancements of sensor data, IoT devices, and high-frequency trading, the demand for improved time series forecasting, anomaly detection, and pattern recognition solutions is on the rise. Moreover, the integration of DL architectures, i.e., RNNs, CNNs, and Trans formers, enables the extraction of hierarchical features from sequential data, further enhancing the accuracy and scalability of time series analysis. 

Acknowledgments 

We would like to express our sincere gratitude to N. Beck, J. Deuschel, N. Lang Richter, D. Dzibela, B. M. Eskofer, A. Foltyn, R. Gruber, D. Hartmann, S. Kram, N. Lang, C. Mutschler, A. Porada, N. L. Raichur, L. Reeb, A. Richter, G. Röder, J. Schemm, J. Seitz, B. Sonnleitner, M. Stahlke, U. Wetzker, N. Witt and H. G. Zimmermann, for their valuable insights and expertise in the feld of learning from time series data.  

44 

References 

Christofer Loefer et al.  

1. A. Abanda, U. Mori, and J. Lozano. Ad-hoc explanation for time series classifcation. 252:109366. 

2. D. Alvarez-Melis and T. S. Jaakkola. On the robustness of interpretability methods. 3. S. Bai, J. Z. Kolter, and V. Koltun. An empirical evaluation of generic convolutional and recurrent networks for sequence modeling. arXiv:1803.01271, 2018. 

4. Y. Bengio, N. Boulanger-Lewandowski, and R. Pascanu. Advances in optimizing Recurrent networks. In Proc. Intl. Conf. Acoustics, Speech and Signal Processing, pages 8624–8628. Vancouver, Canada, 2013. 

5. Y. Bengio, P. Y. Simard, and P. Frasconi. Learning long-term dependencies with gradient descent is difcult. Trans. on Neural Networks, 5(2):157–166, 1994. 

6. D. J. Berndt and J. Cliford. Using Dynamic Time Warping to Find Patterns in Time Series. In Intl. Conf. on Knowledge Discovery and Data Mining, volume 359-370, July 1994. 7. A. Boggust, H. Suresh, H. Strobelt, J. V. Guttag, and A. Satyanarayan. Beyond Faithfulness: A Framework to Characterize and Compare Saliency Methods. 

8. K. M. Borgwardt, A. Gretton, M. J. Rasch, H.-P. Kriegel, B. Schölkopf, and A. J. Smola. Integrating Structured Biological Data by Kernel Maximum Mean Discrepancy. In Bioinfor matics, volume 22(14), pages e49–e57, July 2006. 

9. G. E. Box, G. M. Jenkins, G. C. Reinsel, and G. M. Ljung. Time series analysis: forecasting and control. John Wiley & Sons, 2015. 

10. N. Buduma and N. Locascio. Fundamentals of deep learning: designing next-generation machine intelligence algorithms. O’Reilly Media, 1st edition, 2017. 

11. D. M. Burns and C. M. Whyne. Seglearn: A python package for learning sequences and time series. (March), 2018. arXiv: 1803.08118. 

12. D. M. Burns and C. M. Whyne. Seglearn: A python package for learning sequences and time series. The Journal of Machine Learning Research, 19(1):3238–3244, 2018. 13. D. V. Carvalho, E. M. Pereira, and J. S. Cardoso. Machine learning interpretability: A survey on methods and metrics. 8(8):1–34. 

14. C. Chen, Z. Fu, Z. Chen, S. Jin, Z. Cheng, X. Jin, and X. sheng Hua. HoMM: Higher-Order Moment Matching for Unsupervised Domain Adaptation. In Proc. of the AAAI Conf. on Artifcial Intelligence (AAAI), volume 34(4), pages 3422–3429, Apr. 2020. 

15. N. Courty, R. Flamary, D. Tuia, and A. Rakotomamonjy. Optimal Transport for Domain Adaptation. In IEEE Trans. on Pattern Analysis and Machine Intelligence (TPAMI), volume 39(9), pages 1853–1865, Oct. 2016. 

16. T. Dao, D. Fu, S. Ermon, A. Rudra, and C. Ré. Flashattention: Fast and memory-efcient exact attention with io-awareness. Advances in Neural Information Processing Systems, 35:16344–16359, 2022. 

17. H. A. Dau, A. Bagnall, K. Kamgar, C.-C. M. Yeh, Y. Zhu, S. Gharghabi, C. A. Ratanama hatana, and E. Keogh. The UCR Time Series Archive. 

18. F. Doshi-Velez and B. Kim. Towards A Rigorous Science of Interpretable Machine Learning. 19. T. Eiter and H. Mannila. Computing Discrete Frechet Distance. May 1994. 20. E. Eldele, M. Ragab, Z. Chen, M. Wu, C. K. Kwoh, and X. Li. Label-efcient Time Series 

Representation Learning: A Review. In arXiv preprint arXiv:2302.06433, Feb. 2023. 21. J. L. Elman. Finding structure in time. Cognitive Science, 14(2):179–211, 1990. 22. P. Esling and C. Agon. Time-series data mining. ACM Computing Surveys, 45(1):1–34, Nov 2012. 

23. T. Feigl, S. Kram, P. Woller, R. H. Siddiqui, M. Philippsen, and C. Mutschler. Rnn-aided human velocity estimation from a single imu. Sensors, 20(13), 2020. 

24. T. Feigl, D. Roth, S. Gradl, M. Wirth, M. E. Latoschik, B. M. Eskofer, M. Philippsen, and C. Mutschler. Sick moves! motion parameters as indicators of simulator sickness. IEEE Transactions on Visualization and Computer Graphics, 25(11):3146–3157, Nov 2019. 

25. Y. Ganing, E. Ustinova, H. Ajakan, P. Germain, H. Larochelle, F. Laviolette, M. March, and V. Lempitsky. Domain-Adversarial Training of Neural Networks. In Journal of Machine Learning Research (JMLR), volume 17(59), pages 1–35, 2016. 

2 Sequence-based Learning 45 

26. S. Hochreiter, Y. Bengio, P. Frasconi, J. Schmidhuber, et al. Gradient fow in recurrent nets: the difculty of learning long-term dependencies, 2001. 

27. S. Hochreiter and J. Schmidhuber. Long short-term memory. Neural Computation, 9(8):1735– 1780, 1997. 

28. C. F. Jekel, G. Venter, M. P. Venter, N. Stander, and R. T. Haftka. Similarity Measures for Identifying Material Parameters from Hysteresis Loops using Inverse Analysis. In Intl. Journal of Material Forming, May 2018. 

29. A. Karpathy and L. Fei-Fei. Deep visual-semantic alignments for generating image descrip tions. In Proc. IEEE Conf. on Computer Vision and Pattern Recognition, pages 3128–3137, 2015. 

30. B. Kim, M. Wattenberg, J. Gilmer, C. Cai, J. Wexler, F. Viegas, and R. Sayres. Interpretability beyond feature attribution: Quantitative Testing with Concept Activation Vectors (TCAV). In 35th International Conference on Machine Learning, ICML 2018, volume 6, pages 4186– 4195. 

31. F. Kusters, P. Schichtel, S. Ahmed, and A. Dengel. Conceptual Explanations of Neural Network Prediction for Time Series. In 2020 International Joint Conference on Neural Networks (ĲCNN), pages 1–6. IEEE. 

32. X.-H. Li, Y. Shi, H. Li, W. Bai, C. C. Cao, and L. Chen. An Experimental Study of Quantitative Evaluations on Saliency Methods, volume 1. Association for Computing Machinery. 33. H. Liu and M. Schneider. Similarity Measurement of Moving Object Trajectories. In Intl. Workshop on GeoStreaming, pages 19–22, Nov. 2012. 

34. Q. Liu and H. Xe. Adversarial Spectral Kernel Matching for Unsupervised Time Series Domain Adaptation. In Proc. of the Intl. Joint Conf. on Artifcial Intelligence (ĲCAI), pages 2744–2750, 2021. 

35. C. Löfer, K. Fallah, S. Fenu, D. Zanca, B. Eskofer, C. J. Rozell, and C. Mutschler. Active learning of ordinal embeddings: A user study on football data. Transactions on Machine Learning Research, 2023. 

36. C. Löfer, W.-C. Lai, B. Eskofer, D. Zanca, L. Schmidt, and C. Mutschler. Don’t get me wrong: How to apply deep visual interpretations to time series. arXiv preprint arXiv:2203.07861, 2022. 

37. M. Long, Z. Cao, J. Wang, and M. I. Jordan. Conditional Adversarial Domain Adaptation. In Advances of Neural Information Processing Systems (NIPS), 2018. 

38. S. M. Lundberg and S.-I. Lee. A Unifed Approach to Interpreting Model Predictions. page 10. 39. C. Löfer, C. Nickel, C. Sobel, D. Dzibela, J. Braat, B. Gruhler, P. Woller, N. Witt, and C. Mutschler. Automated Quality Assurance for Hand-Held Tools via Embedded Classifca tion and AutoML, volume 2, page 532–535. 2021. 

40. C. Löfer, L. Reeb, D. Dzibela, R. Marzilger, N. Witt, B. M. Eskofer, and C. Mutschler. Deep siamese metric learning: A highly scalable approach to searching unordered sets of trajectories. ACM Transactions on Intelligent Systems and Technology, 13(1):1–23, Feb 2022. 

41. N. Magdy, M. A. Sakr, T. Mostafa, and K. El-Bahnasy. Review on Trajectory Similarity Measures. In Intl. Conf. on Intelligent Computing and Information Systems (ICICIS), 2015. 42. S. Meyer, T. Windisch, A. Perl, D. Dzibela, R. Marzilger, N. Witt, J. Benzler, G. Kirchner, T. Feigl, and C. Mutschler. Contact tracing with the exposure notifcation framework in the german corona-warn-app. In 2021 International Conference on Indoor Positioning and Indoor Navigation (IPIN), page 1–8, Lloret de Mar, Spain, Nov 2021. IEEE. 43. C. Molnar. Interpretable Machine Learning: A Guide for Making Black Box Models Explain able. 2 edition. 

44. M. P. Oppelt, A. Foltyn, J. Deuschel, N. R. Lang, N. Holzer, B. M. Eskofer, and S. H. Yang. ADABase: A Multimodal Dataset for Cognitive Load Estimation. 23(1):340. 45. M. P. Oppelt, M. Riehl, F. P. Kemeth, and J. Stefan. Combining Scatter Transform and Deep Neural Networks for Multilabel Electrocardiogram Signal Classifcation. In 2020 Computing in Cardiology, page 4. IEEE.  

46 

Christofer Loefer et al.  

46. F. Ott, D. Rügamer, L. Heublein, B. Bischl, and C. Mutschler. Domain Adaptation for Time-Series Classifcation to Mitigate Covariate Shift. In ACM Intl. Conf. on Multimedia (ACMMM), pages 5934–5943, Lisboa, Portugal, Oct. 2022. 

47. F. Ott, D. Rügamer, L. Heublein, B. Bischl, and C. Mutschler. Joint Classifcation and Trajectory Regression of Online Handwriting using a Multi-Task Learning Approach. In Winter Conf. for Applications on Computer Vision (WACV), pages 266–276, Waikoloa, HI, Jan. 2022. 

48. F. Ott, D. Rügamer, L. Heublein, T. Hamann, J. Barth, B. Bischl, and C. Mutschler. Bench marking Online Sequence-to-Sequence and Character-based Handwriting Recognition from IMU-Enhanced Pens. In Intl. Journal on Document Analysis and Recognition (ĲDAR), volume 25(12), page 385–414, Sept. 2022. 

49. F. Ott, M. Wehbi, T. Hamann, J. Barth, B. Eskofer, and C. Mutschler. The OnHW Dataset: On line Handwriting Recognition from IMU-Enhanced Ballpoint Pens with Machine Learning. In ACM on Interactive, Mobile, Wearable and Ubiquitous Technologies (IMWUT), volume 4(3), Cancún, Mexico, Sept. 2020. 

50. A. Radford, K. Narasimhan, T. Salimans, I. Sutskever, et al. Improving language understanding by generative pre-training. 2018. 

51. M. M. Rahman, C. Fookes, M. Baktashmotlagh, and S. Sridharan. On Minimum Discrepancy Estimation for Deep Domain Adaptation. In Domain Adaptation for Visual Understanding, Springer, Cham., Jan. 2020. 

52. M. T. Ribeiro, S. Singh, and C. Guestrin. "Why Should I Trust You?": Explaining the Predictions of Any Classifer. In Proceedings of the 22nd ACM SIGKDD International Conference on Knowledge Discovery and Data Mining, pages 1135–1144. ACM. 

53. T. Rojat, R. Puget, D. Filliat, J. Del Ser, R. Gelin, and N. Díaz-Rodríguez. Explainable Artifcial Intelligence (XAI) on TimeSeries Data: A Survey. 

54. U. Schlegel, H. Arnout, M. El-Assady, D. Oelke, and D. A. Keim. Towards a rigorous evaluation of XAI methods on time series. pages 4197–4201. 

55. R. R. Selvaraju, M. Cogswell, A. Das, R. Vedantam, D. Parikh, and D. Batra. Grad-CAM: Visual Explanations From Deep Networks via Gradient-Based Localization. pages 618–626. 56. L. Sha, P. Lucey, Y. Yue, P. Carr, C. Rohlf, and I. Matthews. Chalkboarding: A new spa tiotemporal query paradigm for sports play retrieval. In Proceedings of the 21st International Conference on Intelligent User Interfaces, pages 336–347, 2016. 

57. R. Shu, H. H. Bui, H. Narui, and S. Ermon. A DIRT-T Approach to Unsupervised Domain Adaptation. In Intl. Conf. on Learning Representations (ICLR), 2018. 

58. R. H. Shumway. Time series analysis and its applications: with R examples. Springer Science+Business Media, 2017. 

59. J. Siebert, J. Groß, and C. Schroth. A systematic review of python packages for time series analysis. (arXiv:2104.07406), Jun 2021. arXiv:2104.07406 [cs]. 

60. K. Simonyan, A. Vedaldi, and A. Zisserman. Deep Inside Convolutional Networks: Visual ising Image Classifcation Models and Saliency Maps. 

61. D. Smilkov, N. Thorat, B. Kim, F. Viégas, and M. Wattenberg. Smoothgrad: removing noise by adding noise. (arXiv:1706.03825), Jun 2017. arXiv:1706.03825 [cs, stat]. 62. J. T. Springenberg, A. Dosovitskiy, T. Brox, and M. Riedmiller. Striving for Simplicity: The All Convolutional Net. 

63. B. Sun, J. Feng, and K. Saenko. Correlation Alignment for Unsupervised Domain Adaptation. In arXiv preprint arXiv:1612.01939, Dec. 2016. 

64. M. Sundararajan, A. Taly, and Q. Yan. Axiomatic Attribution for Deep Networks. In PMLR, volume 70, page 10. 

65. A. A. Taha and A. Hanbury. An Efcient Algorithm for Calculatingthe Exact Hausdorf Distance. In Trans. on Pattern Analysis and Machine Intelligence (TPAMI), volume 37(11), Nov. 2015. 

66. E. Tzeng, J. Hofman, N. Zhang, K. Saenko, and T. Darrell. Deep Domain Confusion: Maximizing for Domain Invariance. In arXiv preprint arXiv:1412.3474, Dec. 2014. 

2 Sequence-based Learning 47 

67. A. Vaswani, N. Shazeer, N. Parmar, J. Uszkoreit, L. Jones, A. N. Gomez, Ł. Kaiser, and I. Polosukhin. Attention is all you need. Advances in neural information processing systems, 30, 2017. 

68. S. Wang, B. Z. Li, M. Khabsa, H. Fang, and H. Ma. Linformer: Self-attention with linear complexity. arXiv preprint arXiv:2006.04768, 2020. 

69. Q. Wen, T. Zhou, C. Zhang, W. Chen, Z. Ma, J. Yan, and L. Sun. Transformers in time series: A survey. arXiv preprint arXiv:2202.07125, 2022. 

70. R. J. Williams and J. Peng. An efcient gradient-based algorithm for on-line training of Recurrent network trajectories. Neural Computation, 2(4):490–501, 1990. 

71. G. Wilson, J. R. Doppa, and D. J. Cook. Multi-Source Deep Domain Adaptation with Weak Supervision for Time-Series Sensor Data. In Proc. of the ACM Intl. Conf. on Knowledge Discovery & Data Mining (SIGKDD), pages 1768–1778, Aug. 2020. 

72. K. Witowski and N. Stander. Parameter Identifcation of Hysteretic Models Using Partial Curve Mapping. In Intl. Conf. on Multidisciplinary Analysis and Optimization (ISSMO), Sept. 2012. 

73. C.-H. H. Yang, Y.-Y. Tsai, and P.-Y. Chen. Voice2series: Reprogramming acoustic models for time series classifcation. In International conference on machine learning, pages 11808– 11819. PMLR, 2021. 

74. T. Zhou, Z. Ma, Q. Wen, X. Wang, L. Sun, and R. Jin. Fedformer: Frequency enhanced decomposed transformer for long-term series forecasting. In International Conference on Machine Learning, pages 27268–27286. PMLR, 2022. 

Open Access This chapter is licensed under the terms of the Creative Commons Attribution 4.0  International License (http://creativecommons.org/licenses/by/4.0/), which permits use, sharing, adaptation,  distribution and reproduction in any medium or format, as long as you give appropriate credit to the  original author(s) and the source, provide a link to the Creative Commons license and indicate if  changes were made.  

The images or other third party material in this chapter are included in the chapter’s Creative Commons license, unless indicated otherwise in a credit line to the material. If material is not included in the chapter’s Creative Commons license and your intended use is not permitted by statutory regulation  or exceeds the permitted use, you will need to obtain permission directly from the copyright holder. 

Chapter 3 

Learning from Experience 

Christopher Mutschler1, Georgios Kontes1, Sebastian Rietsch1 

Abstract Reinforcement Learning (RL) is one of the branches of Machine Learning (ML) that aims to learn from the interaction with an environment. In contrast to ap proaches such as supervised or unsupervised learning, where data samples usually are assigned to a ground truth label (supervised learning) or where they follow some stationary distribution (unsupervised learning), in RL, the agent is learning in direct interaction with the environment. This also defnes what data is being collected as a result of which actions are being executed. The agent is hence learning from ex perience. While more traditionally, RL was focused purely on continuously arriving data, lately also approaches that resort to a given data pool of past environment in teractions have gained more and more interest. This chapter covers the basics of RL and discusses the latest research in interactive environments, learning with available data or knowledge, and challenges that arise from the actual deployment of agents to the real world. 

Key words: Reinforcement Learning, Markov Decision Processes, Exploration Exploitation, Model-based RL, Ofine RL, Safe RL. 

3.1 Introduction 

Sequential decision-making is a fundamental concept in artifcial intelligence (AI) [4], decision theory [41], and operations research (see Chapter 7). It involves making a sequence of decisions over time, where the outcome of each decision depends on previous decisions and afects future decisions. This type of decision 

1Fraunhofer Institute for Integrated Circuits IIS, Fraunhofer IIS, Nuremberg, Germany 

Corresponding author: Christopher Mutschler 

e-mail: christopher.mutschler@iis.fraunhofer.de 

© The Author(s) 2024 49 C. Mutschler et al. (eds.), Unlocking Artificial Intelligence,  

https://doi.org/10.1007/978-3-031-64832-8_3  

50 Christopher Mutschler et al. 

making is pervasive in many real-world applications, such as game playing [59], robotics [98], autonomous driving [82, 80], fnance [94], and healthcare [108]. Traditionally, the theory behind sequential decision making is studied across many disciplines, including engineering (optimizing control loops and minimizing costs), mathematics (simulating and optimizing stochastic processes), economics (e.g., in game theory is studied how people make decisions considering social, political and human sciences), psychology (theory of conditioning and behavior) and neuroscience (dopamine system and the study of how the brain makes decision). Computer science usually addresses sequential decision making within the feld of machine learning. At least traditionally, supervised and unsupervised ML work on statically available datasets (e.g., classifying objects, events, or classes, and fnding representations for hidden structures within the data). In contrast, reinforcement learning works with a trial-and-error scheme: (i) data is acquired using the interaction of a learning agent with its environment (i.e., the learning process itself enables the agent to draw data samples from the environment to continue training), (ii) there are no labels (i.e., feedback to the agent is only provided by means of reward), and (iii) the reward might arrive with a large delay and it is not obvious what the causal relationship between a sequence of actions and a received reward actually is (credit assignment problem). 

As we cannot provide a comprehensive view on the area of RL and sequential decision making, we try to limit ourselves to topics that are of utmost importance for the actual deployment and training of such systems in real world applications. Figure 3.1 proposes a motivation for this chapter (we will not cover topics such as model-free RL and digital twins as deeply). In order to make RL usable in practice, we have to consider that we cannot fully leverage the trial-and-error scheme that RL resorts to, as breakage and damages to material is often not a viable option. Hence, we will focus on how to leverage ofine data (e.g., available through hard-coded regulators that can be observed), model-based RL (which makes use of available physics-models that can and should be used to accelerate learning or that learn a physical approximation of the real world dynamics), and safe RL (to account for constraints that are given by the actual application). This chapter will not focus on the area of interpretability and explainabliltiy (although this is a fourth important factor), as there is a large overlap with the content presented in Chapter 5. 

3.2 Concepts of Reinforcement Learning 

3.2.1 Markov Decision Processes (MDPs) 

The general sequential decision-making framework can be modeled as a Markov de cision process (MDP). An MDP is formally defned as a six-tuple (S, A, �, �, �, �0), where S defnes a set of states the agent may visit, A defnes a (fxed) set of actions the agent may take during an interaction, � is a transition probability matrix that defnes how likely it is for the agent to move between two states given a particular

3 Learning from Experience 51 (to train it with data from reality) Model-free RL   

Offline RL 

Real World RL 

digital twin   

SafeRL Model-based RL to make it work in reality 

(as the real world poses constraints) (to learn with models of reality) 

Fig. 3.1: The perspective that we will focus on in this chapter: (1) leverarging ofine data, (2) using available information in form of models, and (3) accounting for unpredictable and uninterpretable behaviour through SafeRL. 

action has been executed, � is a reward function, � is a discount factor that allows to under-weigh future rewards over immediate rewards, and �0 is a distribution over the states that defne the starting state of the agent. 

Time evolves in discrete time steps. At each time step �, the agent observes the current state �� (or receives an observation �� from the environment), receives a reward �� and then selects an action �� according to a policy � : S ↦→ A, which is a function that maps states to actions. The action modifes the environment and changes its state (given some probability, induced by a random variable P defned over �). The goal of reinforcement learning is to learn an optimal policy �∗that maximizes the expected cumulative reward over a fnite or infnite time horizon:   

�∗ = argmax � 

∑∞ �=0 

E 

��∼� ��+1∼P 

 �� �(��, ��)|�0 = � (3.1)   

3.2.2 Dynamic Programming 

A common way to solve MDPs is dynamic programming (DP). DP computes the optimal state-value function ��(�) (defning the value of being in state �, i.e., the (discounted) reward the agent can expect upon being in state � and following its policy), the optimal state-action-value function ��(�, �)1 (defning the value of being in state � and taking action �, i.e., the (discounted) reward the agent can expect upon being in state �, taking action �, and afterwards following its policy), or an (explicit) policy �. The value function represents the expected cumulative reward starting from a given state and following a given policy. The optimal policy is the 

1 While computing the state-action-value function � requires to estimate |S | × |A | values (instead of only | (�) | for the state-value-function ��(�), it is much more convenient to work with � in practice as it directly estimates the value of each action in a state. At the same time, for �, we also need to account for where an action � brings us in the environment.

52 Christopher Mutschler et al. 

one that maximizes the value function for each state. All such approaches recursively evaluate the Bellman equation. The Bellman equation sets up a system of equations that relates the values of all states to each other; for instance, the Bellman optimality equation, i.e., the Bellman equation for the optimal �-function, is given by:   

��(�, �) = �(�, �) + � ·∑ �′∈S 

P (�′|�, �) · max 

�′∈A��(�′, �′) (3.2)   

However, computing the value function exactly in practice is often infeasible using dynamic programming. First, large and complex MDPs (which we usually are con fronted with in practice) require estimating a large amount of state(-action) values recursively (several times). Second, DP is model-based and requires a model of the environment dynamics, the state transition probabilities P, which is usually not available in real-world applications. 

3.2.3 Model-free Reinforcement Learning 

A diferent approach to solving MDPs is through a (model-free) trial-and-error interaction with the environment. The basic idea is to directly use the experience samples that the agent receives from the environment and to apply an iterative approximative update of the �-function (for instance, using �-learning):   

h 

�(�, �) = �(�, �) + � · 

��(�′, �) − �(�, �)i, (3.3) � + � · max   

where �(�, �) is updated towards a target value using a small learning rate �. The state-action-value �(�, �) is again recursively described by the sum of the reward � that was recently observed and the maximal �-value that can be selected from the successive state the agent ends up in. Updating this function as the agent moves through the environment lets us (in the limit) approximate the optimal �-function. 

3.2.4 General Remarks 

Sampling complexity is the key performance indicator (KPI) to optimize. Com mon metrics to evaluate the performance of supervised or unsupervised ML algo rithms include, for instance, the number of epochs required to learn a model until convergence or the predictive accuracy of a trained model on the test data set. In RL, there is no explicit concept of a ground truth label. However, RL still follows an active learning strategy: the agent is not only tasked to build a model that represents the value function or the policy directly. In essence, the agent is also tasked to select the samples to learn from, i.e., through executing the actions that directly correlate to the samples the agent will observe and use for learning.

3 Learning from Experience 53 

The IID assumption. How the agent collects data and learns from it also infuences model training. A central assumption for training models with ML is violated, as data is not independent and identically distributed. First, data samples are not independent. The samples we receive and use to update our model using, e.g., Eq. 3.3 are highly correlated as they constitute and resemble the trajectories that the agent observes (sequentially). Second, training and test distribution are not identical.2 The distribution that underlies the data-generating process is constantly changing. Considering our central idea of the expected return from Eq. 3.1, the data we use within the expectation is based on actions we sample from � – but � is anything else than a stationary distribution as it is the central element we keep on training. 

The Deadly Triad. Training an RL agent is always prone to instability and diver gence, which arise from a combination of elements that make training diferent from other ML algorithms, see Sutton et al. [92]: 

• Function approximation: usually the number of elements we approximate using � or � is too large to ft into a computer’s main memory, so we approximate those functions using neural networks. Those approximators have an error in their approximation which multiplies within the estimation problem of � and � itself. 

• Bootstrapping: we update targets (e.g., in Eq. 3.3) that include existing estimates rather than relying exclusively on actual rewards and complete returns. In the limits, we hope for convergence of all the values. 

• Of-policy training: we train on the distribution of transitions that are diferent from that produced by the target policy. Sweeping through the state space and updating all states uniformly, as in dynamic programming, does not respect the target policy and is an example of of-policy training. 

3.3 Learning purely through Interaction 

3.3.1 Exploration-Exploitation 

The exploration-exploitation-tradeof [92] is one of the biggest challenges in RL. In its essence, it is a matter of deciding whether to exploit the knowledge that the agent has already obtained, i.e., to select actions from which we can expect high rewards/returns, or to explore the environment by selecting actions that have not or only rarely been selected to obtain potentially much higher rewards. Modern RL algorithms that optimize for the best returns can efciently achieve good exploitation, while exploration remains an open research topic. 

Classic exploration work builds on top of Multi-armed Bandits (MABs). The idea comes from a casino use-case where you face � diferent slot machines, and each of them is confgured with an unknown probability �� of how likely you 

2 Note, that while there are no explicit training and test datasets as in the usual ML setting, in RL, we model P a bit diferently between training and test environments.

54 Christopher Mutschler et al. 

can get a reward at one play (i.e., one-time step �). The question is: What is the best strategy to achieve the highest long-term rewards? This simple but efective problem formulation allows for a theoretical analysis of the exploration-exploitation-tradeof. More formally, with �(��) = E(�|�) = � being the expected reward of �� (i.e., the interaction with slot machine �) and �� = R (��), returning 1 with probability �� and 

0 otherwise, we want to maximize the cumulative reward Í��=0��.3 With the optimal reward probability given as �∗:   

�∗ = �(�∗) = max 

�∈A�(�) = max 

1≤�≤�E [��|�� = �] , (3.4)   

1≤�≤��� = max 

we can formulate the regret:   

L� = E 

∑� �=1 

( �∗ 

|{z} 1 

− �(��) |{z} 2 

) 

=∑ �∈A 

�� (�) | {z } 3 

Δ� 

|{z} 4 

, (3.5)   

where (1)is what the agent should have selected (i.e, the maximum rewarding action), (2) is what the agent actually selected at time �, (3) is the action selection counter, and (4) is the per-action regret. Good exploration algorithms minimize the total regret and maximize the cumulative rewards. 

3.3.1.1 Exploration Strategies 

As practical real world problems involve using deep RL (and its means to approximate large or continuous state and action spaces), we want to focus on exploration in deep RL. Hence, we only briefy cover classic work. Well-known exploration strategies are: 

�-greedy (and variants). This is a simple but often efective method: the agent exploits the knowledge, i.e., �� = arg max�∈A ��(�) with probability 1-� and occasionally selects a random action (with probability �).�-greedy with a constant � has a linear expected total regret. In practice, � is often set to a high value at the beginning and then is slowly annealed, resulting in a greedy agent (but the expected total remains linear). 

(Bayesian) Upper Confdence Bounds. The idea is to estimate the upper con fdence bound ��(�) such that with a high probability, we satisfy �(�) ≤ �ˆ�(�) + ��(�) and then select an action that maximizes the upper confdence bound: ���� 

� = arg max�∈A [��(�) + ��(�)]. �ˆ�(�) is where the average re wards associated with action � up to time � and ��(�) is a function reversely proportional to how many times action � has been taken. Hence, small ��(�) follow from big ��(�) and certain/accurate value estimates and vice versa. While originally, UCB1 [92] only counts the selections and rewards, Bayesian UCB [49] 

3 Note that this formulation (in contrast to any other work in RL) explicitly considers the rewards obtained over the course of training. It quantifes the training performance/progress.

3 Learning from Experience 55 

models ��(�) with a Beta-distribution [48] and hence makes use of confdence intervals. Both UCB1 and Bayesian UCB show logarithmic expected total regret. Probability Matching: Thompson Sampling (TS). TS [78] uses a Beta distribu tion to keep track of the current belief of probabilities and then directly samples from this distribution. Intuitively, highly rewarding actions become more likely to be sampled (while low rewarding actions still occasionally keep being selected), and the observed data is used to update the prior belief. Thompson sampling also shows logarithmic expected total regret while often being more efective than UCB and variants (while also being easier to be implemented). 

3.3.1.2 Exploration in Deep RL 

Exploration in Deep RL is more difcult than in small MDPs not only because the state space becomes larger. While exploration research on small MDPs as before can be theoretically well-grounded (we can, in principle, know the best strategy, defne the total regret and benchmark the algorithm, and defne upper and lower bounds on its mistakes), this is not possible when working with deep neural networks approximating the state and policy in deep RL. In addition to that, especially for more recent deep RL research, there are two descriptive problems on which exploration methods are being evaluated: (1) the hard-exploration problem and (2) the Noisy TV-problem. 

The hard exploration problem is presented in environments with very sparse or even deceptive rewards. In those environments, a random exploration is likely prone to failure as it will rarely fnd successful states or obtain meaningful feedback from the environment. One such example is Montezuma’s Revenge, where an agent traverses several rooms and looks for keys and treasures. The noisy-TV-problem [19] is a hypothetical scenario where a novelty-seeking agent solves a 3D-maze environment (in frst-person perspective) and encounters a TV that shows uncontrollable and unpredictable white noise – novelty-seeking agents usually then become a couch potato and keep looking at the TV forever. 

The key idea is that we count the number of times we visited a state or a state action-pair (instead of counting the number of arms in the bandit). In other words, we use �(�) (or �(�, �)) and add an exploration bonus to the reward that is provided by the environment: 

�+(�, �) = �(�, �) + � · B (�(�)), (3.6) 

where � is a hyperparameter that adjusts the balance between exploration and ex ploitation. Generally speaking, the frst component ��� = �(�, �) is often called the extrinsic reward (i.e., provided by the environment) and ��� = B (�(�)) is called the intrinsic reward (i.e., an exploration bonus added by the agent that decreases with larger �(�)). The intrinsic component rewards discovering novel states and, hence, possibly gaining knowledge about the environment. Recent research can be grouped into diferent categories: (1) Count-based Exploration, (2) Prediction-based Exploration, and (3) Memory-based Exploration.

56 Christopher Mutschler et al. 

(1) Count-based Exploration deals with the problem of counting states in high dimensional state spaces. Encountering the same state (e.g., in manipulation tasks) is unlikely, but some states are similar to others, and exactly this relationship should be represented in the bonus that is calculated. Density Models [13] approximate the fre quency of visits using a parametric model �(�; �) and derive a pseudo count from the model. As the agent observes new data, the density models are incrementally updated. As the density model only needs to correlate high density with large visitation counts (we do not need to sample from the model), we can resort to a large variety of models such as context switching trees [14, 13], PixelCNNs [65, 101], GMMs [112], etc. Another idea is to use hashing such as Locality-Sensitive Hashing (LSH) [95, 21]. The idea is to fnd or learn a hash function that maps the high-dimensional state space into lower-dimensional hash codes that preserve distance information between states, i.e., similar states will have similar hash codes. Simple distance metrics such as the angular distance work reasonably well for low-dimensional state spaces. For larger state spaces, LSH proposes to learn a compression using autoencoders with a regularized loss function that enforces a special representation in the bottleneck (i.e., the hash code). 

(2) Prediction-based Exploration follows the concept of curiosity and intrinsic motivation instead of just counting state visitations [79]. The key idea is to learn about the environment, e.g., its reward structure or dynamics. In the easiest case, the agent uses all the experiences (��, ��, ��+1) seen so far and learns a forward prediction model �� : (��, ��) ↦→ ��+1 and derives an extrinsic reward ���(��, ��) = || � (��, ��) − ��+1||22, i.e., large prediction errors result in a high bonus (i.e., a high intrinsic reward) and vice versa. While early approaches such as Intelligent Adaptive Curiosity (IAC) [66] resort to feature-engineering state representations, recent work such as Deep Predictive models [89] learn such forward dynamics models end-to-end using autoencoders. However, in many applications and environments, the observations change without being explicitly afected by the agent’s actions. Consider, for instance, a tree with leaves that move due to wind – such factors are not afected by the actions and cannot be controlled by the agent. Hence, those elements should not be encoded in the state space and not targeted to being predicted. The Intrinsic Curiosity Module (ICM) [68, 19] jointly learns an inverse dynamics model � : (�(��), (�(��+1))) ↦→ ��, where �(��) is a lower-dimensional embedding of the state observation, i.e., � enforces a bottleneck representation from which an action �� can be inferred, hence focusing on the crucial information contained in the state space. The forward prediction, the inverse dynamics models, and the policy are then jointly optimized. Self-Supervised Exploration via Disagreement [69] combines a policy network with an ensemble of neural networks (whose disagreement is the bonus) that predict forward predictions and learn all networks end-to-end (as���is diferentiable). However, for all previous approaches, the prediction errors still remain large if (i) the prediction target remains stochastic, or information is missing and (ii) if the model class or capacity of the predictor is too limited to ft the complexity of the target function [34]. Hence, Random Network Distillation (RND) [19, 18] predicts something diferent from the actual task using two neural networks: (1) a randomly initialized but fxed network � (��; �) that transforms a state into a feature space, and

3 Learning from Experience 57 

(2) a network ˆ� (��; �ˆ) that is trained to predict the same features as the frst network, i.e., ˆ� (��; �ˆ) = � (��; �); the exploration bonus is ��(��) = || ˆ� (��; �ˆ) − � (��; �||22. The intuition is that similar states have similar features, and if the agent has already seen them, it should also have a lower error in predicting them. RND makes the prediction target deterministic and ensures that the target is within the class of functions that can be represented. 

(3) Memory-based Exploration uses external memories to address a problem that remains present in previous approaches: the exploration bonus is non-stationary (i.e., it drops for a particular state when visiting it several times). As a result, intrinsic rewards will vanish and no longer provide a signal for the agent.4 Never Give Up (NGU) [9] combines an RND (for lifelong learning) with an episodic novelty module for rapid in-episode adaptation. Hence, visiting the same states within one episode is rapidly discouraged while revisiting states that have been visited many times across episodes is only slowly discouraged. Agent57 [8] enhances NGU using a population of policies (that all have their exploration parameters, encouraging exploration either more towards the beginning or the end of the training course) and using a separate estimation of �-values that decompose the infuence of the extrinsic and intrinsic rewards. Agent57 has been the frst general-purpose algorithm that outperforms the standard human benchmark on all 57 Atari games. While there are much more approaches in that area, methods such as Go-Explore [31] present a complementary solution. The idea is to especially address the detachment and derailment problems, i.e., that intrinsic rewards are consumed and vanish and that interesting states should be revisited, respectively. The idea is to use goal-conditioned policies through self imitation learning [32] or through a trajectory-conditioned policy based on a memory of demonstrations [37] that enable an agent to revisit a point (through a sequence of low-intrinsic rewards) to keep exploring other areas of the state space (e.g., keep exploring the tree at the end of the maze in the example before). 

3.4 Learning with Data or Knowledge 

3.4.1 Model-based RL with continuous Actions 

In Model-based RL (MBRL – sometimes also referred to as model-assisted rein forcement learning), the idea is to learn an estimator/model �� : S × A → S from data for the transition dynamics that would assist the search for the optimal policy. In several cases, a model of the reward can also be learned. Model training follows the supervised learning paradigm and utilizes standard loss functions such as MSE. The feld of MBRL is quite diverse [60], including diferent types of algorithms that 

4 Consider, e.g., long sequences within a maze where the agent traverses a tunnel where at the end, the agent might again take several diferent decisions/ways. However, the intrinsic rewards that lead the agent to enter the tunnel in the frst place will vanish, the agent will not enter the tunnel again, and the tree that spans up at the end of the tunnel remains mostly unexplored.

58 Christopher Mutschler et al.   

trained on 

Data 

storestrained on stores   

Model Agent   

Environment 

interacts with 

interacts with   

Fig. 3.2: The high-level concept of Model-based Reinforcement Learning 

operate in diferent representations of the state, like features [61], full observations like images [33] or event latent states [105, 39]). 

The way the learned model is used is also diverse. For example, algorithms like Dyna [91] or Model-based Policy Optimization (MBPO) [46] augment the real data (that is actually collected using the policy in the actual environment) with “imaginary” data (that is generated by running a model of the environment for several time steps from selected initial states). 

Other approaches use the model as a look-ahead approximator. Here, imaginary rollouts are performed from an initial state using the model, and either a policy is trained to select good actions or an open-loop optimization routine (called the planner) is utilized to generate a sequence of actions to be applied in the next time steps. Several types of planners can be used, spanning from well-established planners from control engineering practice like the iterative-linearization and trajectory opti mization iLQR planner [96], to population-based approaches that leverage modern parallel computation capabilities to iteratively simulate several trajectories using the model and select the most promising ones to be applied in the real system [106, 28]. 

One of the downsides of MBRL is that since the model is learned from data, it will always fail to capture the complexity of the environment perfectly. There will always be errors due to the uncertainty of the measurements and the underlying process/dynamics, as well as model extrapolation errors due to a lack of data. Modern MBRL algorithms try to alleviate this problem in two ways (often combined): 

• Online Re-planning: Following the paradigm of Model Predictive Control (MPC) [20], only the frst action of the action sequence generated by an open-loop planner is applied in the environment, and the planning process re-initiates from the new environment state. 

• Uncertainty Estimation: The idea is that probabilistic models can be utilized to capture both aleatory uncertainty, i.e., the uncertainty that is inevitable due to inherent noise in the process or measurements, and epistemic uncertainty due to the lack of training data in some regions of the state-action space. Here, as modeling errors can compound with longer rolling horizons, the uncertainty is

3 Learning from Experience 59 

propagated since the policy/planner that utilizes the model takes into account the model’s confdence of each next state prediction. Various models and policies have been utilized to achieve this, from analytical Gaussian Processes with end-to-end closed-loop policy learning [29] to ensembles of probabilistic neural networks with population-based online planners [24, 61]. 

MBRL algorithms have been utilized in a variety of tasks, often leading to impres sive results [61]. On one hand, one of their downsides is related to the complexity of the (uncertainty-informed) online planner, which could potentially hinder the real-time application. On the other hand, they ofer a way of safe exploration and operation [15, 42], as the model can prevent unsafe actions from execution. In con trast, the model’s uncertainty level in sampled states indicates that the model can be unreliable for prediction in these instances. 

3.4.2 MBRL with Discrete Actions: Monte Carlo Tree Search 

The availability of an environment model allows us to view many decision-making problems as a simple search problem over potential future trajectories. Generally speaking, it permits us to simulate the outcome of possible action sequences and, therefore, estimate the optimal value function by building a search tree. Considering a problem with � possible actions (breadth) and a maximum episode length of � (depth), we must scan over �� possible action sequences, which quickly becomes infeasible to compute in practice. To subdue the computational complexity of the search, Monte Carlo Tree Search (MCTS) has evolved into one of the go-to methods in the feld. Instead of an exhaustive search, MCTS uses a combination of Monte Carlo simulation and tree search as a heuristic search algorithm. 

MCTS executes four recurring steps: Selection, expansion, simulation, and back propagation. In the frst step, MCTS selects a node by traversing the tree until an unexpanded leaf node is reached. It expands the selected leaf node by adding one or more child nodes to it, and simulates one or more trajectories until a terminal state is reached, also called rollouts. This way, an initial value estimate of the state is created. Finally, the results of the simulation phase are backpropagated, updating the statistics of all nodes traversed during the iteration (typically the empirical state return and state visit count). 

MCTS must sufciently balance exploration and exploitation during selection to achieve robust estimates. A widespread method is Upper Confdence bounds applied to Trees (UCT) [52], which treats selection as a multi-armed bandit problem and uses   

the UCB1 formula for action selection, i.e., �� = argmax� �(��, �) + � 

√ln� (�� ) � (��,�),   

where �(��, �) is the empirical reward for taking action � in state ��, �(��) is the total number of trajectories explored from �� and �(��, �) the number of times action � was explored, and � is a hyperparameter. Intuitively, UCB1 favors exploration when estimates are uncertain but leans towards exploitation once more information has

60 Christopher Mutschler et al. 

been gathered. It can be shown that this strategy achieves regret that grows only logarithmic in the number of iterations [6]. 

An important scientifc breakthrough was achieved when AlphaGo [84] became the frst computer program to defeat a professional human Go player. In essence, AlphaGo employs MCTS with a value network to assess the value of a board position and a policy network to bias the action selection, thereby lifting the requirement for accurately simulating rollouts and focusing the search on promising actions. For the latter, a modifed version of PUCT [76] is employed, �� = argmax� �(��, �) +   

� �����(��, �) 

√� (�� ) 

1+� (��,�), where �(��, �) is the output of the policy network. Further,   

Dirichlet noise is added to the prior estimates to stimulate exploration. Due to the two-player nature of many board games, another key technique is self-play, where recent model versions compete as similarly skilled opponents during training. 

From AlphaGo, a whole line of work has evolved, intending to remove more and more prior assumptions from the method. Whereas AlphaGo initializes value and policy networks through pre-training on an expert game dataset, AlphaGo Zero [86] can surpass its ancestor’s performance without resorting to expert data (learning "tab ula rasa"). At the same time, AlphaGo Zero drops hand-engineered features, uses a simplifed neural network structure, and removes MCTS rollout simulations by entirely relying on value network estimates. In AlphaZero [85], the method is gener alized to the game of Chess and Shogi. Another vital breakthrough was achieved with MuZero [83], which learns the environment model and employs it for planning with MCTS. This means MuZero does not require access to a resettable simulator, i.e., providing the game’s rules to the learning method. They also generalized the method to the single-player Atari domain with intermediate rewards. EfcientZero [107] reduces the sample complexity of MuZero and shows promising performance in the limited training data regiment. The latest improvement is Gumbel MuZero and Gumbel AlphaZero [27], which replaces adding Dirichlet noise by sampling actions without replacement using the Gumbel-Top-k trick and sequential halving, allow ing for an efective reduction of the number of required MCTS iterations without degrading performance. 

3.4.3 Ofine Reinforcement Learning 

In many real-world use cases, an extensive trial-and-error procedure as required by traditional (online) RL is not feasible. This might be due to ethical reasons (such as medical treatment or autonomous driving) or simply because it would take too long for an agent to learn some reasonable behavior. The idea of Ofine RL is to resort to existing rollouts (from other agents/policies, collected by observing humans, or by traditionally implemented controllers) and to learn a policy based on this ofine data. 

Figure 3.3 (top left) and (top right) both illustrate the online RL setup, where the agent either follows the policy it is optimizing (on-policy) or where the agent is using data from diferent (earlier versions of the current) policies to optimize its policy

3 Learning from Experience 61   

rollout data 

Environment Agent Update 

rollout data 

Environment 

buffer 

Agent Update   

rollout(s) 

Environment 

Updated Agent rollout data 

buffer 

Train Agent 

rollout(s) 

Updated Agent Environment   

rollout(s) 

data collected 

under different policies training phase 

deployment   

Fig. 3.3: Ofine RL in context: On-Policy RL (top left), Of-Policy RL (top right), Ofine RL (bottom), based on [56]. 

(usually realized by maintaining a bufer of transitions that have been collected under diferent policies at earlier stages of learning). Figure 3.3 (bottom) shows the Ofine RL setup: as in of-policy RL, we maintain data from a variety of policies from which we want to learn a unifed policy (instead of iterating/updating new policies) that can be deployed into the environment. In contrast to Behavioral Cloning [56], which requires data D from a single expert policy �� to get good results and which is prone to failure due to poor generalization in unexpected situations, the expectation of Ofine RL is to outperform all the individual policies �� from which it learned from. 

Figure 3.4 motivates where Ofine RL should do a better job. Assume that D contains two trajectories, one from A to B and one from B to C, each trajectory takes several time-steps, and the agent gets penalty of -1 per time-step. Given the data present in the dataset we expect an agent trained on D to come up with a policy shown on the right, which takes the direct route from A to C (which is supposed to be the optimal solution here). 

Interestingly, a simple naive example already fails. Consider a dataset with expert demonstrations and successful task completions. Training in an of-policy setting, iterating on the transitions from the dataset does not converge to a usable policy;   

A 

B 

C A 

B 

C   

Fig. 3.4: Stitching.

62 Christopher Mutschler et al. 

in some settings, even Q-values start to diverge (i.e., take overly large values). The problem arises during training from bootstrapping the value function on Q-values under a slight distribution shift, i.e., in each state, the policy is deemed to bootstrap from the best (= ���) action available in a particular state, which is prone to approximation errors (as data might be incomplete). This max-term over-estimates the real Q-value and, while being corrected in an online setting (by actually taking this route and getting grounded), we will get no feedback about this error in the ofine setting and hence take routes through the state space that are diferent from what the data covers. 

Existing solutions to Ofine RL can be subdivided into methods that either (1) constrain the policy to stay in a region of trust, i.e., where we have knowledge from the dataset (which covers that regions), or (2) that estimate the state-value function conservatively based on confdence (from what we can infer from the dataset). 

Policy-constrained methods tackle the problem in the policy improvement step, i.e., they try to keep � close to ��. Batch-constrained Q-Learning (BCQ) [36] restricts the action space to force the agent to behave close to on-policy concerning the subset of the given data, hence keeping the extrapolation error of the bootstrapped actions low. While this works reasonably well, it is overly restrictive as BCQ implements a distribution matching strategy (i.e., it also tries to minimize the KL-divergence between � and ��) and hence, if the behavior policy is e.g. uniform, the learned policy is also required to be uniform. Instead, Bootstrapping Error Accumulation Reduction (BEAR) [53] only requires � to lie in the support of ��, i.e., �� : �(�|�) > 0 ⇒ �� (�|�) > �. 

Conservative methods tackle the problem in the policy evaluation step by being conservative in the state(-action)-value estimation in areas of high uncertainty (i.e., for transitions that are not in the dataset), which implicitly then keeps the policy away from out-of-distribution actions. Conservative Q-Learning (CQL) [54] learns a value function that minimizes �(�, �) on � ∈ D, � ∼ (�), and additionally maximizes for cases where � ∼ �� (�) (as in those cases there is no need to be conservative). It is proven that the return estimate of the resulting policy from CQL is lower than the actual policy performance. Model-based Ofine Policy Optimization (MOPO) [110] estimates �(�, �) and �(�′|�, �) from D and applies online RL to the learned model. As still the model can be queried in unknown regions if � diverges from ��, MOPO learns an uncertainty estimate �(�, �) and provides a pessimistic reward to the agent �˜(�, �) = �(�, �) − ��(�, �). However, as a correct estimation of �(�, �) is difcult (especially with neural networks), Conservative Ofine Model-Based Policy Optimization (COMBO) [109] combines the idea of MOPO (using rollouts from a model) with CQL: it samples transitions either from D or from the model. but assigns more trust to those state-action pairs that are observed in D. As a result, COMBO uses more data than CQL (i.e., added data from the model), and the data is correlated with the policy. 

Decision Transformers [22] are an alternative way of solving the Ofine RL problem by positing the sequential decision-making problem as a language or se quence modeling task. The idea is to use strong and advanced neural network ar chitectures (such as Transformers [102], due to their ability to capture long-horizon

3 Learning from Experience 63   

-3 

-1 -2 0 

-1 

0 

-1 

-3   

goal , ... , , goal start goal goal 

-4 -5 -3 -2 

start start 

Fig. 3.5: Decision Transformers, based on [22]. 

goal start   

dependencies) instead of algorithmic frameworks that make use of Bellman back ups: the (return, state, action) tuples are processed in a sequence and learned in an autoregressive fashion, where the task is to predict the next tuple from a hidden state that represents the past sequence (i.e., the Markov state). With regard to the principle of Decision Transformers consider Figure 3.5. Working on a fxed graph and observing/training on random rollouts (the edges show the accumulated reward), the decision transformer can be conditioned on a desired performance and produces a sequence of actions that satisfes the condition, i.e., that delivers the requested per formance. A very related but less noticed approach is Trajectory Transformer [47], which additionally uses discretization and employs beam search for trajectory plan ning. 

3.4.4 Hierarchical RL 

As the name suggests, Hierarchical Reinforcement Learning (HRL) has a hierarchy of policies. Lower-level policies are responsible for solving a sub-task of the problem (for example, they might implement specifc motor skills), while higher-level poli cies (also called master policies) implement a “strategy” that combines lower-level policies to solve a given task. The idea is that this decomposition can help with problems like exploration (since the high-level policy can enable data gathering for under-represented sub-tasks), data efciency (since combining low-level policies can converge faster compared to end-to-end training), and generalization (since a large number of tasks can potentially be solved by learning to combine an available library of sub-policies). Figure 3.6 illustrates the high-level concept of HRL. 

More formally, in the simple case where we have only a two-level hierarchy, we assume � low-level policies parameterized with (��1, ��2, �..., ��� ) and a higher level, coordinating policy �� . There are two important questions: i) how are the low-level policies provided or trained, and ii) how does the high-level policy learn to utilize and combine the low-level ones efciently. 

One of the earliest and most elegant ideas to formalize this problem is the options framework [93]. Here, an option � ∈ Ω is defned by: 

• an intra-option policy ��, which is the policy to be used when the specifc option is selected;

64 Christopher Mutschler et al. observation 

skills / low-level policies 

Policy selection 

mechanism 

action 

Fig. 3.6: Hierarchical Reinforcement Learning concept. 

• a termination function �� : S → [0, 1] that indicates the probability of termi nating (stop using) the option in the current state; 

• an initiation set I ⊆ S, indicating in which states each option can be se lected/activated (even though in many practical problems, this is the entire state space S). 

It has been shown [93] that augmenting MDPs with options results in Semi-MDPs, which in turn have optimal V and Q functions (�∗Ω(�) and �∗Ω(�, �), respectively). When an option is activated, the intra-option policy �� is utilized to select actions in each environment time-step. Once the action is executed and the next state and the reward are acquired, the option terminates with probability �� (�′). If the option is terminated at state �′, one of all available options is activated according to �Ω(�′, ·). The options framework has been extended to methods that learn both the optimal �-function over options and the intra-option policies in an end-to-end manner [7], as well as to approaches that support an arbitrary number of hierarchy levels [74]. 

One of their main limitations is defning the number of options a-priori. Of course, there are also successful HRL approaches that do not follow the options framework. In [35], a combination of Meta Learning and hierarchical policy structure is proposed. Here, several low-level policies are selectively activated by a master policy, with the latter being called within fxed time intervals. The low-level and master policies are trained sequentially over several episodes. Still, in low-level training, the reward of a specifc episode is considered, while in the master policy, the collective reward from all training episodes is utilized. Apart from the proper tuning of the master policy call time interval, also in this approach, the “correct” number of low-level policies has to be selected beforehand. 

In a diferent line of thought, [103] proposes using FeUdal Networks for HRL. In the simplest case, a “Manager” implements a high-level policy that generates a set of sub-goals (in the form of specifc states) in the latent space that a “Worker” must learn how to reach. Through training, the Manager learns to select sub-goals that lead to solving the task. Even though there is no need for pre-selection of the number of low-level policies, selecting proper sub-goals from the Manager policy is an open-ended task on its own that can hinder the scalability of the algorithm.

3 Learning from Experience 65 

In several cases, HRL is a design choice to enable safe and/or interpretable solutions to a given task. For example, in [55], a safe and reliable vehicle obstacle avoidance strategy is learned by combining a set of MPC low-level policies with a high-level DQN selection policy. In [81], utilizing low-level driving “primitives” allows distilling the master policy to a binary decision tree, thus allowing a certain level of interpretability. 

3.5 Challenges for Agent Deployment 

Besides astounding progress and movement in the feld of RL, several key chal lenges remain open for this machine learning technology to be easily and widely applicable in the real world. In this section, we will cover the aspects of safety, policy generalizability, and the issue of defning reward signals. 

3.5.1 Safety through Policy Constraints 

In many applications, an agent has to behave safely in the sense that it should not put itself or entities of its environment at risk. This is especially true for real world applications, where RL-controlled robots and machines could cause fnancial damage or risk human health or lives. At the same time, safety concerns should not disturb reward performance too much, as this would undermine the benefts of RL in contrast to less performant but provably safe traditional methods. This consideration motivates the feld of Safe RL, which aims at providing methods that bring about optimal reward performance while satisfying safety constraints. 

Constrained Markov Decision Processes (CMDPs) are a widespread formalism to model safe RL as a constraint optimization problem. The CMDP problem is an extension of the standard MDP M with a constraint set C = {(��, ��)}��=0, where ��(�, �) is a cost function that returns a cost value for a state and action pair �, �, and ��is the safety constraint bound, and we have � such cost constraints. In many cases, constraints are defned as discounted cumulative cost constraints, i.e., the expression 

��(�) = E� [Íinf 

�=0����(��, ��)] ≤ �� must hold for all � ∈ {0, . . . , �}, where ��is the expected cost. However, mean valued, probabilistic, and other constraint formulations are also utilized in the literature [58]. 

Diferent theoretical constructs to analyze and solve CMDPs have been proposed in the literature. One such category are Lagrangian approaches, which translate the CMDP formulation into a primal-dual optimization problem,   

(�∗, �∗) = arg min 

�∈Π{� (�� ) − ��(�(�) − �)},   

�≥0max 

with � (�� ) = E�∼�0[�� (�)] being the original RL objective to maximize. Besides Lagrangian-PPO and Lagrangian-TRPO [2], a highly infuential method of this

66 Christopher Mutschler et al. 

family is Reward Constrained Policy Optimization (RCPO) [97], which incorporates the constraint as a penalty signal into the reward function into a multi-timescale approach. Further, it has recently been shown that the primal-dual formulation has zero duality gap [67]. 

Another line of work are trust-region methods, which aim to improve the policy through a local policy search while enforcing the constraints in every update. Among them are Constrained Policy Optimization (CPO) [3], Projected-based Constrained Policy Optimization (PCPO) [62] and other derivative works. 

3.5.2 Generalizability of Policies 

A central reason for the growing interest in ML lies in the ability to train models that adapt properly to new, previously unseen data. Even though this is not necessarily true for all RL applications, e.g., learning a policy that behaves optimally inside the training environment could be all that we want, it is of vital importance for the applicability of RL in the real world, where agents will need to be robust to variations in their environments or capable of handling even harder forms of generalization [51]. This starkly contrasts with typical RL benchmarks like Atari and MuJoCo [99], where policies are evaluated directly inside the training environment, making it an often-overlooked algorithmic characteristic in the RL literature. 

More technically, generalization in RL requires an agent to deploy successfully across various tasks or environment instances. This encompasses variations in the state space, for example, due to changes in the initial state distribution, the envi ronment dynamics, visual aspects for image-based observation spaces, the reward function, etc. Contextual MDPs [40] is one construct to formalize this. They add a context distribution that, loosely speaking, allows for modeling distributions over MDPs. Analogous to supervised learning, the need for generalization emerges for difering train and test context sets. Depending on the distribution of the varying environmental factors, policies must learn to interpolate and/or extrapolate from the training experience to close the train-test performance gap. 

An important distinction can be made based on the occurring type of distribution shift. Training and testing are often assumed to be IID, i.e., the MDP contexts are samples of one mutual distribution. The opposite case of out-of-distribution (OOD) test environments, termed domain generalization [57], is especially hard to accomplish. Because today’s state-of-the-art RL methods typically have low sample efciency, agents are trained in simulation even though their deployment domain is a real-world environment. Transferring agents to a physical environment, or sim-to real transfer, requires OOD generalization if no additional measures are employed because camera inputs, actuator feedback, etc. can typically be simulated accurately only to some degree [113]. The issue is often alleviated by highly randomizing the simulation dynamics [70] or visuals [100] (domain randomization), or closing the visual domain gap through image-to-image GAN models [73]. Further, the feld

3 Learning from Experience 67 

of Robust RL aims to tackle specifc forms of environment model misspecifcation through worst-case optimization [111]. 

We can also characterize approaches by how much target domain data they can access. This paints a spectrum from zero-shot generalization, where no explicit target domain data is available [51], to online adaptation, which often assumes access to at least a few training episodes in the test environment (often addressed through methods of Meta RL [12])), to Continual RL, where MDP components are assumed non-stationary and the agent must continually learn to adapt to this property [50]. In the following, we will give a more detailed view of zero-shot transfer, which can be seen as the most general and straightforward form of generalization. 

Zero-Shot Transfer. Similar to methods stated for sim-to-real transfer, a common technique is to increase the similarity between source and target domain data. This can be achieved through data augmentation, as done by UCB-DrAC [72], or domain randomization techniques, like ADR [63]. A line of work aims to optimally sample from the set of randomized MDPs with approaches like POET [104] and PAIRED [30]. The latter trains an adversarial agent that designs the environment levels to guarantee solvability and maximize generalization. 

Analogous to data alignment, another feld aims to learn more robust features not specifc to the training domains. One method is encoding inductive biases, for example, by encouraging internal features that are not predictive of time within an episode, as has been done in IDAAC [71], when we know that optimal policies should not have time-dependence. Also, techniques like �2 weight decay and policy entropy regularization have improved generalization [26], as simple models can be expected to generalize the best. Finally, methods that aim to learn invariant, context independent feature representations like IPO [88] have proved successful. 

More fundamental work is done to optimize the RL objective without overft ting. Iterated Relearning (ITER) [43] introduces repeated knowledge distillation of the policy to counteract the memory efects of neural-network caused by the non stationarity of RL training. Phasic Policy Gradients (PPG) [25] splits the policy and value heads training regiment into two separate phases. Finally, initial investigations have recently shown that MBRL might inherently facilitate better generalizability [5] and might be an interesting future research direction in this area. 

3.5.3 Lack of a Reward Function 

Unlike in RL applications in games, designing a reward function for most real-world problems is a complex task, requiring extensive domain knowledge and experience, as well as a signifcant amount of fne-tuning. There are voices in the community [87] that frmly state that the reward function should be representative of the problem, even if the reward signal is sparse (meaning the reward is a rare event and a signifcant amount of exploration is required), to avoid inducing bias in the way the policy is designed. Nevertheless, designing a more rich reward signal can lead to high-quality solutions with less training data/iterations [38].

**