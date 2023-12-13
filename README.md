# Project Repository

This repository contains code and data for a financial news analysis project. Below is a brief description of the directories and files present in this repository:

## Data Directory
1. **KnowledgeGraph**: Stores node tables and relationship tables of the knowledge graph used for Task2-Q3 and Task2-Q4 inputs.
2. **model**: Holds trained BERT and BiLSTM models, receiving outputs from Task1-Q2-part2 and PreliminaryExperiment-Task1-Q2-part2.
3. **News_input**: Contains company information JSON files and original input news tables for various stages of Task1.
4. **News_output**: Stores interim output files for different stages of Task1.
5. **Result_dataset**: Holds final output files for various stages, also converting Task1 outputs into Task2 inputs.
6. **Training_dataset**: Stores input and output files for the steps involved in designing the model for Task1-Q2.

## Core Code Files
1. **Task1-Q1_NoiseRemoval**: Addresses the first question's task, processes raw data, and accurately removes noise to obtain "training domain data" for data labeling and model training in the second question. Also obtains "application domain data" for sentiment analysis in the second question using a two-stage noise removal process.
2. **Task1-Q2-part1_TrainingSampleAnnotation**: Completes the second question's first stage—data labeling task.
3. **Task1-Q2-part2_BilstmModelTraining**: Accomplishes the second question's second stage—model training task.
4. **Task1-Q2-part3_BilstmModelApplication(Task1.xlsxGot)**: Completes the second question's third stage—applies sentiment analysis models and obtains the final results for Task1: A-share company-related news binary sentiment analysis result data table—Task1.xlsx.
5. **Task2-Q3_ConstructingNeo4jKnowledgeGraph**: With a configured Neo4j database, running this file constructs information from the KnowledgeGraph into a knowledge graph structure.
6. **Task2-Q4_KnowledgeDrivenFinancialAnalysis(Task2.xlsxGot)**: Utilizes information from Task1.xlsx and the KnowledgeGraph for knowledge discovery, generating the final results for Task2: Table detailing the impact on explicitly and implicitly affected companies in A-share-related news—Task2.xlsx.

## Auxiliary Code Files
1. **PreliminaryExperiment-Task1-Q1-E1nE2_PreliminaryMatchingStrategy**: Pre-experiment for Q1, used to explore filtering strategies for relevant news.
2. **PreliminaryExperiment-Task1-Q2-part2-E1_HighConfidenceBERTTunning** and **PreliminaryExperiment-Task1-Q2-part2-E2_(COLAB)FullDataBERTTunning**: Pre-experiments for Q2, used to explore BERT fine-tuning approaches and their final effects, aiding in model strategy decisions.
