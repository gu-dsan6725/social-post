# social-post: Teach One Thing You Learned, in Public

You have spent weeks building RAG pipelines, agents, MCP servers, and eval
harnesses. This lab asks for something different: pick one topic from the
course and explain it to people outside the classroom, as a real post on a
real network, under your own name.

Writing in public is a skill with compound returns. A clear 150-word
explanation of pass^k or MCP does more for how you understand the topic,
and for how recruiters and colleagues see you, than another private
notebook. This lab is small on purpose; the thinking is the work.

## The task

1. **Pick one topic** the class has covered or that you explored because of
   it. Anything works: the N x M argument for MCP, why pass@1 and pass^k
   differ, what a trace shows that an answer hides, how a 2B model routes
   with one token, what broke in your RAG lab and why.
2. **Write a post** for LinkedIn (preferred) or X. Target 100 to 200 words
   for LinkedIn; X gets a single post or a short thread. If you would
   rather write long, publish a LinkedIn or Medium **article** and share it
   with a short companion post.
3. **Make an infographic** and attach it. The image is required, and an
   infographic is the right kind: one idea, a few numbers or a small
   diagram, readable on a phone.
4. **Post it**, ideally at **9am on a Tuesday, Wednesday, or Thursday**;
   those slots reach the most readers.
5. **Commit your materials** here (see Deliverables).

Templates for all three formats are in [`templates/`](templates/):
[LinkedIn post](templates/linkedin-post.md) ·
[X post or thread](templates/x-post.md) ·
[long-form article plus companion post](templates/article.md).

## The one hard requirement on content

Near the top of the post, visibly and in your own words, say that this
comes from coursework: you are taking **DSAN 6725 (Applied Generative AI)
at Georgetown**, and this is a topic you learned or explored in that class
and want to share. Readers should know the context in the first two or
three lines, before the content starts.

- **Tagging the instructor is not required.** You do not need to tag
  anyone at all.
- Everything else about the post is yours: tone, angle, hashtags or none.

## The infographic

- One idea per image. If the post is about pass^k, the image is the curve
  or the 0.9^8 arithmetic, with no second topic.
- A few large numbers or one small diagram beat a wall of icons. Make the
  text big; most readers see it on a phone.
- Any tool works: slides, Figma, Canva, Excalidraw, or a chart you render
  with code. A route that works well: ask Claude Code, Codex, or another AI
  assistant to **draw the infographic as an SVG**, iterate on it until the
  layout and numbers are right, then convert the SVG to a PNG and attach
  the PNG to your post. SVG text is real text, so nothing comes out garbled
- If an image model generates the picture instead, read every word on it;
  image models write garbled labels, and a garbled label in your
  infographic reads as carelessness
- Keep the source file. You will commit the image with your post text.

## Using AI to write: allowed, with rules

You may use AI anywhere in this workflow. The post still has to sound like
a person, because readers now recognize machine writing instantly and
discount it.

The best working order: **write the post yourself first**, badly is fine,
then let AI tighten it, then make the final pass yourself. Starting from
your own draft keeps your voice; starting from a blank AI draft produces
the post everyone else already published.

Banned, whether a human or an AI wrote it:

- Hype words and dead metaphors: game-changer, revolutionary, delve,
  unleash, supercharge, "the future of X is here"
- The standard AI shapes: "It's not about X, it's about Y", the em-dash
  reveal at the end of a sentence, three parallel punchy fragments in a
  row, a closing line that restates the post
- Hot takes you cannot back: "RAG is dead", "agents will replace
  engineers". You are sharing what you learned, with the modesty of
  someone three weeks into it
- Emoji walls and a rocket ship in the first line

A simple test before you post: read it aloud. If a sentence embarrasses
you in your own voice, it will embarrass you more under your name on
LinkedIn.

## Engagement from the class

When a classmate posts, liking or reposting it is **desirable and not
required**. No points attach to it either way; a class that amplifies its
own members' work simply reaches further, and someday you will want the
same from them.

## Deliverables

Commit to `outputs/`:

| File | What it is |
|------|------------|
| `outputs/post.md` | The final text you posted, plus the topic and format you chose (the templates have the exact structure) |
| `outputs/infographic.png` (or .jpg) | The image you attached |
| `outputs/post_url.txt` | One line: the public URL of the live post (and the article URL too, if you wrote one) |

**This lab is worth 100 points.** The rubric lives with the graders; the
short version: the disclosure is up front, the explanation is correct and
yours, the infographic carries one clear idea, and the post reads like a
person wrote it.

When you are ready to be graded, use the commit message `final-submission`.

## Licenses

Content in this repo is MIT licensed. Your post is yours.
