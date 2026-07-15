# Lab: Build "Newton," an AI Study Coach in Copilot Notebooks
 
Build a source grounded, persona driven AI coach that helps students learn Newton's Laws of Motion, using only the materials you give it.
 
> **Note on the screenshots:** each image below lives in the `images/` folder of this repo. Swap a file in that folder (same filename) to update the screenshot without touching this file.
 
## What you'll need
- Microsoft 365 Copilot (with a OneDrive or SharePoint license)
- A supplementary PDF ("ID267")
- Two images of study notes on Newton's Laws (page 1 and page 2), hosted on GitHub for students to download
- A textbook excerpt covering Newton's three laws (Word, PDF, or OneNote page)
## The one rule to remember
Apply Newton's custom instructions **after** the image extraction step (Step 5). The instructions tell Copilot to use *only* the notebook's sources, so if they're switched on when you feed it a raw image, it may refuse the image.
 
---
 
### Step 1 — Download the lab assets
![Repo file list](images/step-01-download-assets.png)
 
1. Download all three files (direct links, main branch):
   - **ID267.pdf** — https://github.com/SamuelBoulanger/student-notebook-workshop/raw/main/ID267.pdf
   - **notes-page-1.png** (notes, page 1) — https://github.com/SamuelBoulanger/student-notebook-workshop/raw/main/notes-page-1.png
   - **notes-page-2.png** (notes, page 2) — https://github.com/SamuelBoulanger/student-notebook-workshop/raw/main/notes-page-2.png
2. The PDF link downloads automatically. The two image links will open in the browser instead, right-click the link (or the opened image) and choose **Save Link As...** / **Save Image As...** to save each one.
![Right-click Save Image As](images/SaveImageAs.png)
 
3. Keep them somewhere easy to find, you'll upload each one into the notebook in the next steps.
---
 
### Step 2 — Create and name the notebook
![New notebook button](images/step-02-new-notebook.png)
 
1. Open **Microsoft 365 Copilot → Notebooks → New notebook**.
2. Name it **Newton's Laws – Study Coach**.
3. You'll see the three pane layout: **sources** (left), **content** (middle), **Copilot chat** (right).
---
 
### Step 3 — Upload the PDF source
![Add sources panel with PDF](images/step-03-add-pdf.png)
 
1. In the left pane, choose **Add sources** and add the PDF you downloaded (**ID267.pdf**).
2. Do this before anything else in the notebook, later steps depend on this source already being present.
---
 
### Step 4 — Create a page *inside* the notebook
![New page highlighted](images/step-04-new-page.png)
 
1. In the left pane, choose **New page**. Title it **My Notes from the Image**.
2. Open **Copilot in the side pane** so it's ready for the next step.
3. **Key point:** create the page *here, in the notebook*, not from a separate Copilot chat. A page born inside the notebook is usable right away, with no sync or indexing wait.
---
 
### Step 5 — Turn the two photos into notes
![Notes images attached in Copilot](images/step-05-extract-notes.png)
 
1. In the Copilot side pane, attach or paste **both notes images** you downloaded in Step 1 (**notes-page-1.png** and **notes-page-2.png**).
2. Use this prompt:
```
Extract the text from these two pages of notes and turn it into clean,
organized study notes on Newton's Laws.
```
 
3. **Result:** two messy photos become clean, organized study notes in the chat response.
---
 
### Step 6 — Add the extraction to a page
![Extracted notes saved to page](images/step-06-save-to-page.png)
 
1. Ask Copilot to save the notes it just produced onto the page you created in Step 4:
```
Save the result on the page "My Notes from the Image."
```
 
2. **Result:** the page now holds your clean, organized study notes, ready to use as a source.
---
 
### Step 7 — Add your remaining sources
![Add sources panel with textbook](images/step-07-add-sources.png)
 
1. In the left pane, choose **Add sources** and add your **textbook excerpt**.
2. This is Copilot's "library," the material it's allowed to read.
---
 
### Step 8 — Give Copilot its persona (Newton)
![Copilot instructions dialog](images/step-08-instructions.png)
 
1. Select the **expand button next to the notebook name** (upper left) → **Copilot instructions**.
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
 
### Step 9 — Check that it's grounded
![Cited answer and fallback message](images/step-09-grounded-check.png)
 
1. Ask an **in-source** question:
```
What is Newton's Second Law, and which source does it come from?
```
 
2. Then ask something **off-topic**:
```
Who won the 2018 World Cup?
```
 
3. **Expect:** a cited answer that names the source file, and for the off-topic question, exactly: *"I cannot find this information in the notebook sources."* That contrast is the "aha": the coach is bounded by your materials.
---
 
### Step 10 — Generate study aids
![Quick create Study Guide menu](images/step-10-study-guide.png)
 
1. From **Quick create / Study Guide** in the left pane, generate in order: **Summary page → Topic pages → Flashcards**.
2. Notice the flashcards include content that exists *only* in the PDF, proof the source added back in Step 3 reached every tool.
---
 
### Step 11 — Reflect
![Finished notebook with all pages](images/step-11-finished.png)
 
- Where did a citation make you trust an answer more?
- What happened when you asked something outside the sources, and why is that a good thing?
- Which study aid (Summary, Topic, Flashcards) would you use the night before a test, and why?
