# COVID-19 Impact on Mental Health Analysis based on Reddit Comments

This study uses natural language processing (NLP) on comments from the website Reddit to determine the effects of the COVID-19 pandemic on the mental health of 5 communities: r/anxiety, r/depression, r/SuicideWatch, r/mentalhealth, and r/COVID19_support.

## Requirements
- Jupyter Notebook or Jupyter Lab
- Python 3.10
- TensorFlow 2.11.0
- NLTK (Natural Language Tool Kit)
- Scikit-learn 1.2.2
- Demoji 1.1.0

## Paper
[The paper](https://ieeexplore.ieee.org/document/9995512) for this research was published in the 2022 IEEE Bioinformatics and Biomedicine (BIBM) conference in Las Vegas.

## Methods
I used two public datasets for training:
- [The Reddit COVID Dataset](https://socialgrep.com/datasets/the-reddit-covid-dataset)
- [Reddit Mental Health Dataset](https://zenodo.org/record/3941387#.ZBS-OezMJhG)

I also collected my own dataset for the 5 subreddits studied using Reddit’s API, the Python Reddit
API Wrapper (PRAW) in order to analyze the most recent comments.

We used the Scikit-learn library to train 6 support vector machines (SVM) -- one for sentiment analysis, and five for binary classifcation of each subreddit. We then extracted features from the SVMs to determine the issues that
these subreddits were struggling with the most during the
COVID-19 pandemic. 

We then used a long short-term memory
(LSTM) recurrent neural network to study the change in
sentiment of each subreddit over the course of the pandemic.

## Conclusions
In this study, we revealed the effectiveness of support
vector machines and LSTM neural networks in analyzing
mental health in social media comments related to COVID-19.

Based on our research, feelings of isolation, out of the potential
factors studied, had the most impact on mental health during
COVID-19. Additionally, this study suggested that the
sentiment of some mental health communities, but not all, were
correlated with new COVID-19 cases. Furthermore, not all
mental health communities were equally affected by the
COVID-19 pandemic; while some subreddits were similarly
affected in one way, they differed in other ways. Continued
research to cover the impacts beyond March of 2022 is still
ongoing.

## Acknowledgements
I am grateful for the support on this project from the following people:
- Kevin Qi, Boston College
- Aaron Zhang, Brown University
- Mikhail Shalaginov, MIT
- Tingying Helen Zeng, AARD

## References
- [1] Brooks, S. K., Webster, R. K., Smith, L. E., Woodland, L., Wessely, S.,
Greenberg, N., &amp; Rubin, G. J. (2020). The psychological impact of
quarantine and how to reduce it: rapid review of the evidence. Lancet
(London, England), 395(10227), 912–920.
- [2] Alonzi, S., La Torre, A., &amp; Silverstein, M. W. (2020). The
psychological impact of preexisting mental and physical health conditions
during the COVID-19 pandemic. Psychological Trauma: Theory,
Research, Practice, and Policy, 12(S1), S236–S238.
- [3] Efstathiou, V., Stefanou, M., Siafakas, N., Makris, M., Tsivgoulis, G.,
Zoumpourlis, V. Rizos, E. (2022). Suicidality and COVID‐19: Suicidal
ideation, suicidal behaviors and completed suicides amidst the COVID‐19
pandemic (Review). Experimental and Therapeutic Medicine, 23, 107.
- [4] Low, D. M., Rumker, L., Talkar, T., Torous, J., Cecchi, G., &amp; Ghosh,
S. S. (2020). Natural Language Processing Reveals Vulnerable Mental
Health Support Groups and Heightened Health Anxiety on Reddit During
COVID-19: Observational Study. Journal of medical Internet research,
22(10).
- [5] Talevi, D., Socci, V., Carai, M., Carnaghi, G., Faleri, S., Trebbi, E., ... &
Pacitti, F. (2020). Mental health outcomes of the CoViD-19
pandemic. Rivista di psichiatria, 55(3), 137-144.
- [6] Liu S, Yang L, Zhang C, Xiang YT, Liu Z, Hu S, Zhang B. Online mental
health services in China during the COVID-19 outbreak. Lancet
Psychiatry. 2020 Apr;7(4):e17-e18. doi: 10.1016/S2215-0366(20)30077-8. Epub 2020 Feb 19. PMID: 32085841; PMCID: PMC7129099.
- [7] CALVO, R., MILNE, D., HUSSAIN, M., &amp; CHRISTENSEN, H.
(2017). Natural language processing in mental health applications using
non-clinical texts. Natural Language Engineering, 23(5), 649-685.
- [8] De Choudhury, M., Gamon, M., Counts, S., & Horvitz, E. (2021).
Predicting Depression via Social Media. Proceedings of the International
AAAI Conference on Web and Social Media, 7(1), 128-137. Retrieved
from https://ojs.aaai.org/index.php/ICWSM/article/view/14432
- [9] Judy Hanwen Shen and Frank Rudzicz. 2017. Detecting Anxiety
through Reddit. In Proceedings of the Fourth Workshop on
Computational Linguistics and Clinical Psychology — From Linguistic
Signal to Clinical Reality, pages 58–65, Vancouver, BC. Association for
Computational Linguistics.
- [10] Z. Liu and H. Chen, "A predictive performance comparison of machine
learning models for judicial cases," 2017 IEEE Symposium Series on
Computational Intelligence (SSCI), 2017, pp. 1-6, doi:
10.1109/SSCI.2017.8285436.
- [11] N. Smitha and R. Bharath, "Performance Comparison of Machine
Learning Classifiers for Fake News Detection," 2020 Second
International Conference on Inventive Research in Computing
Applications (ICIRCA), 2020, pp. 696-700, doi:
10.1109/ICIRCA48905.2020.9183072.
- [12] Zhang Z, Beck MW, Winkler DA, Huang B, Sibanda W, Goyal H; written
on behalf of AME Big-Data Clinical Trial Collaborative Group. Opening
the black box of neural networks: methods for interpreting neural network
models in clinical applications. Ann Transl Med. 2018 Jun;6(11):216. doi:
10.21037/atm.2018.05.32. PMID: 30023379; PMCID: PMC6035992.
- [13] Habimana, O., Li, Y., Li, R., Gu, X., &amp; Yu, G. (2020). Sentiment
analysis using deep learning approaches: An overview. Science China
Information Sciences, 63(1), 111102. https://doi.org/10.1007/s11432-
018-9941-6
- [14] H. Jelodar, Y. Wang, R. Orji and S. Huang, "Deep Sentiment
Classification and Topic Discovery on Novel Coronavirus or COVID-19
Online Discussions: NLP Using LSTM Recurrent Neural Network
Approach," in IEEE Journal of Biomedical and Health Informatics, vol.
24, no. 10, pp. 2733-2742, Oct. 2020, doi: 10.1109/JBHI.2020.3001216.
- [15] JT Wolohan. 2020. Estimating the effect of COVID-19 on mental health:
Linguistic indicators of depression during a global pandemic. In
Proceedings of the 1st Workshopon NLP for COVID-19 at ACL 2020,
Online. Association for Computational Linguistics.
- [16] Pancani, L., Marinucci, M., Aureli, N., & Riva, P. (2021). Forced social
isolation and mental health: a study on 1,006 Italians under COVID-19
lockdown. Frontiers in Psychology, 12, 663799.
