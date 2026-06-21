# 🧠 AM II: AI Study Assistant & Second Brain

![Course](https://img.shields.io/badge/Course-Analytical%20Mechanics%20II-blue)
![Semester](https://img.shields.io/badge/Semester-Spring%202026-brightgreen)
![Professor](https://img.shields.io/badge/Professor-Ali%20Akbar%20Abolhasani-orange)

Welcome to the ultimate **AI-powered Study Assistant** for the **Analytical Mechanics II (AM II)** midterm exam! This repository is configured to act as a "Second Brain," helping students master concepts, tackle complex problems, and secure maximum marks.

## 🎯 Project Overview

This repository configures an AI agent to act as an expert academic tutor specifically tailored for our AM II course. Instead of giving generic internet answers, the AI is constrained by strict guidelines (found in `AGENTS.md`) and a custom `exam-solver` workflow to ensure its output is perfectly aligned with the class material.

### ✨ Key Features

- **📚 Source Prioritization:** The AI exclusively prioritizes our specific course materials. It searches through the `lecture_notes/` and `textbook/` directories before answering any question.
- **🕵️ Trap & Trick Detection:** The AI is trained to actively look for edge cases, subtleties, and "tricks" in exam questions that might mislead students.
- **💯 Exam-Quality Solutions:** Every generated answer is formulated as a step-by-step, comprehensive solution aimed at earning a 100% score on the midterm.
- **🔄 Professor vs. Textbook:** Where applicable, the AI compares Prof. Abolhasani's specific methods with the standard textbook approaches.

## 📂 Repository Structure

- `AGENTS.md`: The core rulebook containing the strict instructions for the AI behavior.
- `.agents/workflows/exam-solver.md`: The step-by-step workflow the AI follows to solve exam problems flawlessly.
- `lecture_notes/`: Directory for Prof. Abolhasani's class notes and slides. *(Place the PDFs/images here)*
- `textbook/`: Directory for the course reference book. *(Place the textbook PDF here)*

## 🚀 How to Use (For Classmates)

1. **Clone the Repository:** Download or clone this repository to your local machine.
2. **Add Materials:** Ensure you populate the `lecture_notes/` and `textbook/` folders with the relevant course files.
3. **Use an AI IDE / Agent:** Open this workspace in an Agentic AI IDE (like the one you are currently using) that supports workspace context and custom `.agents` instructions.
4. **Ask Away:** Start asking midterm practice questions! You can invoke the `exam-solver` workflow to get step-by-step analytical solutions based exactly on what we learned this semester.

## 🤝 Contribution

Feel free to fork this repository, add more summarized notes, or tweak the AI instructions (`AGENTS.md`) if you find a better prompt format. Let's ace this midterm together! 🚀

---
*Created for the students of the Spring 2026 AM II class.*
