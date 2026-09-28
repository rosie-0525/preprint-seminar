# Algebraic Geometry Preprint Seminar

Static site for the Stanford algebraic geometry preprint seminar (Fridays 3–4 pm, Autumn 2026). Everything is in `index.html`; there is no build step.

## Updating the schedule

Each talk is one `<tr>` in the schedule table. The `data-date` attribute (YYYY-MM-DD) drives the highlighting: past talks are greyed out and the next upcoming talk is marked automatically.

To add a paper to a talk, replace the `TBA` span in the paper cell:

```html
<td class="paper">
  <a href="https://arxiv.org/abs/2509.01234">Title of the paper</a>
  <span class="arxiv">arXiv:2509.01234</span>
</td>
```

To set the room, edit the `Where` entry in the header.

## Hosting

Upload `index.html` anywhere static files are served (a departmental web directory, GitHub Pages, etc.). The only external dependency is the STIX Two Text font from Google Fonts; without it the page falls back to Times.
