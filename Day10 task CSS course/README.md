Great job finishing today's CSS lesson on `font-family`, `font-size`, and `font-style`! Let’s test your understanding with **3 beginner-friendly real-world tasks** and **5 fill-in-the-gap questions** based on what you’ve learned today.

---

### ✅ **Task 1: Personal Bio Page**

**HTML**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="bio.css">
    <title>Personal Bio</title>
</head>
<body>
    <section>
        <h1>Michael Okwuchi</h1>
        <p>I am a future tech billionaire. I love building impactful things with code.</p>
    </section>
</body>
</html>
```

**Your Task in `bio.css`:**

* Set a `font-family` of your choice (e.g., `'Courier New'`, `'Arial'`, `'Georgia'`) for the entire page.
* Make the `h1` heading larger than the paragraph.
* Apply a **italic font style** to the paragraph.

---

### ✅ **Task 2: Newsletter Signup**

**HTML**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="newsletter.css">
    <title>Newsletter Signup</title>
</head>
<body>
    <header>
        <h2>Join Our Newsletter</h2>
        <p>Get tech tips and tutorials weekly.</p>
    </header>
</body>
</html>
```

**Your Task in `newsletter.css`:**

* Use a **sans-serif font** for the entire document.
* Set the `h2` font-size to `24px`.
* Use a **different font-style** (e.g., `oblique`) for the paragraph than the heading.

---

### ✅ **Task 3: Product Description**

**HTML**

```html
<!DOCTYPE html>
<html lang="en">
<head>
    <meta charset="UTF-8">
    <meta name="viewport" content="width=device-width, initial-scale=1.0">
    <link rel="stylesheet" href="product.css">
    <title>Product Card</title>
</head>
<body>
    <div class="product-card">
        <h2>Noise Cancelling Headphones</h2>
        <p class="description">Immerse yourself in sound like never before.</p>
    </div>
</body>
</html>
```

**Your Task in `product.css`:**

* Set a different `font-family` for the heading and the paragraph.
* Make the heading bold and the paragraph italic.
* Adjust the paragraph’s font-size to 16px.

---

### ✍️ **Fill in the Gap Questions**

1. The `font-family` property defines the fonts of text on a web page.
2. When using multiple fonts in `font-family`, the browser uses the supported available font in the list.
3. The `font-style` property allows you to style text as **normal**, italic or oblique.
4. To set text size in pixels, you use the `font-size` property with units like px or em.
5. If you want your text to fall back to a system font, always include a san serif font family at the end of the `font-family` list.

---

Chat Gpt Review
Excellent work, Michael! You're making strong progress. Let's go through your tasks and answers one by one, with specific feedback and corrections where needed 👇

---

## ✅ **TASK 1: Personal Bio**

### ✅ HTML:

* ✅ Structure and class use are clean.
* ⚠️ Minor note: You're assigning class `italic` to `<p>`, but in your CSS, you're using `p .italic` — which targets an element **inside** `<p>` with class `italic`.

### ❌ CSS:

```css
p .italic {
    font-size: 1.2em;
    font-style: italic;
}
```

This selector means: “an element inside a `<p>` with the class `italic`.” But your paragraph itself has the class, so it should be:

✅ **Correction:**

```css
p.italic {
    font-size: 1.2em;
    font-style: italic;
}
```

### ✅ General Feedback:

* You used font-family correctly.
* Font sizes are appropriate.
* Just fix the selector.

---

## ✅ **TASK 2: Newsletter Signup**

### ✅ HTML:

* Clean, semantic, and properly linked.

### ✅ CSS:

```css
body {
    font-family: sans-serif;
    font-size: 16px;
}
header.newsletter {
    font-style: normal;
}
h2 {
    font-size: 1.5em;
}
p {
    font-style: oblique;
}
```

✅ You applied:

* A universal sans-serif family.
* A larger heading font-size (`1.5em = 24px` if base is 16px).
* Differentiated styles (normal vs oblique).

👏 Well done! No changes needed here.

---

## ✅ **TASK 3: Product Card**

### ✅ HTML:

* Correctly structured and classed.

### ✅ CSS:

```css
body {
    font-size: 16px;
}
.product-card h2 {
    font-family: helvetica, sans-serif;
    font-style: normal;
}
.description {
    font-family: arial;
    font-style: italic;
    font-size: 1em;
}
```

👍 Smart observation about `font-weight`. You're absolutely right — bold text is controlled via `font-weight`, which you haven’t covered yet. You're thinking like a dev — good!

🟢 Font-family and font-style were applied correctly.

🟡 Optional Tip:
To see clearer font contrast, try mixing **serif** and **sans-serif** fonts instead of two similar sans-serifs like Helvetica and Arial.

---

## ✍️ **FILL IN THE GAP**

Here’s what you submitted (with feedback):

1. ✅ **"The `font-family` property defines the fonts of text on a web page."**

   * ✅ Correct, though "appearance of text" or "typeface" is also acceptable.

2. ⚠️ **"The browser uses the supported available font in the list."**

   * ✅ The meaning is right, but to refine it:
     **Correction:** “...uses the **first available font** in the list.”

3. ✅ **"The `font-style` property allows you to style text as normal, italic or oblique."**

   * ✅ Perfect.

4. ✅ **"Use units like px or em."**

   * ✅ Correct. You can also use `rem` and `%`, but you nailed the key ones.

5. ⚠️ **"Include a san serif font family at the end."**

   * Minor spelling issue:
   * **Correction:** It should be: `sans-serif` (with hyphen and correct spelling).

---

## 🔚 Final Grade

| Section           | Score           |
| ----------------- | --------------- |
| Task 1            | 9/10            |
| Task 2            | 10/10           |
| Task 3            | 10/10           |
| Fill-in-the-blank | 4.5/5           |
| **Overall**       | **33.5 / 35** ✅ |

🔥 You're doing **amazing**, Michael. Keep learning consistently, and you'll master CSS in no time.

---

### 🚀 What’s Next?

Let me know when you’re done with your **next CSS lesson**, and I’ll prepare:

* More tasks
* Fill-in-the-blanks
* Optional “challenge task” to stretch your skills

You’re doing great — let’s keep this momentum going.

