# Credit Card Churn Analysis

This project explores customer attrition in the banking sector using the BankChurners dataset from Kaggle, with the aim of understanding patterns associated with credit card churn and exploring how data analysis can support customer-retention strategies. Developed with the assistance of AI tools, including ChatGPT Projects, Google Gemini Notebooks and DeepSeek, the project follows an end-to-end Data Analytics pipeline encompassing Extract, Transform and Load (ETL), Exploratory Data Analysis (EDA) and predictive modelling, including comparisons between Logistic Regression, Random Forest and XGBoost Classifier. Beyond the technical analysis, the project aims to critically examine the ethical implications of customer profiling and predictive modelling, consider relevant data protection and GDPR principles, and responsibly document a project plan covering implementation, maintenance, future updates and evaluation. The final stage involves developing an interactive dashboard to communicate key findings through accessible visualisations and support evidence-based interpretation. Overall, the project combines practical analytical techniques with responsible AI use, ethical reflection and transparent documentation to demonstrate the stages, considerations and limitations involved in delivering a data analysis project.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

## Dataset Content

* The project uses Kaggle’s BankChurners dataset, which originally contains 10,127 customer records and 23 columns; the ETL process produces a reduced dataset of 10,127 rows and 16 columns for exploring customer attrition, account characteristics, transaction behaviour and potential churn predictors.

## Business Requirements

* The project aims to identify customer characteristics and behaviours associated with credit card attrition and assess whether machine learning can distinguish existing customers from those who have left. The analysis should identify potentially useful patterns for customer-retention strategies, compare classification models using metrics beyond accuracy to account for class imbalance, and communicate findings through an interactive dashboard in the final project stage. Results should be interpreted responsibly, without treating associations as proof of causation or predictions as certain outcomes.

## Hypothesis and how to validate?

* **H1 — Inactivity and customer contact:** Customers who leave may have more inactive months and a different frequency of contact with the bank. Validate by comparing distributions and attrition rates across these variables in the EDA.

* **H2 — Transaction behaviour:** Attrited customers may have lower transaction counts and transaction amounts than existing customers. Validate using group comparisons and visualisations of Total_Trans_Ct and Total_Trans_Amt.

* **H3 — Customer relationships and account characteristics:** Attrition may vary with the number of products held, card category and account tenure. Validate by comparing attrition rates across Total_Relationship_Count, Card_Category and Months_on_book.

* **H4 — Credit and financial behaviour:** Credit limits, revolving balances and average utilisation may differ between existing and attrited customers. Validate through grouped summaries, distributions and comparisons of Credit_Limit, Total_Revolving_Bal and Avg_Utilization_Ratio.

* **H5 — Demographic and socioeconomic characteristics:** Attrition rates may vary across recorded demographic and socioeconomic categories. Explore differences by education, marital status, income category, age and gender, while considering missing or unknown categories and avoiding causal interpretations.

* **H6 — Relationships between predictors:** Some explanatory variables may be correlated, creating redundancy or multicollinearity. Investigate correlation patterns and consider their implications for model interpretation and performance.

* **H7 — Predictive performance:** Customer attrition can be predicted from the available customer and account features with performance better than a simple majority-class baseline. Evaluate Logistic Regression and Random Forest using a stratified train/test split, cross-validation and metrics including precision, recall, F1-score, ROC-AUC and the confusion matrix.

* **H8 — XGBoost comparison:** Evaluate an XGBoost Classifier alongside Logistic Regression and Random Forest using consistent validation procedures and performance metrics to assess their relative predictive strengths and limitations.

## Project Plan

The project plan was designed independently by the project author, who defined the main tasks and organised them in a GitHub Projects Kanban board. The board uses **Backlog, Ready, In Progress, In Review and Done** columns, with milestones, user stories and MoSCoW prioritisation (Must Have, Should Have, Could Have and Won't Have) to organise and prioritise the work. The 13 user stories provided a framework for the project, although the tasks were not completed in their original planned order and the workflow evolved as the analysis progressed.

### Implementation

The planned workflow covered project planning, data inspection and cleaning, initial identification of ethical concerns, exploratory data analysis (EDA), categorical encoding, statistical analysis, feature engineering, logistic regression modelling and performance evaluation, dashboard creation, a final ethics review and README documentation. The analytical work was developed with AI assistance across the main stages of a data analysis pipeline: ETL, EDA and predictive modelling, with Logistic Regression, Random Forest and XGBoost Classifier used to compare classification approaches. The dashboard is planned as a later stage. In retrospect, the project plan could have explicitly included the creation and organisation of separate Jupyter notebooks, clearer dependencies between tasks and dedicated testing and documentation activities.

### Maintenance

To keep the project reproducible and understandable, future maintenance should include keeping the repository organised, documenting data sources and processing decisions, recording software dependencies, and ensuring that code and notebooks can be rerun consistently. Changes to the dataset, analytical methods or modelling assumptions were documented in the repository's history (version control), while sensitive information, credentials and inappropriate disclosures were excluded from published files. If the models were ever used operationally, their performance, fairness and suitability would also need ongoing monitoring.

### Updates

The project was and can be updated by refining the analysis, reviewing the results of the different classification models, completing the interactive dashboard and incorporating the final ethical review into the documentation. Future changes should be recorded in the GitHub board and repository, with user stories, milestones and priorities revised as the scope develops. Any changes to data preparation, features, model settings or evaluation methods should be documented so that their impact on the findings can be assessed.

### Evaluation

The project was evaluated against its analytical, organisational and ethical objectives. This includes checking the accuracy and consistency of ETL outputs; assessing whether the EDA and statistical analyses address the stated hypotheses; evaluating model performance using appropriate validation procedures and metrics, including precision, recall, F1-score, ROC-AUC and the confusion matrix; and checking for data leakage, class imbalance and limitations in interpretation. The completed dashboard should be assessed for clarity, usability and whether its visualisations communicate the findings accurately. Finally, the README and ethical review should be checked for transparent documentation of AI assistance, responsible data use, relevant data protection considerations and limitations. The GitHub board provides a record of planned and completed work, while the evaluation findings can guide subsequent improvements.

## The rationale to map the business requirements to the Data Visualisations

* **Communicate actionable insights:** Develop an interactive dashboard to present key findings clearly and support evidence-based customer-retention strategies, while avoiding causal claims or assumptions about individual customers.
* **Promote responsible interpretation:** Use visualisations and documentation to communicate uncertainty, analytical limitations and relevant ethical considerations.

## Analysis techniques used

* **ETL and data preparation:** Inspect, clean and reduce the dataset, addressing data quality issues and preparing variables for analysis; decisions may affect results and should be documented.
* **EDA and statistical analysis:** Use descriptive statistics, grouped comparisons, distributions and correlation analysis to explore patterns and relationships; associations do not establish causation, and statistical tests require appropriate assumptions.
* **Feature preparation and modelling:** Encode categorical variables and compare Logistic Regression, Random Forest and XGBoost Classifier. Evaluate performance using appropriate validation and metrics, including precision, recall, F1-score, ROC-AUC and the confusion matrix. Class imbalance, feature selection, multicollinearity and data leakage can affect reliability; alternative models and feature-engineering approaches may be explored where justified.
* **Data limitations:** The analysis is constrained by the variables, quality and representativeness of the available dataset; findings may not generalise to other customers, banks or time periods, and missing context cannot be recovered through modelling alone.
* **Generative AI assistance:** ChatGPT Projects, Google Gemini and DeepSeek supported ideation, code development, debugging and documentation across the ETL, EDA and modelling stages. AI-generated outputs require independent review, testing and validation; the project plan and workflow were devised and organised by the author.

## Ethical considerations

* **Public data is not permission for every use:** Although the BankChurners dataset is publicly available through Kaggle, its original collection context, provenance and licensing conditions may not be fully verifiable within this project. The analysis considers data minimisation, appropriate use of customer identifiers, data quality and responsible interpretation, but does not independently establish whether the original data collection had a lawful basis, whether informed consent was obtained, or whether the dataset is genuinely anonymous and free from historical bias. Public availability alone does not resolve these issues.
* **Data protection and minimisation:** The project should use only the data necessary for its analytical purpose, exclude customer identifiers such as `CLIENTNUM` from predictive features, and avoid exposing personal or confidential information through datasets, visualisations or published outputs.
* **GDPR and the limits of compliance claims:** Whether GDPR applies depends on whether individuals are identifiable and on the nature of the processing; any real-world use involving personal data would need a lawful basis, a defined purpose, appropriate security and retention controls, and respect for individuals’ rights.
* **Data Protection Impact Assessment (DPIA):** A formal DPIA is not automatically required for this educational project, but a bank considering large-scale customer profiling or automated decisions with significant effects should assess whether one is legally required, document risks to individuals and introduce proportionate safeguards before deployment.
* **Bias, fairness and financial vulnerability:** Churn models may reproduce historical inequalities or rely on proxy variables, potentially leading to some customer groups receiving less favourable treatment; model performance and error rates should therefore be examined across relevant groups where suitable data and lawful methods are available.
* **Predictions can affect real people:** A churn prediction is uncertain, not a statement of fact about a customer; if used operationally, false predictions could trigger unwanted marketing, inappropriate retention offers or unfair treatment, so consequential decisions should not be delegated to a model without appropriate human oversight.
* **Responsible modelling and interpretation:** The project compares Logistic Regression, Random Forest and XGBoost Classifier models using appropriate validation and performance measures, while recognising class imbalance, potential data leakage, model limitations and the distinction between predictive associations and causal explanations.
* **Transparency and explainability:** Model performance alone does not establish that a system is fair or suitable for use; any practical deployment should make its purpose, limitations and decision process understandable to relevant stakeholders and provide a way to review or challenge consequential outcomes.
* **AI-assisted development and accountability:** The Jupyter notebooks in this repository were developed with assistance from ChatGPT Projects, Google Gemini and DeepSeek; AI-generated code, analysis and explanations can be incorrect or biased, so outputs must be checked, tested and reproducible, and responsibility for the submitted work remains with the project author.
* **Privacy when sharing work with AI services:** Uploading datasets, notebooks or code to external AI tools can expose personal data, confidential information, credentials or material subject to licensing restrictions; only information that is appropriate and authorised to share should be submitted, taking account of each service’s data-handling terms and settings.
* **Academic integrity, attribution and ownership:** AI assistance should be disclosed transparently in line with course requirements, and external code, datasets and other materials should be attributed appropriately; generated content should not be assumed to be original, factually correct or free of third-party rights.
* **Responsible publication and maintenance:** Before sharing the repository or deploying the dashboard, check for sensitive data, secrets, licensing issues and misleading disclosures; any operational model would also need appropriate access controls, ongoing performance and fairness monitoring, and documented updates as customer behaviour and data change.

## Dashboard Design (optional)

* Feel free to delete this section if this is a data visualisation only (unit 1 or 2) project submission.
* List all dashboard pages and their content, either blocks of information or widgets, like buttons, checkboxes, images, or any other item that your dashboard library supports.
* Later, during project development, you may revisit your dashboard plan to update a feature (for example, at the beginning of the project, you were confident you would use a given plot to display an insight, but later you used another plot type).
* How were data insights communicated to technical and non-technical audiences?
* Explain how the dashboard was designed to communicate complex data insights to different audiences. 

## Unfixed Bugs

* Please list any unfixed bugs and explain why they were not fixed. This section should include shortcomings of the frameworks or technologies used. Although time can be a significant variable to consider, paucity of time and difficulty understanding implementation are not valid reasons to leave bugs unfixed.
* Did you recognise gaps in your knowledge, and how did you address them?
* If applicable, include evidence of feedback received (from peers or instructors) and how it improved your approach or understanding.

## Development Roadmap

* What challenges did you face, and what strategies were used to overcome these challenges?
* What new skills or tools do you plan to learn next based on your project experience? 

## Deployment (optional)

* If this is a Unit 3 Streamlit, Power BI or Tableau Public project, then you can include a link here and explain how you hosted the dashboard.

## Main Data Analysis Libraries

* Here you should list the libraries you used in the project and provide an example(s) of how you used these libraries.

## Credits

* In this section, you need to reference where you got your content, media and extra help from. It is common practice to use code from other repositories and tutorials; however, it is important to be very specific about these sources to avoid plagiarism. 
* You can break the credits section into Content and Media, depending on what you include in your project. 

### Content 

- The text for the Home page was taken from the Wikipedia Article A
- Instructions on how to implement form validation were taken from a [Specific YouTube Tutorial](https://www.youtube.com/)
- The icons in the footer were taken from [Font Awesome](https://fontawesome.com/)

### Media

- The photos used on the home and sign-up page are from This Open-Source site
- The images used for the gallery page were taken from this other open-source site



## Acknowledgements (optional)

* Thank the people who supported this project.
