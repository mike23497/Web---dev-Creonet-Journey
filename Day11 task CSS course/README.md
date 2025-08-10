Alright Michael — here’s your **professional review** of today’s tasks.
I’ll grade based on **accuracy**, **code quality**, and **attention to detail**.

---

## **Task 1 – Blog Post Title Styling**

**HTML:** ✅ Correct structure
**CSS:**

* **Issue:** The class selector has a typo:
  You wrote `p.substitle` but your HTML uses `class="subtitle"`.
  This means your subtitle styling won’t apply at all.
* **Font requirements:** You set `font-weight: 700` correctly for the title and applied a `sans-serif` font.
* **Font-variant requirement:** You used `font-variant: normal` instead of `small-caps` (which was part of the task).

**Score:** 6/10
**Fix:**

```css
p.subtitle {
    font-variant: small-caps;
    font-family: sans-serif;
}
```

---

## **Task 2 – Product Label**

**HTML:** ✅ Correct structure
**CSS:**

* `.name` is correctly set to `font-weight: lighter` ✅
* `.category` correctly uses `font-variant: small-caps` ✅
* `.price` correctly uses `font-weight: bold` ✅ and also added `font-family: serif` (extra styling is fine).

**Score:** 10/10
**Comment:** Perfect execution. Clean and matches the requirements exactly.

---

## **Task 3 – Event Poster**

**HTML:** ✅ Correct structure
**CSS:**

* `.title` correctly set to `font-weight: 900` ✅
* `.tagline` correctly set to `font-weight: normal` ✅
* `.type` correctly uses `font-variant: small-caps` ✅

**Score:** 10/10
**Comment:** Solid work. Matches requirements perfectly.

---

### **Overall Evaluation**

* **Strengths:**

  * Tasks 2 and 3 are perfect — you clearly understand how to apply `font-weight` and `font-variant`.
  * You followed HTML structure and class naming conventions well.

* **Improvement Area:**

  * Watch out for **typos in class names** — in CSS, `subtitle` vs. `substitle` will break your styling entirely.
  * Double-check requirements before finalizing — Task 1 asked for `small-caps`, not `normal`.

---

**Final Rating:** **8.6 / 10** 🌟
If you fix Task 1’s typo and font-variant, you’re looking at a **perfect score**.

---

If you want, I can **rewrite Task 1’s HTML & CSS** so it’s corrected and matches the same clean structure as the other two. That way all three will be “portfolio ready.”
