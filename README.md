# OOPSmini_project

# 🎯 Student–Job Skill Analysis System

A beginner-friendly Python mini-project that analyzes how well a student's technical skills match a job description. It calculates a **skill match percentage**, identifies matching skills, and highlights missing skills to help students understand their job readiness.

Built using **Python and Object-Oriented Programming (OOP)** concepts, this project uses only core Python without any external libraries or database.

## ✨ Features

- 👨‍🎓 Store student profiles and technical skills.
- 💼 Define job descriptions with required skills.
- 📊 Calculate the percentage of matching skills.
- ✅ Identify skills that match the job requirements.
- ❌ Detect missing skills that students can learn.
- 🔄 Support case-insensitive skill comparison.
- 🧹 Normalize skill names by removing extra spaces and duplicates.
- 🛡️ Handle edge cases, including empty skill lists and zero required skills.
- 🧩 Demonstrate inheritance, encapsulation, abstraction, and polymorphism.
- 🐍 Use core Python features without external dependencies.

## 🛠️ Technologies Used

- **Programming Language:** Python
- **Concepts:** Object-Oriented Programming (OOP)
- **Modules:** Core Python only
- **Data Structures:** Lists
- **Control Flow:** Loops and conditional statements
- **Database:** Not required

## 📁 Project Structure

```text
student_job_analyzer/
├── main.py          # Sample data and program execution
├── models.py        # StudentProfile and JobDescription classes
├── analyzers.py     # Skill analysis and score calculation
├── manager.py       # Coordinates analysis and displays reports
└── README.md        # Project documentation
```

## 🚀 Getting Started

### Prerequisites

Install Python 3 on your system.

Check your Python installation:

```bash
python --version
```

### Installation and Execution

**1. Clone the repository**

```bash
git clone <your-repository-url>
```

**2. Navigate to the project directory**

```bash
cd student_job_analyzer
```

**3. Run the application**

```bash
python main.py
```

No additional package installation is required.

## ⚙️ How It Works

1. Create a student profile with the student's name and technical skills.
2. Define a job description containing the required skills.
3. Normalize the skill names by trimming spaces, converting them to lowercase for comparison, and removing duplicates.
4. Compare the student's skills with the job's required skills.
5. Calculate the match percentage.
6. Identify the missing skills.
7. Display a complete student–job skill analysis report.

## 📐 Match Score Formula

The match score is calculated using the following formula:

**Match Percentage = (Matching Skills / Total Unique Required Skills) × 100**

For example, if a job requires five unique skills and the student possesses two of them:

```text
Match Percentage = (2 / 5) × 100
                 = 40%
```

If a job has no required skills, the match score is set to **0%** to prevent division by zero.

## 📋 Sample Output

```text
STUDENT–JOB SKILL ANALYSIS REPORT

Student Name: Gamana

Job Title: Python Developer

Required Skills: 5

Matching Skills:
- Python
- SQL

Missing Skills:
- Django
- REST API
- Git

Match Score: 40%

Explanation:
The student matches 2 out of 5 unique required skills.
Therefore, the skill match percentage is 40%.
```

*Note: The output depends on the sample student profile and job description configured in `main.py`.*

## 🧱 Object-Oriented Programming Concepts

### 1. Encapsulation
Stores student and job information inside classes and provides getter methods to access the data.

### 2. Inheritance
`MatchScoreCalculator` and `MissingSkillDetector` inherit from the abstract base class `SkillAnalyzer`.

### 3. Abstraction
The `SkillAnalyzer` class defines a common `analyze()` interface for different skill analysis operations.

### 4. Polymorphism
The `Manager` class calls the same `analyze()` method on different analyzer objects, allowing each object to perform its specific task.

### 5. Single Responsibility Principle
Each class has a clear responsibility, making the code easier to understand, maintain, and extend.

## 🧪 Edge Cases Tested

- No matching skills
- All required skills present
- Partial skill match
- Student with no skills
- Job with no required skills
- Uppercase and lowercase skill names
- Leading and trailing spaces
- Duplicate student skills
- Duplicate job skills
- Both skill lists empty

## 🎓 Learning Outcomes

By completing this project, I gained practical experience in:

- Designing classes and objects in Python.
- Implementing inheritance and polymorphism.
- Understanding abstraction and encapsulation.
- Working with lists, loops, and conditional statements.
- Applying string normalization and duplicate removal.
- Implementing basic validation and edge-case handling.
- Organizing Python programs into multiple modules.
- Developing a simple, reusable, and maintainable application.

## 🔮 Future Enhancements

- Add a graphical user interface using Tkinter.
- Support multiple students and job descriptions through user input.
- Generate personalized recommendations for missing skills.
- Export analysis reports to CSV or PDF.
- Add a web interface for students and recruiters.
- Introduce weighted skill matching based on job importance.

## 👩‍💻 Author

**Deepa Bhavyasri Sonti**

B.Tech – Computer Science and Engineering

GitHub: [Deepabhavyasrisonti](https://github.com/Deepabhavyasrisonti)

## 📄 License

This project is intended for educational and learning purposes. You may adapt and extend it for your own practice.
