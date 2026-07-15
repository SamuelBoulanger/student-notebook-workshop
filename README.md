# Lab: Build "Newton," an AI Study Coach in Copilot Notebooks

Build a source-grounded, persona-driven AI coach that helps students learn Newton's Laws of Motion — using only the materials you give it.

> **Note on the image placeholders:** each `🖼️` line marks where a screenshot goes, with a suggested filename. Replace it with your own capture before publishing.

## What you'll need
- Microsoft 365 Copilot (with a OneDrive or SharePoint license)
- An image of study notes on Newton's Laws (a photo or screenshot)
- A textbook excerpt covering Newton's three laws (Word, PDF, or OneNote page)
- A supplementary PDF ("ID267") for later

## The one rule to remember
Apply Newton's custom instructions **after** the image step (Step 5). The instructions tell Copilot to use *only* the notebook's sources — so if they're switched on when you feed it a raw image, it may refuse the image.

---

### Step 1 — Create and name the notebook
> 🖼️ *screenshot:* the **New notebook** button in Microsoft 365 Copilot · `step-01-new-notebook.png`

1. Open **Microsoft 365 Copilot → Notebooks → New notebook**.
2. Name it **Newton's Laws – Study Coach**.
3. You'll see the three-pane layout: **sources** (left), **content** (middle), **Copilot chat** (right).

---

### Step 2 — Create the notes page *inside* the notebook
> 🖼️ *screenshot:* left pane with **New page** highlighted · `step-02-new-page.png`

1. In the left pane, choose **New page**. Title it **My Notes from the Image**.
2. **Key point:** create the page *here, in the notebook* — not from a separate Copilot chat. A page born inside the notebook is usable right away, with no sync or indexing wait.

---

### Step 3 — Turn the image into notes
> 🖼️ *screenshot:* the notes image attached in Copilot, notes appearing on the page · `step-03-extract-notes.png`

1. Attach or paste your notes image into the notebook's Copilot chat.
2. Use this prompt:

```
Read this image and turn it into clean, organized study notes on
Newton's Laws. Put the result on the page "My Notes from the Image."
```

3. **Result:** a messy image becomes structured notes on your page in seconds — no sources or setup required yet.

---

### Step 4 — Add your sources
> 🖼️ *screenshot:* the **Add sources** panel with the textbook file listed · `step-04-add-sources.png`

1. In the left pane, choose **Add sources** and add your **textbook excerpt**.
2. This is Copilot's "library" — the material it's allowed to read. (You'll add the PDF later, in Step 7.)

---

### Step 5 — Give Copilot its persona (Newton)
> 🖼️ *screenshot:* the **Copilot instructions** dialog with the persona pasted in · `step-05-instructions.png`

1. Select the **expand button next to the notebook name** (upper-left) → **Copilot instructions**.
2. Paste the block below, then **Save** (you can edit it anytime):

```
You are Newton, a Physics Learning Coach for 16-year-old STEM
students studying Newton's Laws of Motion.

GROUNDING
- Use only information from this notebook's sources (student notes,
  textbook, and any added PDFs). Cite the source file name when you use it.
- If the answer isn't in the sources, say exactly:
  "I cannot find this information in the notebook sources."
- If a question is outside physics / Newton's Laws, gently steer the
  student back to the topic.

TEACHING STYLE
- Explain clearly and step-by-step, in language a high-school STEM
  student understands.
- Define every technical term before you use it.
- Encourage curiosity and critical thinking; guide toward the answer
  rather than just handing it over.

SOLVING PROBLEMS
- Show each calculation step and the reasoning behind it.
- Always include units and state the formula used.
- Flag common mistakes when they are relevant.

QUIZZES (use this format instead of the one below)
- Draw only from notebook content.
- Give questions at three levels: Easy, Medium, Challenging (2 each).
- Put all answers in a separate Answer Key at the end.

FORMAT for concept and problem answers (not quizzes):
1. Short Answer
2. Explanation
3. Source Used
4. Check Your Understanding (one question back to the student)

TONE: Positive, encouraging, and patient. Focus on helping students
learn, not just giving answers.
```

---

### Step 6 — Check that it's grounded
> 🖼️ *screenshot:* a cited answer next to the "I cannot find this…" fallback · `step-06-grounded-check.png`

1. Ask an **in-source** question:

```
What is Newton's Second Law, and which source does it come from?
```

2. Then ask something **off-topic**:

```
Who won the 2018 World Cup?
```

3. **Expect:** a cited answer that names the source file — and, for the off-topic question, exactly: *"I cannot find this information in the notebook sources."* That contrast is the "aha": the coach is bounded by your materials.

---

### Step 7 — Add the PDF, then generate study aids
> 🖼️ *screenshot:* **Quick create / Study Guide** menu with Summary, Topic pages, Flashcards · `step-07-study-guide.png`

1. Add the PDF (**ID267**) as a new source.
2. From **Quick create / Study Guide** in the left pane, generate in order: **Summary page → Topic pages → Flashcards**.
3. Notice the flashcards include content that exists *only* in the PDF — proof the new source reached every tool.

---

### Step 8 — Reflect
> 🖼️ *screenshot (optional):* the finished notebook with all pages in the left pane · `step-08-finished.png`

- Where did a citation make you trust an answer more?
- What happened when you asked something outside the sources — and why is that a good thing?
- Which study aid (Summary, Topic, Flashcards) would you use the night before a test, and why?
