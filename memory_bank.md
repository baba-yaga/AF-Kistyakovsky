# Project Memory Bank

## 1. Project Overview
*   **Project Name:** AF Kistyakovsky Landing Page
*   **Purpose:** A single-page presentation website for A. F. Kistyakovsky, focusing on his biography, legacy/family, and works. It aims to be short, lively, and without academic heaviness, with a warm, respectful, and conversational tone.
*   **Technologies:** HTML, CSS (with specific color palette and typography), JavaScript (implied for animations and interactive elements).
*   **Design Principles:** Vintage autumn palette, system sans-serif typography, 1200px container, responsive grid for hero section and son cards, soft animations (`.reveal`, `.float`), accessibility (contrast, focus styles, alt-texts).
*   **Associated Remote URL:** `https://github.com/baba-yaga/AF-Kistyakovsky.git`

## 2. File Structure (Key Directories and Files)
*   `.` (Root Directory)
    *   `design_brief.md`: Project design brief.
    *   `index.html`: Main landing page HTML.
    *   `index1.html`, `index2.html`: Possibly alternative or older versions of the landing page.
    *   `README.md`: Project README.
    *   `styles.css`: Main CSS file for styling.
    *   `assets/`: Directory for various assets.
        *   `.gitignore`: Git ignore file for assets.
        *   `АлександраИвановна и сыновья.docx`: Document.
        *   `О_дневнике_КистяковскогоАФ.docx`: Document.
        *   `Предисловие.pdf`: PDF document.
        *   `images/`: Image assets.
            *   `Alex Fed with Alex Alex.jpg`
            *   `alexandra_and_six_sons_ps.jpg`
            *   `alexandra_and_six_sons.jpg`
            *   `alexandra_and_six_sons.psd`
            *   `Alexandra-Ivanovna_ps.jpg`
            *   `family_af.jpg`
            *   `fzm-canvas_texture-03.jpg`
            *   `grave.jpg`
            *   `Kistiakovskie 1.tif`
            *   `kistyakovsky_af.jpg`
            *   `александр.jpg`
            *   `богдан.jpg`
            *   `борис.jpg`
            *   `владимир.jpg`
            *   `игорь.jpg`
            *   `юлий.jpg`
        *   `sons/`: Directory possibly related to individual sons.
            *   `_template.html`: HTML template.
            *   `Bogdan_Alexandrovich.jpg`
            *   `Igor_Alexandrovich.jpg`
            *   `Vladimir_Alexandrovich.jpg`
            *   `Yuly_Alexandrovich.jpg`
    *   `Stitch design/`: Another design-related directory.
        *   `index.html`
        *   `screen.png`

## 3. Important Notes/Conventions
*   **Multiple `index.html` files:** (`index.html`, `index1.html`, `index2.html`) suggest different versions or stages of development. `index.html` is the main landing page.
*   **Visual Content:** Extensive use of image assets (`assets/images`, `assets/sons`) indicates a visually rich project, focused on displaying historical/biographical content.
*   **Document Assets:** Documents (`.docx`, `.pdf`) in `assets/` suggest content that might be integrated or referenced on the landing page.
*   **Templating:** The presence of `_template.html` in `assets/sons` implies a templating approach for individual "son" pages, though currently, the son cards in `index.html` link to `#`.
*   **CSS Variables:** `styles.css` defines a comprehensive set of CSS variables for colors, border-radius, shadow, and font families, ensuring consistent styling.
*   **Responsive Design:** The CSS includes media queries for responsive layouts, adapting to different screen sizes for navigation, hero section, and son grid.
*   **Animations:** CSS classes like `.reveal` and `.float` are used for soft entrance animations and subtle floating effects on images.
*   **Accessibility:** Basic accessibility features are included, such as `sr-only` for screen readers and `focus-visible` styles for keyboard navigation.
*   **Content Rules:** Specific content rules are outlined in `design_brief.md` regarding historical facts (e.g., "Права..." publication details) and mentions of descendants.

## 4. Key Code Snippets
### CSS Color Tokens (from `styles.css`)
```css
:root{
  --bg:#f4e9d8; --paper:#fbf4ea; --ink:#2a1e19; --sepia:#6b4a39;
  --maroon:#8f1d2e; --orange:#e37f2d; --saffron:#f0be62;
  --sky:#8ab6d6; --teal:#2f7d76; --muted:#7b675c;
  --radius:18px; --shadow:0 12px 30px rgba(42,30,25,.18);
  --display:"Cormorant Garamond","Cormorant","Garamond","Times New Roman",serif;
}
```
### HTML Structure for a Son Card (from `index.html`)
```html
<a class="son" href="#">
  <figure class="portrait sepia">
    <img src="assets/images/владимир.jpg" alt="Владимир Кистяковский" loading="lazy" />
  </figure>
  <h3 style="margin:10px 0 4px;font-size:18px">Владимир Кистяковский</h3>
  <small>1865-1952</small>
</a>
```
