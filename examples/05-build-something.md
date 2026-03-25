# Example 5: Build Something

> Time: ~20 minutes
> Goal: Build a working tool from scratch — without writing a single line of code yourself

## The Big Idea

This is where Claude Code goes from "useful assistant" to "wait, it can do THAT?"

You're going to build a real, working web application. Right now. No programming knowledge required.

## Project: Research Group Website

Let's build a simple website for your research group.

```
Build a modern, clean website for our research group with these pages:

1. **Home** — Group name: "Berven Lab - Proteomics & Biomarker Discovery"
   Department of Biomedicine, University of Bergen
   Brief intro about our research focus

2. **Research** — Our main areas:
   - CSF Proteomics & Neurodegenerative Disease Biomarkers
   - Single-Cell Proteomics
   - Mass Spectrometry Method Development
   - Clinical Proteomics Translation

3. **Team** — A page with placeholder cards for team members
   (name, photo placeholder, title, research interest)

4. **Publications** — A page that could list recent publications

5. **Contact** — Department address, email, map placeholder

Use a single HTML file with embedded CSS. Make it look professional —
UiB colors (dark blue and white). Responsive for mobile.
Save it as research-group-website/index.html
```

### Preview It

```
Open the website in my browser so I can see it
```

### Iterate

This is the magic. Just tell Claude what to change:

```
I like it, but:
- Make the header image area taller
- Add a Norwegian flag icon next to the language option
- The team cards should be 3 per row on desktop
- Add our actual UiB logo (just use a placeholder URL for now)
```

## Alternative Project: Data Dashboard

If a website isn't your thing, try this:

```
Build me an interactive data dashboard for proteomics experiments.
Single HTML file, no server needed.

Features:
- Upload a CSV file (protein IDs, expression values across samples)
- Show a sortable, searchable table of all proteins
- Generate a volcano plot (user selects two groups to compare)
- Generate a heatmap of the top 50 most variable proteins
- Export filtered results as CSV

Use modern JavaScript with Plotly.js for charts.
Save it as proteomics-dashboard/index.html
```

## Alternative Project: Task Tracker

```
Build a simple task tracker for managing my department duties.
Single HTML file with localStorage (no server needed).

Features:
- Add tasks with: title, category (Research/Teaching/Admin/PROBE), priority, deadline
- Filter by category
- Mark tasks as done
- Show overdue tasks in red
- Clean, minimal design

Save it as task-tracker/index.html
```

## What Just Happened

You just built a working web application by describing what you wanted in plain English.

No HTML. No CSS. No JavaScript. You described it like you'd describe it to a colleague, and Claude built it.

This is what Claude Code does. It turns ideas into working software.

## Going Further

Want to get ambitious? Here are real things Claude Code can build for you:

- **Lab inventory system** — track reagents, antibodies, consumables
- **Student progress tracker** — PhD milestones, publications, hours
- **Experimental protocol library** — searchable, versioned, shareable
- **Budget calculator** — for grant applications, with NOK formatting
- **Conference trip planner** — abstract deadlines, flights, budgets

Just describe what you need. Claude builds it.

> *This is not a conspiracy, Frode. AI can actually do this. No lizard people involved.*

**Next:** [06-advanced-tricks.md](06-advanced-tricks.md) — the deep stuff.
