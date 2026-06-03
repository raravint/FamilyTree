# Version Updates

A running log of changes to the Family Tree application.

---

## Version 3.3 — June 2026

**New features**

- **Recalculate Generations** (Admin) — recomputes every person's generation from the family links. Parents set the generation; people with no parents inherit it from their spouse. Use it after adding a new ancestor at the top of the tree. It updates the on-screen view for review only — Export CSV and re-publish to make it permanent.

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
