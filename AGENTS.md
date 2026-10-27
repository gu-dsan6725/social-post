# AGENTS.md

Guidance for AI coding agents working in this repository.

## What this repo is

A short lab for DSAN 6725 (Applied Generative AI, Georgetown, Fall 2026): each student picks
one topic from the course and publishes a real post about it, under their own name, on
LinkedIn (preferred) or X, or as a LinkedIn/Medium article shared with a companion post. The
post must carry an infographic and must say near the top that it comes from this course. There
is no code in this repo; the deliverables are the final post text, the image, and the live URL.

- The GitHub repo `gu-dsan6725/social-post` is **private**; student copies are made by
  [assignment-setup](https://github.com/dsan-gu/assignment-setup), which withholds `solution/`.
- Students finish with the commit message `final-submission`. The lab is worth 100 points; the
  rubric is `solution/GRADING.md`.
- The course repo is `../6725-fall-2026`.

## Layout

| Path | Purpose |
|------|---------|
| `README.md` | The whole assignment: task, the disclosure requirement, infographic guidance, the AI-usage rules, timing (9am Tue/Wed/Thu), deliverables |
| `templates/linkedin-post.md` | 100-200 word post template with checklist |
| `templates/x-post.md` | Single post or short thread template |
| `templates/article.md` | Long-form article plus companion-post template |
| `outputs/` | Student deliverables: `post.md`, `infographic.png`, `post_url.txt` |
| `solution/GRADING.md` | Rubric; withheld from student copies |

## Rules for edits

- The hard content requirement is non-negotiable and must stay prominent in README and every
  template: the course context (DSAN 6725, Georgetown) appears at the top of the post, before
  the content. Tagging the instructor is **not required** and must stay that way in all
  student-facing text; class engagement (likes, reposts) stays
  **desirable and not required**.
- The AI-usage section is policy: AI allowed, write-first-then-edit recommended, and the ban
  list of machine-writing tells stays explicit. Do not soften it.
- All prose follows the course writing skill
  (`../6725-fall-2026/.claude/skills/writing/SKILL.md`), and this repo additionally avoids
  double hyphens and em dashes everywhere; use commas, colons, and parentheses.
- No solution exemplar post is committed: a sample post would become forty near-copies on
  LinkedIn. The rubric is the only grading artifact.

## Git

- `main` only. Commit when the user asks. Never commit student outputs here.
- No AI co-author trailers; agents assist, humans author.
