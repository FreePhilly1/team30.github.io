# Predicting NCAA Basketball Game Results
## ML4641 - Team 30
### Introduction
National sports, and notably college basketball, has proliferated throughout society and has garnered millions of fans throughout the world. With NCAA basketball becoming a premier form of entertainment, it becomes important to be able to predict these games for several reasons. In today’s literature, several machine learning models have been formed specifically for predicting the outcome of team sport games. Bunker and Thabtah [1] analyzed the proficiency of using artificial neural networks to predict outcomes of games and found the average performance of this model to be around 67.5%. Fialho et al. [2] reviewed different models such as artificial neural networks and support vector machines when applied to soccer and suggested that neural networks over the other methods due to their higher accuracy. Jain and Kaur [3] used Caret algorithm to pre-process the data then used Boruta algorithm for features selection. With these studies in mind, an effective plan for developing a predictive model for NCAA basketball games can be made.
### Problem Definition
With sports betting finding immense popularity in today’s society it becomes desirable to investigate whether machine learning techniques can be applied to gain an advantage. A successful predictive model would lead to huge financial implications in a lucrative industry.
### Methods
To determine the outcome of a game, we will perform binary classification (win vs loss) between two teams using the input data of player and team statistics. We can obtain such datasets on various player and team statistics through the NCAA developer API. We will experiment with three methods:
1. Decision Trees/Ensembles: we will first experiment with a single decision tree to predict the game outcomes. Because decision trees are white-box algorithms, we can then determine if it is necessary to implement decision tree ensembles. We will start with the sci-kit learn package, but if necessary we may transition to a specialized decision tree library such as XGBoost.
2. Support Vector Machines: we will train an SVM to linearly separate two teams into winner and loser classes. If we determine that nonlinearity may improve the prediction model, we can then apply the kernel trick. We will use sci-kit learn to implement SVM.
3. Neural Network: we will separate NCAA player/team statistics with their corresponding win or loss into training and testing datasets, where the testing dataset will validate the learned predictor function. We will use a Multilayer Perceptron (MLP) with 3 hidden layers, but we will also experiment with the optimal value of hidden layers. We will implement the MLP with the PyTorch package.

### Potential Results and Discussion
To evaluate each method, we will measure the accuracy and the F1 score. Because decision trees often perform better for tabular data compared to other machine learning techniques, we expect that decision trees would be the best method for predicting NCAA game outcomes. However, we also expect SVMs to perform well given that they are robust prediction models, and we only intend to use the tools for binary classification which works well for SVMs. It is unlikely that neural networks would yield strong results because they would require an enormous amount of (clean) data to perform well.
### Proposed Timeline
### Contribution Table
## Contributions

| Contributor                    | Task                                                                     |
|--------------------------------|--------------------------------------------------------------------------|
| Alvin Fabrio                   | Created Gantt chart and assisted members in performing other tasks. Prepared the presentation and one of the members that performed it.                                                       |
| Phillip Kim                    | Jeevan George                                                            |
| Jerred Chen                    | Christian Lee, Nicholas Tan, Leonard Thong                               |
| Jun Yi Chuah                   | Christian Lee, Nicholas Tan, Leonard Thong                               |
| Alexa Hanna                    | Yan Huang                                                                |
| Contributions                  | Yan Huang                                                                |
| Presentation                   | Yan Huang and Jeevan George                                              |
| GitHub Repository Setup        | Nicholas Tan                                                             |
| GitHub Page Setup              | Nicholas Tan, Jeevan George, and Leonard Thong                           |
| Review and Edit                | Jeevan George, Christian Lee, Nicholas Tan, Leonard Thong, and Yan Huang |
| References                     | Jeevan George, Christian Lee, Nicholas Tan, Leonard Thong 

Member | Contribution
------ | ------
Alvin Fabrio | Created Gantt chart and assisted members in performing other tasks. Prepared the presentation and one of the members that performed it.
Phillip Kim | Wrote the introduction/background and problem definition. Researched articles to provide details about the background of the NCAA and statistics of already existing predictive models for the sport. Also one of the members who participated in the presentation of our proposal.
Jerred Chen | Provided the techniques to train our model and methods for data classification. Also went in depth about the details of the potential results, discussing how we will be able to measure the accuracy of our model.
Jun Yi Chuah | Researched many of the articles used in the background and problem definition. Also assisted with writing the potential results and discussion with the researched articles.
Alexa Hanna | Created the contribution table and powerpoint presentation. Filled in each member’s contribution within the table and also filled in most of the information within the presentation. Also one of the presenters for the proposal video.

### References
[1] R. P. Bunker and F. Thabtah, “A machine learning framework for sport result prediction,” Applied Computing and Informatics, vol. 15, no. 1, pp. 27–33, Jan. 2019, doi: https://doi.org/10.1016/j.aci.2017.09.005.

[2] G. Fialho, A. Manhães, and J. P. Teixeira, “Predicting sports results with Artificial Intelligence – A proposal framework for soccer games,” Procedia Computer Science, vol. 164, pp. 131–136, 2019. 

[3] S. Jain and H. Kaur, "Machine learning approaches to predict basketball game outcome," 2017 3rd International Conference on Advances in Computing,Communication & Automation (ICACCA) (Fall), Dehradun, India, 2017, pp. 1-7, doi: 10.1109/ICACCAF.2017.8344688.
