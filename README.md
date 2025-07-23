# 🐉 Train Your Git (and Your Dragon)

Welcome to Berk — and to Git!

This project will teach Git basics through a collaborative, story-driven project where each student contributes a chapter from the perspective of a character in *How to Train Your Dragon*.

This is a Markdown file. To see a render of this file in your IDE, right click on the tab with the file name and click *Open Preview* (Ctrl+Shift+V).

## Goals
- Learn how to use Git: branching, committing, pushing, resolving conflicts
- Collaborate on a shared creative project
- Have fun telling stories with dragons

## Student Characters
Each student will write chapters from their character’s perspective and follow Git workflows.

| Student   | Character     | Role in Story                                     |
| --------- | ------------- | ------------------------------------------------- |
| Student 1 | **Hiccup**    | Protagonist, awkward dragon-slayer-turned-trainer |
| Student 2 | **Astrid**    | Fierce warrior, suspicious of Hiccup              |
| Student 3 | **Toothless** | The Night Fury dragon, silent but expressive      |
| Student 4 | **Stoick**    | Hiccup’s father, chief of Berk                    |
| Student 5 | **Gobber**    | Blacksmith and dragon training instructor         |

## Instructions

1. Clone this repository:

```bash
git clone https://github.com/phpet/train-your-git.git
cd train-your-git
```

2. Each student creates a feature branch based on their character:
```bash
git branch hiccup-story    # create the branch
git checkout hiccup-story  # switch to it
```

Each student will will use their own branches:
- astrid-story
- toothless-story
- gobber-story
- stoick-story

3. Edit the corresponding file under `chapters/`. 

    Include:

    - A short narrative (5–10 sentences) from your character’s perspective
    - Markdown formatting (headers, bold/italic for thoughts, etc.)
    - You can use AI to create the story if you don't know the story or haven't watched the movie yet.

4. Commit your changes:
```bash
git commit -m "Toothless saves Hiccup in the cove"
```
5. Push and open a Pull Request.
```bash
git push origin toothless-story
```
On github website, open a Pull Request and assign it to Philip.

## Key Git Concepts and Activities

| Concept               | Activity                                                   |
| --------------------- | ---------------------------------------------------------- |
| `git status`          | Check what’s changed                                       |
| `git add`             | Stage your new chapter file                                |
| `git commit`          | Save your change with a message                            |
| `git push`            | Upload your branch to GitHub                               |
| `git pull`            | Get other student's changes locally                        |
| Pull Request (PR)     | Submit your story for review                               |
| Code Review           | Students review each other’s PRs                           |
| Merge Conflicts       | Triggered during simultaneous edits                        |
| `git log`, `git diff` | Explore project history and differences                    |

After trying the git commands above, use also the Source Control UI from Kiro (the third icon on the left).

## Conflicts
Conflicts are dragons — learn to tame them.

Conflict Exercise

After initial PRs are merged:

1. Astrid and Hiccup will both edit the same line in chapters/01-hiccup.md.
2. They each will commit and push to separate branches.
3. Merge one PR (the second will have a merge conflict).
4. Resolve the conflict:

```bash
git pull origin main
# edit file manually to fix conflict
git add chapters/01-hiccup.md
git commit -m "Resolved conflict between Astrid and Hiccup"
git push
```
