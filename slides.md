---
marp: true
title: Software Product Documentation
author: Sharath
paginate: true
theme: default
---

<!-- Custom Theme -->
<style>
section {
  font-family: "Inter", sans-serif;
  padding: 32px;
}
h1, h2 {
  color: #0a3d62;
}
strong {
  color: #1e3799;
}
.code-box {
  background: #f3f3f3;
  padding: 12px;
  border-radius: 8px;
}
</style>

<!-- _class: lead -->

# Software Product Documentation  
### Technical Presentation (Marp)

**Contact:** 21f3000557@ds.study.iitm.ac.in

---

# Introduction

This presentation outlines:

- Product architecture  
- System components  
- Complexity analysis  
- API examples  
- Marp-based documentation workflow  

---

# Why Use Marp?

- Git-friendly Markdown  
- Supports custom themes  
- Math (KaTeX), code, tables  
- Exports: **PDF**, **HTML**, **PPTX**, **PNG**  
- Easy to maintain across teams  

---

<!-- BACKGROUND IMAGE SLIDE -->
![bg cover](images/background.jpg)

# Architecture Overview

This slide demonstrates a local background image:  
`images/background.jpg`

---

# Algorithmic Complexity

### Example: Time Complexity

Inline: `O(n \log n)`

Block:

$$
T(n) = 5n^2 + 2n + 7
$$

### Recurrence Example

$$
T(n) = 2T\left(\frac{n}{2}\right) + n
$$

Master Theorem:

$$
T(n) = O(n \log n)
$$

---

# API Example

```python
class AuthService:
    def login(self, username, password):
        user = db.find_user(username)
        if user and user.verify(password):
            return generate_token(user.id)
        return None
