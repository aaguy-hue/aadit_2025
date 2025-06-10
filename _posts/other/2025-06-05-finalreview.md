---
title: CSA Reflection
permalink: /blogs/finalreview
comments: true
layout: post
description: This is a deeper review on data types, wrapper classes and classes specific in preparation for using Data Structures.
author: Aadit Mathur
---

# AP CSA Final Reflection – My Personal Contributions

This year in AP Computer Science A has been one of the most collaborative and impactful programming experiences I’ve had. While I came into the class with prior experience, CSA challenged me to think about large-scale systems, backend architecture, and working on codebases that affect an entire class of students.

Here’s a detailed reflection on what I personally contributed to our Agile Toolkit project and what I learned throughout the process.

---

## 🧩 My Key Contributions

### 📊 Grading System Backend

I designed and implemented the backend infrastructure for handling grades:

- Built and optimized the **database tables** for tracking grades, grading status, feedback, and revision history.
- Implemented **API endpoints** to allow students, graders, and teachers to interact with grade data.
- Supported **secure user access** so that only authorized users could view or edit relevant data.
- Ensured clean separation of concerns and modular design for long-term maintainability.

---

### 📨 Grade Requests System

I built the **Grade Requests** system, which is essential for how peer grading works in **Team Teaches**:

- When a student teaches a lesson and grades another student’s homework, they **submit a Grade Request**.
- That request is **not final**—it needs to be reviewed and approved by the teacher before the grade is committed.
- I implemented the full logic and APIs behind:
  - **Submitting requests**
  - **Displaying pending approvals to the teacher**
  - **Approving/rejecting those requests**
- This system ensures **accountability and transparency** while still giving student teachers autonomy in grading.

---

### 🤝 Peer Grading for Team Teaches

I worked closely with **Rahul** and **Tarun** on the **Peer Grading** system specifically designed for **Team Teach presentations**:

- Enabled students to submit **peer evaluations** with numeric scores and written feedback.
- Integrated this with the Grade Requests system so that teachers could verify and approve any grades tied to these peer interactions.
- Ensured that the evaluations respected the structure of our grading model and didn’t conflict with other systems.

---

### 🗂️ Assignments and Submissions System

While I was not the lead on this feature, I contributed significantly to the **Assignments and Submissions** infrastructure:

- Helped implement the logic for:
  - Creating new assignments
  - Accepting student submissions
  - Tracking submission timestamps and revisions
- Contributed to the **data models** and **APIs** that support assignment listing, due dates, and status checks.
- Participated in debugging and performance tuning sessions to ensure a smooth user experience.

---

### 🔍 Code Reviews & Production Approvals

One of my ongoing responsibilities was **reviewing and approving pull requests (PRs)**—especially those headed to our deployed version:

- Reviewed all PRs for correctness, style, and performance before they were merged into production.
- Checked for regressions, unnecessary complexity, or untested features.
- Approved and merged PRs that affected critical systems like grading, authentication, and assignments.
- Helped teammates debug issues during reviews and suggested refactors when necessary.

This made me think critically not just about my own code, but about *maintaining quality and consistency across the entire codebase*.


## 🎓 Certificates (Foundational Skills)

### 🛠️ Agile Tools & Workflow Certificate
Demonstrated understanding of Agile methodologies, including Scrum roles, sprints, backlog management, and collaborative development tools.

### 🌐 Full-Stack System Design Certificate
Built and maintained a web-based system for managing assignments and grading, incorporating front-end interfaces, back-end logic, and database integration.

### 📋 Project Management Integration Certificate
Applied task tracking, project planning, and iterative updates to real classroom tools that affect both educators and students.

### 🔧 GitHub & Version Control Certificate
Used GitHub for collaborative work, including branching, merging, and issue tracking, as part of multi-member team development.


## 🪙 NFTs (Unique Contributions)

### 🧠 Assignment Engine Architect NFT
Designed and implemented a unique digital system to manage assignment creation, submission, and review, helping improve classroom workflow.

### 📊 Agile Dashboard Innovator NFT
Created or contributed to an interactive dashboard or toolkit that visualizes Agile metrics and improves team coordination.

### 🤝 Multi-Project Collaborator NFT
Worked across multiple group projects within the HyFlex framework, contributing to backend systems, API logic, or integrated workflows.

### 🎓 Education Impact NFT
Made a tangible impact on real educational environments through tools that support grading, scheduling, or student feedback.


---

## 🧠 What I Learned

- **Backend Design:** I learned how to design scalable, modular APIs and data structures that interact smoothly.
- **System Integration:** Building systems that rely on one another (e.g., Grade Requests, Assignments, Peer Grading) taught me how to manage dependencies and shared state.
- **Code Review Discipline:** Reviewing PRs sharpened my eye for bugs, technical debt, and architectural flaws.
- **Collaboration at Scale:** With nearly 50 people on the project, I learned how to communicate clearly and coordinate without blocking others.
- **Debugging Under Pressure:** I had to debug some stubborn issues under time constraints—often learning new techniques along the way

---

## 💬 Final Thoughts

This class has been much more than just an AP course—it’s been a simulation of working on a real development team. I’m especially proud of the backend infrastructure I helped build, and the role I played in reviewing and maintaining the code we deployed. While things haven't always been smooth, it's been a great experience.
