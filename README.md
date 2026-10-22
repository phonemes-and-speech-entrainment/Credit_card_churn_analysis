# Project XYZ

**Project XYZ** is a comprehensive data analysis tool designed to streamline data exploration, analysis, and visualisation. The tool supports multiple data formats and provides an intuitive interface for both novice and expert data scientists.

# ![CI logo](https://codeinstitute.s3.amazonaws.com/fullstack/ci_logo_small.png)

## Dataset Content

* Describe your dataset. Choose a dataset of reasonable size to avoid exceeding the repository's 100GB limit.

## Business Requirements

* Describe your business requirements

## Hypothesis and how to validate?

* List here your project hypothesis(es) and how you envision validating it (them) 

## Project Plan

* Outline the high-level steps taken for the analysis.
* How was the data managed throughout the collection, processing, analysis and interpretation steps?
* Why did you choose the research methodologies you used?

## The rationale to map the business requirements to the Data Visualisations

* List your business requirements and a rationale for mapping them to the Data Visualisations

## Analysis techniques used

* List the data analysis methods used and explain limitations or alternative approaches.
* How did you structure the data analysis techniques? Justify your response.
* Did the data limit you, and did you use an alternative approach to meet these challenges?
* How did you use generative AI tools to help with ideation, design thinking and code optimisation?

## Ethical considerations (optional)

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

### Heroku (optional)

* This section is necessary only if you are deploying a Streamlit app to Heroku as part of your submission for units 2 and 3. 
* The App live link is: https://YOUR_APP_NAME.herokuapp.com/ 
* Set the `.python-version` Python version to a [Heroku-22](https://devcenter.heroku.com/articles/python-support#supported-runtimes) stack currently supported version.
* The project was deployed to Heroku using the following steps.

1. Log in to Heroku and create an App
2. From the Deploy tab, select GitHub as the deployment method.
3. Select your repository name and click Search. Once it is found, click Connect.
4. Select the branch you want to deploy, then click Deploy Branch.
5. The deployment process should happen smoothly if all deployment files are fully functional. Click the button Open App at the top of the page to access your App.
6. If the slug size is too large, then add large files not required for the app to the `.slugignore` file.

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
