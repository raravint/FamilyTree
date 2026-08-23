# Version Updates

A running log of changes to the Family Tree application.

---

## Version 3.7 — July 2026

**New**

- **Lineage: repeated people are now marked.** When relatives married within the family, the same ancestor can be reached through more than one line and so appears more than once in the Lineage view. Every occurrence is now flagged with a dashed border and an *"↩ also shown"* badge, so it is clear it is one person shown in multiple places rather than several different people. The view stays a clean tree; nothing is merged.

**Lineage improvements**

- **Ancestors now show spouses, with step-parents marked.** Going up, each ancestor appears with their partner. Where an ancestor had more than one marriage, the partner who is not on your direct bloodline is tinted grey and labelled *step*, so the direct line stays clear.
- **Connector lines** now join the generations, making the shape of the tree easier to follow.
- **Clicking a sibling now adds them** beside the selected person (with their own descendants) instead of switching to them; click again to remove, and add as many as you like. A half-sibling is shown with a small two-parent cap — the shared parent plus their different parent — so the split in the line is clear. Clicking a person's box still just opens their details.

---

## Version 3.6 — July 2026

**New**

- **Lineage tab** — a new view (before Branch View) that shows a person's complete line at once: ancestors fanning **upward** and descendants fanning **downward**, meeting at the selected person in the middle.
  - The upward part is a true bloodline pyramid — each ancestor's father and mother sit side by side, and a parent's other marriages or step-relations are not mixed in.
  - **Siblings** appear as links; clicking one re-centres the view. Full siblings keep the same ancestors, while a half-sibling's line traces back through their own different parent.
  - **Directional collapse:** hide everyone above a chosen ancestor, or everyone below a chosen descendant.
  - Includes the legend and a **Print Lineage** option (A3 PDF) with the same credits footer as the other tabs.
- The Lineage tab is always visible, like Branch View.

---

## Version 3.5 — July 2026

**Fixes**

- **Branch View default** now accepts either the person's id (e.g. `p417`) or their exact name, and the Admin picker shows the current selection. If the configured person isn't found, the Admin tab now says so instead of silently ignoring it.
- **Import Config** now restores every setting — tabs, credits, presenter line, branch default, contact-form email and donation links — instead of only the email settings.
- **Download config.json** no longer forces the Branch View, Contact and Help tabs back on, and it keeps the explanatory notes inside the file.

**New**

- **Tab visibility** now includes Contact Us and Help, so these can be shown or hidden alongside the existing options. Branch View is always visible, as it is the main way visitors explore the tree.

---

## Version 3.4 — July 2026

**New features**

- **Minimisable legend** — the colour, flag and DNA legend now sits at the bottom-right as a small button you can expand or tuck away, so it no longer covers the tree. Works on both the Family Tree and Branch View tabs.
- **Branch View default person** — administrators can set a person that Branch View opens to by default (chosen via a generation filter and person selector), or leave it empty to open with the search box.
- **Multi-line "Presented By"** — the presenter line now supports line breaks, shown on both the welcome screen and printed PDFs.

**Changes**

- On mobile, the details panel now starts closed so the whole tree is visible; tap a person to open their details. On desktop the panel still opens by default.

---

## Version 3.3 — June 2026

**New features**

- **Recalculate Generations** (Admin) — recomputes every person's generation from the family links. Parents set the generation; people with no parents inherit it from their spouse. Use it after adding a new ancestor at the top of the tree. It updates the on-screen view for review only — Export CSV and re-publish to make it permanent.
- **Configurable "Presented By"** — the presenter line on the welcome screen (and printed PDFs) is now set in the Admin panel and stored in `config.json`, alongside the existing contributor credits.

**Notes**

- Adding a parent does **not** automatically renumber descendants. Run *Recalculate Generations* afterward, then export and publish.
- Genuine cross-generation marriages are surfaced in the Validation tab rather than being silently changed.

---

## Version 3.2 — June 2026

**New features**

- **Add Partner** — administrators can now add a spouse directly from a person's panel. The new partner is automatically linked as their spouse, placed in the same generation, and given the same country.
- **Generation numbers on nodes** — every person's generation (e.g. *Gen 7*) now appears on their box in both the Family Tree and Branch View.
- **Version Updates tab** — this page. It reads a `version.md` file and can be shown or hidden from the Admin panel.

**Changes**

- The **Export Branch (CSV)** button in Branch View is now visible only to a logged-in administrator.
- The welcome screen now reads *Presented by Yathavan Pathmanathan (Canada) & Raj Aravinthan (Australia)*.

---

## Version 3.1 — June 2026

**New features**

- **Add Child** now pre-fills the parent, their spouse, and the country automatically.
- **Type-to-search** for Father, Mother and Spouse fields when editing — no more scrolling long lists.
- **Generation override** — the generation can be set manually when editing a person.
- **Branch legend** — the colour, flag and DNA legend now appears on the Branch View too.

**Changes**

- Clicking a person in Branch View now opens their details in place, without jumping to the Family Tree tab.
- The main search box moved into the Family Tree tab.
- Larger fonts for the legend and credits on printed PDFs.

---

## Version 3.0 — June 2026

- Split into separate `index.html`, `data.csv` and `config.json` files for easier hosting and data updates.
- Branch View collapse and expand for children and siblings.
- Configurable tab visibility and welcome-screen credits via the Admin panel.
