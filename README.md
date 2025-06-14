# 🧾 Multi-Step Survey Form
🔗 [Live Demo](https://replit.com/@Ravikantmahi/Multi-Step-Survey-Form)

A beautiful, responsive, and animated **multi-step form** designed for user surveys. Built using **HTML**, **CSS**, and **JavaScript**, this form guides users through multiple sections with progress tracking and smooth transitions.

> 🛠 Developed by [Ravi Kant](https://github.com/Ravikantmahi)

---

## ✨ Features

- ✅ 4-Step animated form with sliding transitions
- ✅ Progress bar with interactive steps
- ✅ Input fields for personal, contact, and educational info
- ✅ Final step includes dropdown and comments section
- ✅ Form submits data via [FormSubmit](https://formsubmit.co/) to your email
- ✅ Custom alert and reset on submission

---

## 📸 Demo

| Steps | Form |
|-------|------|
| ![Progress Bar](https://user-images.githubusercontent.com/placeholder/progress.gif) | ![Form UI](https://user-images.githubusercontent.com/placeholder/form.gif) |

---
```
## 🛠️ Tech Stack

| Technology | Usage |
|------------|-------|
| `HTML5`    | Form Structure |
| `CSS3`     | Layout, Design, Animations |
| `JavaScript` | Slide logic and validations |
| `Font Awesome` | Icons in progress bar |
| `FormSubmit` | Email form submission |

---
```
## 🚀 How It Works

### 🔁 Form Steps

1. **Basic Info** → First and Last Name  
2. **Contact Info** → Email and Phone  
3. **Education** → College and Branch  
4. **Other Info** → Domain and Suggestions  

Each step has:
- Slide animation
- "Next" and "Previous" buttons
- Progress indicator (`active` classes handled via JS)

### ✅ Submission

- On clicking **Submit**, all steps are marked complete  
- `alert()` confirms success  
- Form resets with `location.reload()`

---

## 🧩 Project Structure

```bash
multi-step-form/
├── index.html       # Main form HTML
├── style.css        # CSS styling and animations
├── script.js        # JS logic for transitions and form flow
└── README.md        # This documentation
```
🧠 Key Code Concepts
📦 HTML
```
 <form action="https://formsubmit.co/your-email" method="POST">
  <!-- Multi-step form pages here -->
</form>
```
🎨 CSS
```
.step .bullet.active,
.step .check.active {
  background: #3498db;
  color: white;
}
.slide-page {
  transition: margin-left 0.5s ease;
}
```
🧠 JavaScript
```
nextBtnFirst.addEventListener("click", function(event){
  event.preventDefault();
  slidePage.style.marginLeft = "-25%";
  bullet[current - 1].classList.add("active");
  current += 1;
});
```
📬 Submission Handler
You can customize the email in the HTML:
```
<form action="https://formsubmit.co/YOUR_EMAIL_HERE" method="POST">
```

---
© 2023 Made with 🌍 by Ravi Kant
