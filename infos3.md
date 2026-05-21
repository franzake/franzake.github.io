You are editing my AcademicPages/Jekyll GitHub website.

Goal: redesign the Publications page into a compact, modern academic publication list similar to Yann Dubois’ website style.

Repository:
https://github.com/franzake/franzake.github.io

Current problem:
- My Publications page is too bulky.
- Publication cards are oversized.
- BibTeX/code blocks are visible and too large.
- A broken --- appears on the page.
- The layout does not look like a clean academic website.

Target design:
- One unified “Publications” list.
- No “Conference Papers” section.
- Compact horizontal publication entries.
- Optional thumbnail on the left.
- Text content on the right.
- Clean title, authors, journal, year, and short summary.
- Small links below each entry: Paper, DOI, Scholar, Code, PDF if available.
- No visible BibTeX blocks by default.

Use my Google Scholar profile as reference:
https://scholar.google.com/citations?user=2ShbCuEAAAAJ&hl=fr

Use my ORCID:
https://orcid.org/0000-0003-0192-0370

For each publication, use this visual structure:

html <div class="publication-item">   <div class="publication-thumbnail">     <img src="/images/publications/example.png" alt="Paper preview">   </div>   <div class="publication-content">     <h3>Publication title</h3>     <p class="authors"><strong>Ake, F.</strong>, Author 2, Author 3, et al.</p>     <p class="venue">Journal Name, Year</p>     <p class="summary">One concise sentence summarizing the contribution.</p>     <p class="pub-links">       <a href="#">Paper</a> ·       <a href="#">DOI</a> ·       <a href="#">Google Scholar</a> ·       <a href="#">Code</a>     </p>   </div> </div> 

CSS requirements:
css .publication-item {   display: flex;   gap: 22px;   padding: 24px 0;   border-bottom: 1px solid rgba(150,150,150,0.25);   max-width: 950px; }  .publication-thumbnail img {   width: 190px;   height: 120px;   object-fit: cover;   border-radius: 6px; }  .publication-content h3 {   margin-top: 0;   margin-bottom: 6px;   font-size: 1.1rem;   font-weight: 700; }  .publication-content p {   margin: 4px 0; }  .authors {   font-size: 0.95rem; }  .venue {   font-weight: 600; }  .summary {   font-size: 0.95rem; }  .pub-links a {   font-size: 0.9rem;   font-weight: 600; }  @media (max-width: 700px) {   .publication-item {     flex-direction: column;   }    .publication-thumbnail img {     width: 100%;     height: auto;   } } 

Tasks:
1. Edit _pages/publications.md.
2. Remove broken ---.
3. Remove all giant BibTeX/code blocks.
4. Remove oversized cards and colored badges.
5. Create a compact publication list using the structure above.
6. Use accurate publication metadata from Google Scholar.
7. Keep the page GitHub Pages/Jekyll compatible.
8. Keep styling clean, modern, and readable in dark mode.
9. If thumbnails are unavailable, use a neutral placeholder image or omit the thumbnail.
10. Do not create publication categories or filters.
