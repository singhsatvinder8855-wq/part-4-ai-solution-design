# Part 4: AI Solution Design Report

## Task 1: Choose a Business Domain

### Selected Domain
For this project, I chose the **Education** domain.

---

## Task 2: Define the Business Problem

### What Problem is Being Solved?
I am designing a solution to predict and manage **student dropout risk**. The goal is to identify students who are struggling before they actually drop out of their courses.

### Users or Stakeholders
- Academic advisors  
- Teachers  
- Student success teams at the university  

### Current Manual or Traditional Process
Currently, advisors manually check spreadsheets, attendance records, assignment submissions, and midterm grades to identify students who may need extra support.

### Limitations of the Current Process
- Manual processing takes up to **567 hours per month**
- Average case resolution time reaches **44.7 hours**
- Human errors increase the error rate up to **11.16%**
- Some at-risk students may be missed due to delayed or incomplete analysis

---

## Task 3: Identify the AI Task Type

### AI Task Type
**Classification**

### Why This AI Task Type is Suitable
Classification is suitable because the system needs to categorize students into groups such as:
- High Risk
- Low Risk

The AI model will provide a clear prediction about whether a student is likely to drop out or not.

---

## Task 4: Data Requirement Plan

### Type of Data Needed
The system requires:
- Attendance data
- Assignment data
- Assessment and quiz scores

### Structured or Unstructured Data
The project will use **structured data** stored in tables and spreadsheets.

### Input Features
Examples of input features include:
- Attendance percentage
- Number of missing assignments
- Average quiz marks
- Midterm scores
- Student participation records

### Target Variable or Labels
The target variable will indicate:
- `1` = Student dropped out
- `0` = Student did not drop out

### Data Collection Method
Data can be collected automatically from:
- Learning Management Systems (LMS) such as Moodle or Canvas
- University student databases

### Data Quality Risks
Possible risks include:
- Missing attendance records
- Delayed grade uploads
- Incorrect or incomplete data entries

These issues can reduce prediction accuracy.

---

## Task 5: Model Recommendation

### Recommended Model
**Feed-forward Neural Network**

### Why This Model is Appropriate
A feed-forward neural network works well with structured numerical data. It can identify hidden patterns between student performance and dropout behavior.

For example:
- Low attendance + poor quiz scores + missing assignments may indicate a high dropout risk.

The model can learn these complex relationships better than traditional rule-based methods.

---

## Task 6: Evaluation Plan

### Technical Metrics
The model will be evaluated using:
- Recall
- Intervention Success Rate

Recall is important because the system should identify as many at-risk students as possible.

### Business Metrics
Success will be measured by:
- Reduction in manual processing hours
- Faster case resolution time
- Lower human error rates

### Possible Failure Cases
One possible issue is:
- A student may be incorrectly flagged as high-risk after a temporary poor performance due to illness or personal issues.

### Human Review Process
The AI system will only generate risk alerts. Final decisions will always be reviewed by human academic advisors before taking action.

---

## Task 7: Responsible AI Considerations

### Possible Risks
The major risks include:
- Label bias
- Over-monitoring students
- Privacy concerns

Historical data may contain biases that unfairly affect certain groups of students.

### Risk Mitigation Plan
To reduce these risks:
- Only academic performance data will be used
- Personal demographic data will be excluded
- Human oversight will remain part of the process
- Student privacy policies will be followed

---

## Task 8: Final Solution Summary

### Problem
Manual student monitoring is slow, resource-intensive, and prone to errors.

### Proposed AI Solution
Develop a classification-based AI system that automatically identifies students who are at risk of dropping out.

### Required Data
- Attendance records
- Assignment submissions
- Assessment and quiz results

### Recommended Model
Feed-forward Neural Network

### Expected Business Impact
- Save hundreds of hours of manual work
- Improve student support response time
- Reduce human errors
- Increase student retention rates

### Risks and Mitigation
Potential risks such as bias and privacy concerns will be handled through:
- Limited data usage
- Human validation
- Ethical AI practices