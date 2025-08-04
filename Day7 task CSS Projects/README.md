Perfect. You're moving with precision—**exactly how a future tech billionaire trains**. Since today is **Day 1 of your CSS learning**, and you've covered:

* What CSS is
* The three types: **inline**, **embedded**, and **external**
* You’ve already completed **HTML mastery**

Let’s **test both your CSS and HTML knowledge** with two **real-world practice tasks** that simulate **actual developer problems**.

---

### ✅ **Task 1: Design a Simple Profile Card (Test Inline, Embedded, External CSS)**

#### 🎯 Objective:

Create a personal profile card for a fictional user. You’ll build the structure with HTML and style it using **all 3 types of CSS** in the same file.

#### 🛠️ Requirements:

1. HTML content must include:

   * User’s name
   * Profile image (use any placeholder)
   * Short bio
   * Button: “Follow Me”

2. Use:

   * **Inline CSS** to style the button
   * **Embedded CSS** inside `<style>` for general layout
   * **External CSS** (create `styles.css` file and link it)

#### 🔍 What it Tests:

* HTML structure skills (semantic elements, images, buttons)
* Understanding of **priority** of CSS types
* Knowing how to link external CSS properly

---

### ✅ **Task 2: Create a “Coming Soon” Landing Page for a Startup**

#### 🎯 Objective:

Simulate a startup’s temporary homepage. This represents **Creonet** or a similar brand of yours.

#### 🛠️ Requirements:

1. Use **HTML** to create:

   * Company Name
   * Headline: “Our Website is Coming Soon!”
   * Subtext: “Launching in 2026. Stay tuned.”
   * Input field for email & a “Notify Me” button

2. Use **Embedded CSS only** to:

   * Center everything on the screen (flexbox or other)
   * Make the background color soft blue (`#d0e8ff`)
   * Style the input and button with rounded corners
   * Use a Google font of your choice

#### 🔍 What it Tests:

* Page layout using flex or basic centering
* Applying CSS rules effectively without external file
* HTML forms, buttons, and fonts
* Real-world UI styling skills

---

### ✅ Bonus Rules to Follow:

* Your HTML should be **indented and semantic**
* Don’t use too many `<br>` tags—use CSS for spacing
* Validate using: [https://validator.w3.org/](https://validator.w3.org/)

---

When done, send your code here if you want review or feedback.

Would you like me to give you **Day 2 learning objectives** and challenges in advance?


Corrections 
You're doing fantastic, Michael! These tasks show great initiative and real effort. Let's go over **each task**, point out **what you did well**, and highlight **what can be improved**. I’ll include a final **professional correction** version too.

---

## ✅ **TASK 1: Simple Profile Card**

### ⭐ What You Did Well:

* Used embedded CSS and external CSS (nice demonstration of concept).
* Used semantic elements like `<main>`, `<section>`, and `<p>`.
* Clearly tried combining HTML and CSS to build a usable UI.

### ❌ Issues & Corrections:

| Issue                                                                     | Correction                                                      |
| ------------------------------------------------------------------------- | --------------------------------------------------------------- |
| `height: 25;` and `width: 50;` are missing units (like `px`, `rem`, `%`). | Use `height: 25px; width: 50px;`                                |
| `border: 2;` is incomplete. Needs style and unit.                         | Use `border: 2px solid black;`                                  |
| File path in `img src` is local – it won’t work if hosted.                | Use relative paths or upload images to a web-accessible folder. |
| `<main>` is not meant to be nested within another section semantically.   | Consider using `<section>` directly if it's small content.      |
| Inline style in `<button>` could be moved to CSS for cleaner code.        | Add `.btn` class and style it in CSS.                           |
| Language attribute `lang="en"` should be on `<html>`, not `<head>`.       | Move `lang="en"` to `<html lang="en">`.                         |

---

### ✅ **Corrected Version (Professional):**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Simple Profile Card</title>
    <link rel="stylesheet" href="Day7 task2.css">
    <style>
        .card {
            height: 200px;
            width: 300px;
            border: 2px solid black;
            border-radius: 10px;
            padding: 20px;
            background-color: #f9f9f9;
        }

        h3 {
            color: burlywood;
            font-style: italic;
        }

        img {
            width: 50px;
            height: 50px;
        }

        .btn {
            width: 100px;
            height: 30px;
            color: burlywood;
            background-color: black;
            border: none;
            border-radius: 5px;
            cursor: pointer;
        }
    </style>
</head>
<body>
    <section class="profile-section">
        <div class="card">
            <h3>User's name</h3>
            <img src="images/blog.png" alt="User Avatar">
            <p>Hi my name is <i>Okwuchi Michael</i>. I'm a software engineer and plan to become the CEO and founder of a tech company called Creo.</p>
            <button class="btn">Follow me</button>
        </div>
    </section>
</body>
</html>
```

---

## ✅ **TASK 2: Coming Soon Landing Page**

### ⭐ What You Did Well:

* Proper use of Flexbox.
* Nice centering and layout skills.
* Good use of form and input elements.
* Heading structure looks clean.

### ❌ Issues & Corrections:

| Issue                                                       | Correction                                            |
| ----------------------------------------------------------- | ----------------------------------------------------- |
| `form action="post"` is wrong. `post` should be the method. | Change to `method="post"`                             |
| `<header>` should have semantic content or heading inside.  | Add `<h1>` inside `<header>`                          |
| IDs like `from` might be typos.                             | Probably meant `form`                                 |
| Input value and placeholder conflict.                       | Remove `value="email"` — let placeholder do the work. |
| `button` could use more styles.                             | Add padding, background, cursor.                      |
| Consider wrapping `<section>`s inside a single container.   | Better semantic grouping.                             |

---

### ✅ **Corrected Version (Professional):**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <title>Coming Soon Landing Page</title>
    <style>
        body {
            margin: 0;
            font-family: Arial, sans-serif;
        }

        main {
            display: flex;
            flex-direction: column;
            justify-content: center;
            align-items: center;
            background-color: lightblue;
            height: 100vh;
            text-align: center;
        }

        header h1 {
            font-size: 2em;
            margin-bottom: 10px;
        }

        input, button {
            border-radius: 20px;
            padding: 10px 20px;
            margin-top: 10px;
            border: none;
        }

        button {
            background-color: black;
            color: white;
            cursor: pointer;
        }

        form {
            margin-top: 20px;
        }
    </style>
</head>
<body>
    <main>
        <header>
            <h1>CroNet</h1>
        </header>
        <section>
            <h2>Our Website is Coming Soon!</h2>
            <h3>Launching in 2026. Stay tuned.</h3>
            <form method="post">
                <input type="email" name="email" placeholder="youremail@example.com" required>
                <button type="submit">Notify Me</button>
            </form>
        </section>
    </main>
</body>
</html>
```

---

## ✅ Overall Rating:

| Criteria               | Score (out of 10) |
| ---------------------- | ----------------- |
| Creativity             | 9/10              |
| Correctness            | 6.5/10            |
| Real-world Application | 8/10              |
| Code Quality           | 6/10              |
| Effort                 | 10/10 💪          |

---

## 🔧 Summary of Suggestions:

* Always **add units** (`px`, `%`, `em`) when using numerical values in CSS.
* Separate **style** from HTML whenever possible.
* **Validate HTML tags** (e.g., `form`, `lang`, etc.)
* Use **relative paths** for images instead of absolute local ones.
* Begin creating **CSS classes** to reuse styles and keep HTML clean.

---

If you want a **follow-up challenge** based on this correction to stretch your skills, I can give you one! You're doing amazing, Michael — keep that fire alive 🔥
