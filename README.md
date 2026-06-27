# Modern Interactive Personal Portfolio

A premium, dynamic, and dark-themed personal portfolio website built using vanilla **HTML5**, **CSS3**, and **JavaScript (ES6+)**. The website is designed to be fully customizable, high-performance, and deployable instantly on **GitHub Pages**. 

All visual content (biography, education history, work experience, skills, and projects) is dynamically driven from a single configuration file, making updates straightforward.

## 🚀 Live Demo
Visit the live site: [gokulkrishnar.github.io/portfolio/](https://gokulkrishnar.github.io/portfolio/)

---

## ✨ Features

- **Dynamic Content Injection**: Update your portfolio by editing a single configuration file ([portfolio-data.js](portfolio-data.js)) without touching HTML tags.
- **Interactive Canvas Backdrop**: A lightweight, high-performance HTML5 canvas particle background that moves organically and draws glowing cyan trails to the visitor's cursor.
- **Typewriter Role Cycle**: Dynamically types and erases customizable career roles in the hero section.
- **Project Filter System**: Instantly filter projects by domain (e.g. AI & ML, Web Apps, Data Science) using smooth transitions.
- **Web3Forms Contact Integration**: A fully functional AJAX-powered contact form that validates input and delivers messages directly to your inbox using Web3Forms.
- **Ambient Neon Glows**: Smooth glassmorphic containers overlaying subtle, blurred cyan and purple backdrops.
- **Responsive Layout**: Designed for mobile, tablet, and desktop viewports, with a slide-out drawer menu for mobile navigation.
- **Clean Scroll reveals**: Custom scroll intersections that fade elements into view gracefully.

---

## 🛠️ Project Structure

```bash
├── index.html          # Semantic HTML skeleton & Web3Forms integration
├── style.css           # Custom CSS variables, glassmorphic styling, & responsiveness
├── portfolio-data.js   # Centralized portfolio data (Edit this to update content!)
├── script.js           # Rendering engine, particles canvas, and form handler
└── assets/
    ├── logo.svg        # Site favicon & brand representation
    └── resume.pdf      # Downloadable CV asset
```

---

## ⚙️ How to Update Your Portfolio

You do not need to edit `index.html` to add new experience or projects. Simply open [portfolio-data.js](portfolio-data.js) and modify the Javascript object keys:

### 1. Personal Information & Socials
Modify the `personalInfo` block to update your name, tagline, email, locations, and social media handles:
```javascript
personalInfo: {
  name: "Gokul Krishna R",
  shortName: "GKR",
  tagline: "...",
  email: "gokulkrishnar04@gmail.com",
  linkedin: "https://www.linkedin.com/in/GokulKrishnaR04",
  github: "https://github.com/GokulKrishnaR",
  resumeUrl: "assets/resume.pdf",
  location: "Kochi, Kerala, India"
}
```

### 2. Typewriter Roles
Edit strings in the `roles` array to change the roles typed out in the hero section:
```javascript
roles: [
  "Machine Learning Engineer",
  "Data Analyst",
  "AI Developer",
  "Federated Learning Researcher"
]
```

### 3. Timeline (Experience & Education)
Add or remove entries from the `experience` and `education` lists. They render automatically into a side-by-side vertical timeline layout:
```javascript
experience: [
  {
    role: "Data Analytics Intern",
    company: "IBM SkillsBuild",
    duration: "December 2024",
    details: "..."
  }
]
```

### 4. Technical Skills
Group your capabilities into domains. Each category supports custom FontAwesome icons (e.g. `fa-code`, `fa-brain`, `fa-cubes`):
```javascript
skills: [
  {
    category: "AI & Machine Learning",
    icon: "fa-brain",
    items: ["Machine Learning", "Deep Learning", "NLP"]
  }
]
```

### 5. Projects & Tags
Add your project showcases. Ensure the `category` matches the group filter tabs you want to display:
```javascript
projects: [
  {
    title: "AI Resume & Portfolio Builder",
    description: "...",
    category: "Web Apps",
    tags: ["LLMs", "Python", "Gradio"],
    githubUrl: "https://github.com/...",
    liveUrl: "https://..."
  }
]
```

---

## 📬 Contact Form Configuration

To route form messages to your personal inbox:
1. Go to [Web3Forms](https://web3forms.com/) and register a free account using your email.
2. Get your `Access Key`.
3. Open [index.html](index.html) and locate the hidden input field inside the `<form>` element:
   ```html
   <input type="hidden" name="access_key" value="YOUR_ACCESS_KEY_HERE">
   ```
4. Replace `YOUR_ACCESS_KEY_HERE` with your Web3Forms access key.

---

## 📄 License
This repository is open source and available under the [MIT License](LICENSE).

---
© 2026 Gokul Krishna R.
