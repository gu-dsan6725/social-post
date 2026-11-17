# Best practices for technical posts

What experienced technical writers do, and what the platforms reward as of
November 2026. Platform behavior changes often; recheck the sources before
each workshop.

## Pick the topic

- **Write about what you just learned or struggled with.** Julia Evans
  builds many of her posts this way: if something confused her, it likely
  confuses others, and what she learned getting unstuck helps them
  ([jvns.ca, 2021](https://jvns.ca/blog/2021/05/24/blog-about-what-you-ve-struggled-with/)).
- **Keep it small.** Simon Willison publishes "Today I Learned" notes on one
  small thing; most take him under ten minutes
  ([simonwillison.net](https://simonwillison.net/2022/Nov/6/what-to-blog-about/)).
  His top tip is to lower your standards and publish while you are still
  unhappy with the draft
  ([interview](https://writethatblog.substack.com/p/simon-willison-on-technical-blogging)).
- **Learn in public.** swyx argues that most people learn in private and
  lurk, and that sharing as you learn costs only your ego
  ([swyx.io](https://www.swyx.io/learn-in-public)).
- **One idea per post.** If you need "and" to state it in one sentence, you
  have two posts.
- **Use your own artifact.** A number you computed, a log or trace you
  read, a failure you caused and fixed, a chart from your own run. It shows
  you did the work, and no AI draft can honestly supply it.

## Structure

Start from the story spine, rule 4 of Pixar's 22 rules of storytelling,
which improv teacher Kenn Adams invented: "Once upon a time there was ___.
Every day, ___. One day ___. Because of that, ___. Because of that, ___.
Until finally ___." It fits a film and a bug report equally well
([Open Culture](https://www.openculture.com/2013/03/pixars_22_rules_of_good_storytelling.html),
[NPR](https://www.wunc.org/2026-06-23/meet-the-creator-of-the-story-spine-an-8-sentence-tool-to-create-and-analyze-stories)).
A post cuts the same beats down to five parts:

| Part | What goes there | Length |
|------|-----------------|--------|
| Hook and context | What happened, and where you learned it | Lines 1 to 2 |
| The idea | One concept, every term spelled out | 2 to 4 sentences |
| Your evidence | A number, trace, chart or failure from your own work | 2 to 3 sentences |
| What it changes | What you now do differently | 1 to 2 sentences |
| The close | A real question for readers who know more | 1 line |

- LinkedIn shows about three lines before "...see more". The context and
  the hook both have to sit above the cut.
- Open with the specific thing: a number, a named failure. Skip greetings,
  questions and announcements.
- Use short paragraphs and white space. Most readers are on a phone.

## Formats

| Format | Length | Use it when |
|--------|--------|-------------|
| LinkedIn post | 100 to 200 words, one image | One idea and one number |
| LinkedIn document (PDF carousel) | 5 to 10 slides | A sequence or a comparison |
| X post or thread | 280 characters, or 2 to 4 posts | Steps that each stand alone |
| Medium or LinkedIn article, plus a short post | 600 to 1,200 words | A worked example with code or screenshots |

Analysts report PDF carousels as LinkedIn's highest-engagement format in
2026, because swiping keeps readers on the post
([Sendible](https://www.sendible.com/insights/linkedin-algorithm)).
An article still needs a short companion post that teaches the one finding
on its own.

## What the platforms reward

**LinkedIn.** Reading time (dwell time) is the signal analysts rank highest;
comments and saves count more than likes. Reactions in the first 60 to 90
minutes decide whether a post reaches past your network. The feed pushes
down generic AI text, engagement pods and posts that send readers away
([Sendible](https://www.sendible.com/insights/linkedin-algorithm),
[SocialPilot](https://www.socialpilot.co/blog/linkedin-algorithm)).
LinkedIn removed hashtag following, so hashtags now label the topic; one to
three is plenty.

**X.** Replies carry far more weight than likes, most of all when the author
replies back; bookmarks and reposts also beat likes
([SocialPilot](https://www.socialpilot.co/blog/twitter-algorithm)). Reports
on link penalties conflict, so keep the substance in the post and put any
link last.

**Medium.** Human curators pick stories for Boost, Medium's widest
distribution, and they weigh the author's first-hand experience. The
simplest route is to submit to a publication in the Boost Nomination
Program: editors of 100+ independent Medium publications can each nominate
20 stories a month, and Medium's own curators decide which ones get Boosted
([BNP editors](https://blog.medium.com/bnp-editors-9c0a6f5a133a),
[How can I get Boosted?](https://blog.medium.com/how-can-i-get-boosted-33e743431419)). Medium won't Boost AI-generated writing and wants AI-assisted text
labeled; grammar and spell checks need no label
([distribution guidelines](https://help.medium.com/hc/en-us/articles/360006362473),
[AI content policy](https://help.medium.com/hc/en-us/articles/22576852947223)).

## Timing

| Study | Platform | Best window (reader's local time) |
|-------|----------|-----------------------------------|
| [Sprout Social 2026](https://sproutsocial.com/best-times-to-post/linkedin-general/): about 2 billion engagements, 307,000 profiles | LinkedIn | Midweek, midday; weekends weakest |
| [Buffer 2026](https://buffer.com/resources/best-time-to-post-on-linkedin/): 4.8 million posts | LinkedIn | Weekdays 3 to 8 p.m.; Wednesday 4 p.m. top |
| [Sprout Social 2026](https://sproutsocial.com/insights/best-times-to-post-on-twitter/) | X | Tuesday to Thursday, noon to 6 p.m. |

All three studies favor Tuesday to Thursday, and each names a different
best hour. Pick one midweek slot, such as 9 a.m. Tuesday, schedule your
posts for it, and check back during the first hour to answer comments.
After a few posts, check your own analytics.

## Consistency beats intensity

- **Make it a discipline.** Every two weeks, once a month, whatever works
  for you. Pick the pace once and keep it.
- **Draft early, schedule the post.** Write the draft on Sunday, then
  schedule it for 9 a.m. Tuesday. LinkedIn and X can both schedule a post,
  so it goes up on its own and is not one more thing to remember.
- **Expect a quiet start.** Unless you already have an audience, your
  first few posts will get little engagement. Everyone starts there, so
  keep to your schedule. People start to find you after months of regular posts.

## The image

- One idea per image. A big number or one small chart, readable on a phone.
- A fast route: ask an AI assistant to draw it as an SVG, fix it until every
  number is right, then convert it (`rsvg-convert -w 1200 chart.svg -o
  chart.png`; on a Mac, `brew install librsvg` first).
- If an image model draws it, read every word; image models misspell labels.
- Add alt text when you upload: one sentence on what the image shows.

## Using AI

Write the first draft yourself, let AI tighten it, then make the final pass
aloud. An editing prompt that keeps your voice:

```
Here is my draft post. Fix grammar and spelling.
Check each factual claim and flag any you doubt.
Keep my words, my order and my voice.
Add no phrases, emojis or hashtags.
List any other suggestions separately, with a reason for each.

[paste your draft]
```

## Giveaways to cut

- Words: game-changer, revolutionary, delve, unleash, supercharge, deep
  dive, landscape, journey, seamless, robust, leverage as a verb, "the
  future of X is here".
- Shapes: "It's not about X, it's about Y"; the em-dash reveal; "We didn't
  do X. We did Y."; labels such as "Key insight:"; three punchy fragments in
  a row; a closing line that repeats the post.
- Habits: a rocket or emoji wall in line 1, a wall of hashtags, hot takes
  you cannot back.

To fix any of these, replace the shape with the fact underneath it, usually
a number or a named action.

## After you post

- Stay for the first hour and reply to each comment with something specific.
- When someone corrects you, thank them, edit the post, and say what changed.
- Skip comment pods and like-for-like groups; platforms detect them.
- Keep an idea file. One post a month gives you twelve samples of your
  thinking in a year.
- Put a recurring Sunday block on your calendar for the next draft.

## Before you post

- [ ] Course or project named in the first three lines
- [ ] One idea, one image, and they match
- [ ] A number, chart or failure of your own
- [ ] Every claim checked; every term spelled out
- [ ] No giveaways from the lists above
- [ ] Every word on the image spelled right; alt text added
- [ ] Read aloud once
- [ ] Scheduled for your regular slot, Tuesday to Thursday, and you can check back in the first hour
