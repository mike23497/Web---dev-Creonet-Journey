Alright — we’ll make this a quick skill check for your **CSS text-align** (horizontal) and **vertical alignment** knowledge.

---

### **3 Practice Tasks**

1. Create a paragraph of text and center it horizontally on the page.
2. Make a heading (`<h1>`) aligned to the right horizontally.
3. Place text inside a container and center it both horizontally and vertically.

---

### **5 Fill-in-the-Gap Questions**

1. The CSS property used to align text horizontally is `_text-align_`.
2. To center text horizontally inside a block element, set `text-align` to `_center_`.
3. The property `vertical-align` works inside `___inline table_____`-level or table-cell elements.
4. To align text vertically in the middle of a table cell, use `vertical-align: ____baseline____`.
5. `text-align: justify;` makes text align to both the left and right edges by adjusting the `____space____` between words.

---
Corrections
Alright, let’s go through this like a real professional code review — I’ll break it into **rating**, **errors/issues**, and **professional improvement suggestions**.

---

## **1. Professional Rating**

* **Code structure:** 8/10 — clean, logical, and readable, with proper indentation.
* **Class naming:** 7/10 — clear for the most part, but could be more descriptive.
* **CSS organization:** 8/10 — selectors are clear, grouped logically.
* **Concept application:** 9/10 — correct use of `text-align` and `vertical-align: sub`.

---

## **2. Errors / Issues**

### HTML:

* **Section naming:** `<section class="hori">` is unused in CSS — dead class.
* The `vertical-align` example (`span.sub`) is fine, but your task mentioned *vertical centering*, and `sub` is not vertical centering; it’s for subscript positioning.
* `<title>` is “Document” — should reflect the content for good practice.

### CSS:

* Your `vertical-align` fill-in-the-gap answers are partly wrong:

  * Q3 should be “inline **or** table-cell” — not “inline table.”
  * Q4 should be “middle” for vertical centering, not “baseline” (baseline is default, not middle).
* Missing demonstration of **vertical centering inside a table-cell** or flexbox — which is a more practical application.

---

## **3. Professional Suggestions**

### **HTML**:

* Give sections semantic names (e.g., `horizontal-center-section`, `right-align-header`) to make your code self-explanatory.
* Add more practical vertical alignment examples, like text in a `div` that’s centered both ways.

### **CSS**:

Instead of just using `vertical-align: sub`, you can also show `vertical-align: middle` inside a container:

```css
.container {
    display: table-cell;
    vertical-align: middle;
    height: 200px;
    width: 100%;
    text-align: center;
}
```

Or using Flexbox (modern approach):

```css
.container {
    display: flex;
    justify-content: center; /* horizontal */
    align-items: center;     /* vertical */
    height: 200px;
}
```

---

✅ **Corrected Fill-in-the-Gap Answers:**

1. `text-align`
2. `center`
3. `inline or table-cell`
4. `middle`
5. `space`

---



