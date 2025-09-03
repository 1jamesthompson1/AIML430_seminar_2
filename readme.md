# Seminar 1

This repository contains the reports and presentation for Seminar 2 from Remote

**Seminar details**:
Title: ...
Time: Currently unknown
Location: HM LT001 
Team members:
- Dwayne Mark (Dwayne) Acosta
- Mohamed Amine (Mohamed) Benaziza
- David Franz
- Ray Marange
- James Thompson

## Instructions

Insturctions copied from the website: https://ecs.wgtn.ac.nz/Courses/AIML430_2025T2/Seminar2

How?

Similar structure to the first seminar with a few changes:

    Rather than a specific paper, you will be expected to find five papers in a pre-determined area.
    You pick the area/topic and get Bach's approval. It can't overlap with any of your team members' reports, and it can't be identical to another group's (first-in, first-served). The deadline for approval is 4pm Friday 5th September.
    Your summary notes and critical analysis will be longer than in the first seminar (max 1 page/500 words per team member).
    Your notes/analysis and seminar will also focus on the implications of applying AI techniques to your application area.
    Notes (8%, group); Presentation (4%, group, 15-25 (MAX) minutes); facilitation of discussion (2%, individual); asking a question in another seminar (1%, individual).
    Split the writing and presenting workload as you see fit - but everyone should do their part! 

When?

    Notes and slides due Sunday start of Week 9 (Sunday 14th September 11:59 pm).
    Seminars in weeks 9, 10, start of 11. 


## Contributers

The documents are in LaTeX. The summary report is called [summary.tex](summary.tex) and the presentation is called [presentation.tex](presentation.tex).

The output pdfs of these can be found in the [output](output/) directory.

The bibliography is in Bibtex format, [references.bib](references.bib).


### Building documents

I use LaTeX workshop in vscode to do my work. However if you want to just build manually you can do so as well.
Assuming you have a Tex distribution installed you can just run.

```bash
latexmk -pdf summary.tex -output-directory=output
latexmk -pdf presentation.tex -output-directory=output
latexmk -c --output-directory=output
```

It will build both documents with the dependencies.

### Adding referecnes

To add referecnes add the bibtex entry directly into the references.bib file. Then you can use the usual `\cite{...}` command.

### Pushing to main

You must make a pull request to merge changes into the main branch. The pull request will check to make sure that the latex builds.