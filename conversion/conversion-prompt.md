Please convert the attached PDF or image (e.g., a scanned lecture board) into a single, fully accessible and structured HTML file.  

Requirements:

Document Structure
 - Use semantic HTML5 elements:
   - `<header>` for the document title or course info
   - `<main>` containing a single `<article>` with `aria-label="[Document Description]"`
   - Use a proper heading hierarchy: `<h1>`, `<h2>`, etc.
   - Use `<section>` for logical content blocks (e.g., Overview, Concepts, Equations, Recap)

Accessibility & WCAG Compliance
 - Add `role="document"` to the `<body>` and meaningful ARIA labels where needed
 - Include spoken-word descriptions below each math equation or visual question, inside an italicized paragraph with a class like `.spoken-description`
 - Use accessible image markup with:
   - `<figure>` and `<figcaption>`
   - Clear and descriptive `alt` text

Math & Formatting
 - Detect and format all math using MathJax:
   - Inline math: `\\( ... \\)`
   - Display math: `\\[ ... \\]`
   - Include this in `<head>`:
     ```html
     <script type="text/javascript" async src="https://cdn.jsdelivr.net/npm/mathjax@3/es5/tex-mml-chtml.js"></script>
     ```
 - Left-align all display equations (no bullets), using a class like `.equation`

Content Sections
 - Include these clear sections in order:
   1. Overview** – a short summary of the topic
   2. Concepts** – key ideas or rules with math
   3. Example Equations** – display equations and their spoken explanations
   4. Image or Figure** – show any chalkboard/screenshot with descriptive alt text
   5. Recap** – a short, intelligent summary placed at the end

Output Format
 - Provide a ZIP file containing:
   - The final `.html` file
   - Any referenced images with simplified filenames (e.g., `figure1.png`)

Bonus (Optional)
 - Add light CSS for readability:
   - Font: system-ui or Arial
   - Max width: `920px`
   - Reasonable spacing and color contrast

Make sure the HTML stands alone, is clean and production-quality, and adheres to accessibility and semantic standards.
