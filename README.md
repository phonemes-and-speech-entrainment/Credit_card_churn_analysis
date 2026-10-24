# Credit Card Churn Analysis

This project explores customer attrition in the banking sector using the BankChurners dataset from Kaggle, with the aim of understanding patterns associated with credit card churn and exploring how data analysis can support customer-retention strategies. Developed with the assistance of AI tools, including ChatGPT Projects, Google Gemini Notebooks and DeepSeek, the project follows an end-to-end Data Analytics pipeline encompassing Extract, Transform and Load (ETL), Exploratory Data Analysis (EDA) and predictive modelling, including comparisons between Logistic Regression, Random Forest and XGBoost Classifier. Beyond the technical analysis, the project aims to critically examine the ethical implications of customer profiling and predictive modelling, consider relevant data protection and GDPR principles, and responsibly document a project plan covering implementation, maintenance, future updates and evaluation. The final stage involves developing an interactive dashboard to communicate key findings through accessible visualisations and support evidence-based interpretation. Overall, the project combines practical analytical techniques with responsible AI use, ethical reflection and transparent documentation to demonstrate the stages, considerations and limitations involved in delivering a data analysis project.

**NOTE**: The modelling and EDA were performed by AI assistants which ran simulations of the author's previous projects to adapt new content, according to detailed instructions. However, running the ML models multiple times (with small changes in implementations) led to small contradictions in the best performance of each model. Contradictions can also be observed by comparing SOME ML results with those of the EDA. This result raises an important moral issue when it comes to AI ethics: should AI be allowed to make social or business decisions without THOROUGH human supervision? And should it be preferred over traditional human solutions resulting from practical experiments? These questions are all the more relevant given the difficult interpretability of the AI analysis despite the relative simplicity of the dataset and ML problem. 

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

## Dataset Content

* The project uses [Kaggle’s BankChurners dataset](https://www.kaggle.com/datasets/sakshigoyal7/credit-card-customers), which originally contains 10,127 customer records and 23 columns; the ETL process produced a reduced dataset of 10,127 rows and 16 columns for exploring customer attrition, account characteristics, transaction behaviour and potential churn predictors.

## Business Requirements

* The project aimed to identify customer characteristics and behaviours associated with credit card attrition and assess whether machine learning can distinguish existing customers from those who have left. The analysis identified potentially useful patterns for customer-retention strategies, compared classification models using metrics beyond accuracy to account for class imbalance, and communicated findings through an interactive dashboard in the final project stage. Results are interpreted responsibly, without treating associations as proof of causation or predictions as certain outcomes.

## Hypothesis and how to validate?

* **H1 — Inactivity and customer contact:** Customers who leave may have more inactive months and a different frequency of contact with the bank. Validated by comparing distributions and attrition rates across these variables in the EDA.

* **H2 — Transaction behaviour:** Attrited customers may have lower transaction counts and transaction amounts than existing customers. Validated using group comparisons and visualisations of `Total_Trans_Ct` and `Total_Trans_Amt`.

* **H3 — Customer relationships and account characteristics:** Attrition may vary with the number of products held, card category and account tenure. Validated by comparing attrition rates across `Total_Relationship_Count`, `Card_Category` and `Months_on_book`.

* **H4 — Credit and financial behaviour:** Credit limits, revolving balances and average utilisation may differ between existing and attrited customers. Validated through grouped summaries, distributions and comparisons of `Credit_Limit`, `Total_Revolving_Bal` and `Avg_Utilization_Ratio`.

* **H5 — Demographic and socioeconomic characteristics:** Attrition rates may vary across recorded demographic and socioeconomic categories. Explored differences by education, marital status, income category, age and gender, while considering missing or unknown categories and avoiding causal interpretations.

* **H6 — Relationships between predictors:** Some explanatory variables may be correlated, creating redundancy or multicollinearity. Investigated correlation patterns and considered their implications for model interpretation and performance.

* **H7 — Predictive performance:** Customer attrition can be predicted from the available customer and account features with performance better than a simple majority-class baseline. Evaluated Logistic Regression and Random Forest using a stratified train/test split, cross-validation and metrics including precision, recall, F1-score, ROC-AUC and the confusion matrix.

* **H8 — XGBoost comparison:** Evaluated an XGBoost Classifier alongside Logistic Regression and Random Forest using consistent validation procedures and performance metrics to assess their relative predictive strengths and limitations.

## Project Plan

The project plan was designed independently by the project author, who defined the main tasks and organised them in a GitHub Projects Kanban board. The board uses **Backlog, Ready, In Progress, In Review and Done** columns, with milestones, user stories and MoSCoW prioritisation (Must Have, Should Have, Could Have and Won't Have) to organise and prioritise the work. The 13 user stories provided a framework for the project, although the tasks were not completed in their original planned order and the workflow evolved as the analysis progressed.

### Implementation

The planned workflow covered project planning, data inspection and cleaning, initial identification of ethical concerns, exploratory data analysis (EDA), categorical encoding, statistical analysis, feature engineering, logistic regression modelling and performance evaluation, dashboard creation, a final ethics review and README documentation. The analytical work was developed with AI assistance across the main stages of a data analysis pipeline: ETL, EDA and predictive modelling, with Logistic Regression, Random Forest and XGBoost Classifier used to compare classification approaches. The dashboard was completed as a later stage. In retrospect, the project plan could have explicitly included the creation and organisation of separate Jupyter notebooks, clearer dependencies between tasks and dedicated testing and documentation activities.

### Maintenance

To keep the project reproducible and understandable, future maintenance should include keeping the repository organised, documenting data sources and processing decisions, recording software dependencies, and ensuring that code and notebooks can be rerun consistently. Changes to the dataset, analytical methods or modelling assumptions were documented in the repository's history (version control), while sensitive information, credentials and inappropriate disclosures were excluded from published files. If the models were ever used operationally, their performance, fairness and suitability would also need ongoing monitoring.

### Updates

The project was and can be updated by refining the analysis, reviewing the results of the different classification models, completing the interactive dashboard and incorporating the final ethical review into the documentation. Future changes should be recorded in the GitHub board and repository, with user stories, milestones and priorities revised as the scope develops. Any changes to data preparation, features, model settings or evaluation methods should be documented so that their impact on the findings can be assessed.

### Evaluation

The project was evaluated against its analytical, organisational and ethical objectives. This includes checking the accuracy and consistency of ETL outputs; assessing whether the EDA and statistical analyses address the stated hypotheses; evaluating model performance using appropriate validation procedures and metrics, including precision, recall, F1-score, ROC-AUC and the confusion matrix; and checking for data leakage, class imbalance and limitations in interpretation. The completed dashboard was assessed for clarity, usability and whether its visualisations communicate the findings accurately. Finally, the README and ethical review were checked for transparent documentation of AI assistance, responsible data use, relevant data protection considerations and limitations. The GitHub board provides a record of planned and completed work, while the evaluation findings can guide subsequent improvements.

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
* **GDPR and the limits of compliance claims:** Whether GDPR applies depends on whether individuals are identifiable; any real-world operational use involving personal data requires a lawful basis, defined purpose, security controls, and adherence to data subject rights.
* **Data Protection Impact Assessment (DPIA):** While a formal DPIA is not automatically mandatory for this educational project, a financial institution implementing large-scale profiling or automated decisions must assess legal obligations and introduce safeguards before deployment.
* **Bias, fairness and financial vulnerability:** Churn models may reproduce historical inequalities or rely on proxy variables, potentially leading to disparate impact or unfair treatment across demographic subgroups; model performance and error rates should therefore be examined across relevant groups where suitable data and lawful methods are available.
* **Predictions can affect real people:** A churn prediction is uncertain, not a statement of fact about a customer; if used operationally, false predictions could trigger unwanted marketing, inappropriate retention offers or unfair treatment, so consequential decisions should not be delegated to a model without appropriate human oversight.
* **Responsible modelling and interpretation:** Balancing algorithms to handle class imbalance responsibly ensures metrics like recall are prioritised so that high-risk churners are not overlooked.
* **Transparency and explainability:** Model performance alone does not establish that a system is fair or suitable for use; any practical deployment should make its purpose, limitations and decision process understandable to relevant stakeholders and provide a way to review or challenge consequential outcomes.
* **AI-assisted development and accountability:** Because tools like ChatGPT, Gemini, and DeepSeek were used to write code, all outputs were independently tested and verified, maintaining full author accountability.
* **Privacy when sharing work with AI services:** Uploading datasets, notebooks or code to external AI tools can expose personal data, confidential information, credentials or material subject to licensing restrictions. Care was taken to avoid exposing sensitive credentials or proprietary personal information to third-party AI platforms.
* **Academic integrity, attribution and ownership:** AI assistance and external data sources are fully disclosed in accordance with academic standards.
* **Responsible publication and maintenance:** Repositories are vetted to ensure no secrets, sensitive data, or unverified claims are published prior to sharing or deployment.

## Dashboard Design 

### Planning

- **Dashboard Strategy & Reduced Dataset Concept:** Rather than overloading users with the full multidimensional feature space, the planned dashboard focused on creating a **second reduced dataset** specifically optimized for UI performance and storytelling. This subset aggregates high-impact behavioural flags (such as sudden drops in transaction counts, revolving balance thresholds, and inactivity months) paired with model risk probabilities.
- **Ethical Focus in Visualization:** To prevent the dashboard from encouraging aggressive or invasive profiling, the design emphasises aggregate customer segment trends rather than individual-level surveillance. Visual elements explicitly highlight analytical uncertainty and caution against treating model scores as causal certainties.
- **Planned Layout & Components:**
  - *Overview Summary Cards:* Key metrics including overall churn rate (~16%), active customer counts, and average customer tenure.
  - *Behavioural & Transactional Breakdown:* Interactive charts comparing `Total_Trans_Ct` and `Total_Trans_Amt` distributions between active and attrited cohorts.
  - *Risk & Feature Insight Panel:* Visual representation of top features selected via model tuning (e.g., revolving balances, contact frequency), paired with contextual tooltips explaining model limitations and ethical safeguards.

### Implementation & Adaptation: How the Created Dashboard Differs from the Plan

- **Shift to Interactive Multi-Dimensional Filters & Demographic Audits:** While the initial plan focused primarily on core transaction distributions and feature risk panels, the actual Tableau Public implementation expanded to include comprehensive global filters (`Card_Category`, `Marital_Status`, `Income_Category`, and `Education_Level`) and explicit demographic/socioeconomic auditing plots.
- **New Visual Elements Added for Fairness & Equity:** 
  - *Income & Credit Limit Fairness (`credit limit: income x attrition`):* Examines whether credit allocation is equitably distributed relative to income, or if lower-income brackets face systemic limits or higher vulnerability.
  - *Socioeconomic & Educational Interaction (`attrited customers: income x education`):* Breaks down churn patterns across crossing income and education brackets, addressing data quality gaps such as explicit "Unknown" categories.
  - *Demographic Compliance (`gender x attrition`):* Reconfigured into a clean horizontal 100% stacked bar chart to audit gender equity and prevent disparate impact.
- **Integration of an Ethics & Data Governance Disclaimer:** Added a dedicated structural text container outlining model limitations, non-causal interpretations, and protections against invasive customer profiling.

### Communication to Technical and Non-Technical Audiences

- **Layered Visual Design:** Complex machine learning findings and model drivers are translated into intuitive, high-impact visual comparisons (such as transaction cuts and demographic ratios) that are easily grasped by business stakeholders and non-technical viewers.
- **Contextual Transparency:** Tooltips, categorical filter controls, and an explicit ethics disclaimer ensure that technical metrics (like attrition probabilities) are contextualized responsibly, framing outputs as aggregate behavioral tendencies rather than deterministic individual predictions.

## Unfixed Bugs

* Early iterations of model selection threw data-sparsity warnings when combining older pandas structures with `xgboost` integration; these were resolved by updating explicit type checks and utilising compatible data matrix pipelines.

* Gaps in understanding advanced feature selection (`SelectFromModel`) and hyperparameter tuning pipelines were addressed through iterative code testing and cross-referencing AI-assisted documentation.

## Development Roadmap

* Encountered technical hurdles when attempting to bridge advanced machine learning concepts (such as automated hyperparameter optimisation via `GridSearchCV` and embedded feature selection) with ethical constraints like model interpretability and bias mitigation.

* Skills Learned & Future Goals: Strengthened technical proficiency in building robust scikit-learn pipelines, handling class imbalance with cost-sensitive tuning, and evaluating models using ROC-AUC and recall metrics. Future goals include mastering advanced model explainability frameworks to audit feature importances for fairness.

## Deployment 

* The Tableau dashboard was deployed using Tableau Public and can be viewed online by accessing the following [link](https://public.tableau.com/views/Credit_Card_Fairness_Analysis/Credit_Card_Dashboard?:language=en-GB&:sid=&:redirect=auth&:display_count=n&:origin=viz_share_link).

## Main Data Analysis Libraries

* **Pandas:** For data loading, cleaning, manipulation, and aggregation in DataFrames across the ETL and exploratory phases.
* **NumPy:** For efficient numerical operations, mathematical functions, and array handling on tabular data structures.
* **Matplotlib:** For creating foundational, customisable plots and visualising statistical distributions.
* **Seaborn:** For generating high-level, aesthetically pleasing, and informative statistical graphics (such as countplots, histograms, and correlation maps).
* **Scikit-learn (`sklearn`):** For implementing machine learning classification models (Logistic Regression, Random Forest, XGBoost), preprocessing tools (`StandardScaler`, `OneHotEncoder`), pipeline construction, automated model tuning (`GridSearchCV`), and embedded feature selection (`SelectFromModel`).
* **XGBoost (`xgboost`):** For gradient-boosting classification and handling gradient optimisation on tabular customer data.
* **Imbalanced-learn (`imblearn`):** For handling class imbalance via over-sampling techniques (`SMOTE`) and ensuring safe data resampling within cross-validation (`ImbPipeline`).
* **OS:** For interacting with the operating system, managing file paths, and handling directory navigation across the project environment.
* **Warnings:** For controlling and filtering runtime and deprecation warnings to maintain clean and reproducible notebook outputs.

## Credits

### Content 

* Dataset sourced from Kaggle: *Credit Card Customers* (BankChurners dataset).  
* Code Institute learning materials and project templates serving as structural foundations.   
* Code development, debugging, and structural ideation assisted by generative AI tools (ChatGPT Projects, Google Gemini Notebooks, and DeepSeek). 

### Media

* The Code Institute logo was used as per the project template.

## Acknowledgements (optional)

* Special thanks to mentors, peers, and evaluators who provided feedback throughout the development of this analysis pipeline.