# 🧪 Static Review Summary

## ✅ What I Reviewed

I reviewed two components of the image gallery project:

1. **requirements.md** — a documentation file outlining functional and non-functional requirements for a web-based image gallery.
2. **gallery.html** — the implementation file containing HTML and JavaScript code for the image gallery UI and logic.

---

## 🐛 Types of Issues Found

- **Documentation clarity issues** — vague requirements, unclear terms, or redundancy in the wording.
- **Accessibility** — missing `alt` attributes for images and lack of screen reader considerations.
- **Maintainability** — some inline styles and hardcoded logic in the JavaScript could be improved for better separation of concerns.
- **Logic issues** — some functions lacked input validation or error handling.

---

## 💭 Reflection on Static Testing Process

Static review helped me deeply understand the structure and intent of the application without running the code. I learned that:

- Reading code line by line encourages you to think about **intent and consequences**.
- It can be challenging to spot subtle bugs without execution, especially logic flaws.
- Requirements review forced me to think like an end-user — whether features were described clearly enough to be implemented and tested.

---

## 📚 Assignment Questions

### 📌 Question 1: Documentation Review

- **Are all features in `requirements.md` clearly defined?**  
  Mostly, yes — the document is well-structured with functional and non-functional requirements separated. However, some terms like "look good visually" were subjective and could be clarified.

- **Were there unclear, missing, or contradictory elements?**  
  - "Look good visually" (FR1.3) was too vague.
  - Filtering should “update immediately” (FR2.3), but the expected behavior on slow networks or invalid categories wasn't clarified.

- **What improvements did you suggest?**  
  - Suggested clarifying vague phrases.
  - Recommended explicitly defining accessibility expectations like `alt` tags and keyboard navigation.

---

### 📌 Question 2: Code Review

- **Summarize the 3 PR comments you made:**  
  1. Suggested adding `alt` attributes to `<img>` tags to improve accessibility.  
  2. Noted that inline styling in JavaScript should be replaced with CSS classes for maintainability.  
  3. Highlighted the lack of input validation in the `filterImages()` function.

- **Why are they important to resolve?**  
  - Accessibility ensures all users, including those with disabilities, can access content.
  - Maintainability improves the ability to update and scale the project.
  - Validation helps prevent bugs and improves robustness.

---

### 📌 Question 3: Reflection

- **What aspects of the requirements or code were unclear or problematic?**  
  - Subjective phrasing in requirements.
  - Some JavaScript logic was tightly coupled to the DOM and lacked error handling.

- **Did you identify any missing validations, assumptions, or inconsistencies?**  
  - Missing checks for undefined or invalid category filters.
  - Assumption that all images load successfully without fallback handling.

- **What challenges did you face during static review, and what did you learn?**  
  - Hard to identify runtime issues without executing the code.
  - Learned how important precise documentation and separation of concerns are in a project.

---
