\# Feature Fatigue Analysis using User Reviews  

\### A Case Study on Zerodha Kite



This project analyzes user review data to understand how feature-related discussions evolve over time and how increasing product complexity can lead to sustained user friction. The study introduces a \*\*Feature Fatigue Index (FFI)\*\* that combines discussion intensity and sentiment trends to identify high-impact issue areas.



The goal is not to evaluate the product itself, but to demonstrate how \*\*public user feedback can be transformed into structured, decision-oriented insights\*\* using data science techniques.



---



\## 📌 Problem Statement



As digital products mature, new features are continuously added. However, increased functionality does not always translate to improved user satisfaction. Users may experience difficulty navigating, understanding, or adapting to frequent changes.



This project attempts to answer:

\- Which feature areas consistently attract user attention?

\- How does sentiment evolve as discussion intensity increases?

\- Can we quantify sustained user friction beyond raw sentiment scores?



---



\## 📊 Data Overview



\- \*\*Source\*\*: Publicly available Google Play Store user reviews  

\- \*\*Volume\*\*: 1,000+ user reviews  

\- \*\*Time Range\*\*: Multi-month review history  

\- \*\*Granularity\*\*: Individual reviews aggregated at monthly level  



Only publicly accessible data was used. No personal or private user information was collected.  

Data was cleaned and processed to prepare it for text analysis and time-series aggregation.



---



\## 🔍 Methodology



The analysis follows a structured pipeline:



1\. \*\*Text Preprocessing\*\*

&nbsp;  - Cleaning and normalization of review text

&nbsp;  - Removal of noise and irrelevant tokens



2\. \*\*Topic Discovery\*\*

&nbsp;  - TF-IDF vectorization

&nbsp;  - Latent Dirichlet Allocation (LDA) for topic modeling

&nbsp;  - Identification of 6 dominant discussion themes



3\. \*\*Topic Velocity Analysis\*\*

&nbsp;  - Monthly aggregation of topic frequency

&nbsp;  - Measurement of changes in user attention over time



4\. \*\*Sentiment Analysis\*\*

&nbsp;  - VADER sentiment scoring at review level

&nbsp;  - Monthly topic-wise sentiment trends



5\. \*\*Feature Fatigue Index (FFI)\*\*

&nbsp;  - Composite index combining:

&nbsp;    - Topic discussion velocity

&nbsp;    - Sentiment trend behavior

&nbsp;  - Normalized to enable relative comparison across topics



---



\## 📈 Key Visual Insights



\### Feature Fatigue Index (FFI) by Topic

Identifies topics where sustained discussion is accompanied by weaker sentiment trends.



\### Topic Velocity Over Time

Shows how user attention shifts across feature areas month-by-month.



\### Sentiment Trends Across Topics

Highlights how user sentiment evolves independently of discussion volume.



All visualizations are available in the `/visuals` folder and explained in detail in the report.



---



\## 📄 Case Study Report



A detailed, non-technical case study explaining:

\- The motivation behind the analysis

\- What each metric represents

\- How to interpret the findings



📄 \*\*Report\*\*:  

`/reports/Zerodha\_Kite\_Feature\_Fatigue\_Case\_Study.pdf`



---



\## 📁 Project Structure

zerodha-kite-feature-fatigue/

│

├── data/

│   ├── raw/

│   │   └── zerodha\_kite\_reviews\_raw.xlsx

│   │

│   └── processed/

│       ├── zerodha\_kite\_reviews\_clean.xlsx

│       ├── zerodha\_kite\_reviews\_with\_topics.xlsx

│       ├── zerodha\_kite\_monthly\_topic\_sentiment.xlsx

│       ├── zerodha\_topic\_velocity.xlsx

│       ├── zerodha\_kite\_feature\_fatigue\_index.xlsx

│       └── zerodha\_kite\_feature\_fatigue\_index\_labeled.xlsx

│

├── notebooks/

│   ├── 01\_data\_collection.ipynb

│   ├── 02\_text\_cleaning.ipynb

│   ├── 03\_topic\_modeling.ipynb

│   ├── 04\_topic\_velocity\_analysis.ipynb

│   ├── 05\_sentiment\_trends\_by\_topic.ipynb

│   └── 06\_feature\_fatigue\_index.ipynb

│

├── visuals/

│   ├── feature\_fatigue\_index\_by\_topic.png

│   ├── sentiment\_trend\_by\_topic.png

│   └── topic\_velocity\_over\_time.png

│

├── report/

│   └── Zerodha\_Kite\_Feature\_Fatigue\_Case\_Study.pdf

│

└── README.md




---



\## 🧠 Key Takeaways



\- High user attention does not always imply positive experience.

\- A small number of topics often account for most sustained discussion.

\- Combining sentiment with temporal attention reveals deeper user friction patterns.

\- Feature Fatigue Index provides a scalable way to prioritize issue areas.



---



\## 🔗 Author



\*\*Swastik Singh\*\*  

\- GitHub: https://github.com/swastiksingh04  

\- LinkedIn: https://www.linkedin.com/in/swastik-singh-821464275/



---



\## ⚠️ Disclaimer



This project is an independent academic-style analysis based on publicly available data and is not affiliated with or endorsed by Zerodha.





