# Basic Information

| Name:              | Michael Zhang     |
| -------------------- | ------------------- |
| Gender:            | Male              |
| Place of Birth:    | Inner Mongolia    |
| Date of Birth:     | 1993.12           |
| Contact Number:    | 13520572037       |
| Email:             | 904690437@163.com |
| Education Level:   | Undergraduate     |
| Current Residence: | Beijing           |


# **Educational Experience**

## **Jilin University**

**Duration**: August 2011 – June 2015

* **Degree**: Bachelor's in Communication Engineering
* **Status**: Full-time undergraduate

## **Beihang University**

**Duration**: August 2022 – June 2025 (Expected)

* **Degree**: Master of Science (MSc) in Software Engineering
* **Status**: Part-time postgraduate

# Professional Skill

* **Highly proficient in Python, with extensive experience in remote development via Linux. Skilled in C, C++, and C# languages.**
* **Expertise in PyTorch and well-versed with training frameworks such as Megatron and ColossalAI.**
* **Experience in AIGC training and adept at crafting prompts to leverage the capabilities of ChatGPT.**
* **Comprehensive knowledge in Natural Language Processing (NLP), encompassing areas like large model training, classification matching, entity extraction, among others. Proficient in a range of machine learning algorithms.**
* **Personal repositories can be found at: **
  * [Gitee](https://gitee.com/michaelzhang93/projects)
  * [GitHub](https://github.com/Caesar1993?tab=repositories)

# Project Experience:

## *Project 1. Medical GPT large model training*

* **Project Duration**: February 2023 - Present
* **Project Description**:
  1. **Development and training of a specialized large-scale model in the medical field with tens of billions of parameters for intelligent consultations.**
  2. **Utilized over 100 million doctor-patient online conversation records as training data.**
* **Key Steps**:
  1. **Conducted rigorous data cleaning for both single-round and multi-round dialogues. After refinement, over 50 million doctor-patient dialogues were retained for training.**
  2. **To optimize training efficiency across multiple machines and GPUs, implemented acceleration strategies including the Megatron framework, data bucketing, and gradient accumulation.**
  3. **Selected GPT-2 as the foundational model. Additionally, explored training methodologies for large-scale models like GLM and LLaMA.**

## *Project 2. GLM fine-tuning*

* **Project Duration**: 2023/4-present
* **Project Description**:
  1. **Addressed challenges associated with the BERT model’s token limitations leading to sub-optimal accuracy and recall rates in long text classification. Here, long text refers to articles exceeding 2,000 words.**
  2. **Aimed to achieve both accuracy and recall rates of approximately 80% for each category to meet business standards.**
* **Key Steps**:
  1. **Evaluated the capabilities of prevalent large models and, after reviewing the p-Tuning paper, ascertained the GLM model’s Natural Language Understanding (NLU) prowess. Selected the chatglm-6b model as the foundational model.**
  2. **Experimented with the THUNS public dataset, focusing on texts ranging between 2,000 to 4,000 words. The training dataset comprised 30,000 instances.**
  3. **Employed the p-Tuning technique to fine-tune chatglm-6b. Achieved F1 scores higher than 80% for nine categories in a test set of 5,000 items. The remaining three categories also exceeded 75%.**

## *Project 3. Chart Extraction of Paper PDF*

* **Project Duration**: 2022/12-2022/2
* **Project Description**:
  1. **Recognized the significance of graphical data (charts, tables) within research paper PDFs and aimed to efficiently extract and present them to researchers.**
  2. **Before my intervention, the precision and recall rates for graph and table extraction were roughly 60%—deemed unsatisfactory.**
* **Key Steps**:

1. **After dissecting the structure of the papers’ PDF format, transitioned from neural network approaches to stream data and rule-based processing.**
   2. **Utilized PyMuPDF for stream data identification, progressively building extraction rules (e.g., triggering horizontal line detection upon table name identification).**
2. **Currently, evaluations based on individual graphics and tables reveal over 95% accuracy in table extraction, rendering it commercially viable. Image extraction accuracy stands at 85%, a notable edge over competitors.**

## *Project 4. **Medical Institutions’ Abbreviation and Full-Name Extraction***

* **Project Duration**: 2022/10-2022/12
* **Project Description**:
  1. **Managed a dataset comprising millions of medical papers, detailing paper publishing institutions sourced from wos/scopus/deminson. While wos featured institutional abbreviations, the latter two sources predominantly showcased full names, albeit with notable omissions. The project necessitated correlating every paper to its respective institution’s full name.**
* **Key Steps**:

1. **Initially segregated organizational data into distinctive name and address categories via a binary classification model.**
   2. **Mapped English abbreviations to full English names based on spatial information derived from varied sources.**
2. **Refined subdivision rules, culminating in the production of 140,000 high-quality English abbreviation-full name pairs, fortifying project delivery.**

## *Project 5. US patent text matching*

* **Project Duration**: 2022/10-2022/12
* **Project Description**:

1. **This project is the latest kaggle competition with 34k labeled data, and the label is the similarity score of two patent phrases**
2. **The competition requires the model result and the Pearson correlation coefficient of the label as the evaluation index**

* **Key Steps**:

1. **Discover the semantic information in the training data, combine the two phrases to be matched with domain information, such as the chemical domain, and enrich the input of the model;**
2. **Two frameworks of text matching and text classification were built to achieve this task, using the deberta/bert pre-training model;**
3. **Text matching uses CosineSimilarity to fit the score of the label, using MSEloss as the loss function;**
4. **In the text classification, the Linear function is finally used to map the result to a 5-dimensional vector, and CrossEntropyloss is used as the loss function;**
5. **Finally, the pearson coefficient on the training set can reach 0.79, and the gold medal scheme on kaggel is 0.87.**

## *Project 6. Multi-label classification*

* **Project Duration**: 2022/6-2022/9
* **Project Description**:

1. **Identify key events in sales chat, such as customer satisfaction points, complaint points, etc.**
2. **Supervised training, initial labels are obtained based on rules and manual annotations**

* **Key Steps**:

1. **Ensure that the distribution is as balanced as possible during the data sampling process, and use cleanlab to evaluate the quality of the label**
2. **Divide long conversations into short conversations through the QA model or multiple rounds of conversations, and then identify them**
3. **Call FastText and bert model, the f1 value of 6 categories has reached more than 80%, and it has been deployed online.**

## *Project 7. Knowledge Graph-Based Question Answering*

* **Project Duration**: 2021/12-2022/1
* **Project Description**:

1. **Store the information of Jay Chou’s works in the form of triples, then write them into cypher statements, and store them in neo4j**
2. **Then use regularization to extract entities, attributes, tags, etc. in natural language**
3. **Insert the extracted information into the template, which defines the cypher statement, and then query to get the result**

* **Key Steps**:

1. **Grab the entity list, construct triples, and separate entities, attributes, and labels from triple texts based on certain rules**
2. **In the problem of matching with the template, you can use Jaccard distance, edit distance, neural network and other methods**
3. **Think about upgrading to NER model to extract entities, or directly use the model to generate cypher sentences**

# Work Experience

## **1. China National Publications Import and Export (Group) Corporation**

**Duration**: October 2022 – Present

**Position**: NLP Algorithm Engineer

**Achievements**:

1. **Developed a 10B-scale large model training framework.**
2. **Successfully extracted tables and images from research paper PDFs, achieving over 95% accuracy for table extraction and surpassing 80% for image extraction.**
3. **Analyzed the addressing conventions in medical papers, and utilized a combination of neural networks and rule-based techniques to extract 140,000 pairs of correspondences between common institutional abbreviations and their full names.**

---

## **2. Megaview Technology**

**Duration**: June 2022 – September 2022

**Position**: NLP Algorithm Intern

**Achievements**:

1. **Identified pivotal events during sales sessions using models such as FastText and BERT.**
2. **Authored statistical tools to evaluate ASR (Automatic Speech Recognition) efficiency.**
3. **Managed the cleansing and processing of tens of millions of dialogue data.**


# **Self-Evaluation**

* **Communication**: Skilled in conveying ideas effectively and understanding others.
* **Logic**: Possess robust logical reasoning and problem-solving abilities.
* **Responsibility**: Highly accountable with a strong sense of duty towards tasks and roles.
* **Learning Ability**: Quick to grasp new concepts and adapt to new environments.
