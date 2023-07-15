# Student Result Analysis
This repository contains an analysis of the student results dataset. The dataset provides information about students' demographics, parental education, test preparation, and scores in various subjects.

## Usage
To run the analysis, ensure that the required libraries (numpy, pandas, matplotlib, seaborn) are installed. The student results dataset should be saved as a CSV file named "Student_results.csv" in the same directory.
<br> Execute the code in a Python environment such as Jupyter Notebook or any Python IDE. The results will be displayed through various charts and summaries.
<br> Feel free to modify the code and adapt it to your own dataset or add additional analyses as needed.

## Dataset
The dataset used for this analysis is stored in the `Student_results.csv` file. It contains the following columns:

- `Gender`: Gender of the student
- `EthnicGroup`: Ethnic group of the student
- `ParentEduc`: Education level of the student's parent
- `LunchType`: Type of lunch the student has
- `TestPrep`: Test preparation status
- `ParentMaritalStatus`: Marital status of the student's parent
- `PracticeSport`: Sports practice status
- `IsFirstChild`: Indicates if the student is the first child in the family
- `NrSiblings`: Number of siblings the student has
- `TransportMeans`: Mode of transportation used by the student
- `WklyStudyHours`: Number of weekly study hours
- `MathScore`: Score in Math subject
- `ReadingScore`: Score in Reading subject
- `WritingScore`: Score in Writing subject

## Analysis and Visualizations

### Data Insights

Before diving into the analysis, let's get some insights into the dataset by loading and examining the data:

```python
import pandas as pd

df = pd.read_csv("Student_results.csv")
print(df.head())
print(df.describe())
print(df.info())
print(df.isnull().sum())
```

### Gender Distribution

![download](https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/7945d81f-7a2c-4e13-83bb-070c42225e85)
![download](https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/419b9760-da9a-4107-a876-cfe817c4ca17)

- The analysis reveals the distribution of students based on gender. It shows that there are more females than males in the dataset.

### Parent's Effect on Student's Education

#### Parent Education

![download](https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/4e245581-916a-4a6d-b2dd-303944c23595)

- The analysis examines the relationship between parent education and student scores. It suggests that parent education has a positive impact on their child's education (scores).

#### Parent Marital Status

![download](https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/d3445dca-868e-473c-b59b-d9a7532b7b54)

- The analysis explores the impact of parent marital status on student scores. It suggests that there is no significant effect based on parent marital status.

### Individual Score Analysis

<p float="left">
    <img src="https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/9e8f1e79-c2ea-43a6-8fb3-0b9490445d01" alt="Image 1" width="200" />
    <img src="https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/1bd47992-3a9b-4fca-b18e-8eac7b9ae2a7" alt="Image 2" width="200" />
    <img src="https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/245493f4-9014-4b74-9bc1-f71f380ea0a4" alt="Image 3" width="200" />
    <img src="https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/e5714f34-adf9-4f58-ac85-b999b629de5f" alt="Image 4" width="400" />
    <img src="https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/abe23d8e-81ed-48ca-aa71-87a6f7b1958c" alt="Image 5" width="200" />
    <img src="https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/259d424d-3996-48f0-a213-67828efa5e81" alt="Image 6" width="300" />
</p>

- The analysis focuses on the distribution of scores in Math, Reading, and Writing subjects. The box plots and violin plots provide insights into the spread and central tendency of the scores. Math appears to be relatively more challenging compared to the other subjects.

### Ethnic Groups Distribution

![download](https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/42ea767b-2f74-4637-9012-a26552c7fdc3)
![download](https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/26bd6810-6fc1-4c1d-8c6f-e7e8aecb9ec6)


- The analysis visualizes the distribution of students across different ethnic groups. It gives an overview of the representation of each group in the dataset.

### Scores Analysis based on different parameters

#### Average Scores by Test Preparation

![download](https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/2bc6c575-3907-4003-8e9d-91e8e9adad9f)

- The analysis compares the average scores of students based on their test preparation status. It shows that students who completed test preparation tend to have higher average scores compared to those who did not.

#### Average Scores by Lunch Type

![download](https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/119fa93a-3758-4c2e-ac0c-ee002eff8d38)

- The analysis investigates the relationship between lunch type and student scores. It demonstrates that students who have a standard lunch tend to have higher average scores compared to those with a free/reduced lunch.

#### Average Scores: First Child vs. Other Siblings

![download](https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/30e705d1-b783-421c-9f41-48a32305f633)

- The analysis examines the impact of having siblings on student scores. It suggests that there is no significant effect based on whether the student is the first child or has siblings.

#### Average Scores by Sports Practice

![download](https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/508e892d-6168-426e-b357-0861c1579cfa)

- The analysis explores the relationship between sports practice and student scores. It indicates that students who regularly practice sports tend to have better average scores compared to those who do not participate in sports.

#### Average Scores by Transportation Means

![download](https://github.com/BhaskarAcharjee/Student-Result-Analysis/assets/76872572/16865ce6-25d4-4940-a9f6-aae34b8a2089)

- The analysis investigates the impact of transportation means on student scores. It shows that the mode of transportation does not have a significant effect on average scores.


### Conclusion

The analysis of the student results dataset leads to the following conclusions:

- There are more females than males in the dataset.
- Higher levels of parent education are associated with higher average scores.
- There is no significant effect based on parent marital status.
- Math appears to be relatively more challenging compared to other subjects.
- Ethnic Group A has the lowest average scores, while Ethnic Group E has the highest average scores.
- Test preparation leads to higher average scores.
- Having a standard lunch is associated with higher average scores.
- Regular sports practice leads to better average scores.
- The mode of transportation does not show a significant impact on student average scores.

For detailed code and analysis, please refer to the Jupyter Notebook or Python script in this repository.
