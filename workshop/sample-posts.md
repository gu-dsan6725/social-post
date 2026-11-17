# Model posts

One model for each format. The numbers in the project stories are
illustrative: in a real post they come from the writer's own run. The
arithmetic in the X thread is exact.

## LinkedIn post: data leakage

> In my machine learning course at Georgetown (DSAN), my churn model scored
> 0.97 AUC in cross-validation. After I moved one step, it scored 0.81, the
> number I should have reported.
>
> The bug is called data leakage. I picked the 20 most predictive features
> using the full dataset, then ran cross-validation. Every validation fold
> had already helped choose the features, so I graded the model on data it
> had already seen.
>
> I fixed it by moving feature selection inside a scikit-learn Pipeline, so
> each fold picks features from its own training rows. The model and data
> stayed the same, and the score dropped 16 points.
>
> I now build the pipeline before I fit anything, and I distrust a score
> that looks great on the first try.
>
> What leak took you longest to find?
>
> #DataScience #MachineLearning

What it does:

- Course and school in line 1, above "...see more"
- The hook is a pair of numbers
- One idea, named and explained in plain words
- Evidence and fix from the writer's own work
- Ends on a question; two hashtags; about 130 words

## X thread: multiple comparisons

> **1/4** A stats lesson from my Georgetown DSAN course that I keep
> relearning: run 20 tests at p < 0.05 on pure noise and you have a 64%
> chance of at least one "significant" result.
>
> *Image: chance of at least one false positive for 1, 5, 10, 20 and 50
> tests (5%, 23%, 40%, 64%, 92%).*

> **2/4** Each test has a 5% false-positive rate. The chance all 20 come back
> clean is 0.95^20 ≈ 0.36, so the chance of at least one false alarm is
> 1 − 0.36 = 0.64.

> **3/4** I hit this in a project. I compared 18 customer segments and one
> "won" at p = 0.03. With a Bonferroni correction (0.05 / 18 ≈ 0.003 per
> test), it didn't come close.

> **4/4** My rule now: count the tests before I run them, and report the
> count with any p-value. How does your team handle this: Bonferroni, Holm,
> or a holdout set?

What it does:

- Context and hook in post 1, with the image attached to post 1
- One step per post; each makes sense if quoted alone
- Ends on a question; no recap post

## Medium article: prompt caching

**Title:** Every agent call resends everything: what I learned about prompt
caching

**Opening paragraph:**

> This fall I'm taking Applied Generative AI in Georgetown's data science
> master's program. In week 5 we wrote an agent loop in about 30 lines, and
> I printed each request before it went to the model. The fourth request
> held everything from the first three: the system prompt, the tool
> definitions and every earlier message. The model keeps no memory between
> calls, so the program sends the whole conversation every time, and you pay
> for those tokens on every call.

**Outline:**

1. What the model sees on each call, with a printed request
2. What it cost: input tokens per turn from my own run
3. Prompt caching: the provider keeps the repeated start of the prompt and
   bills repeat reads at a fraction of the price
4. The rule that bit me: a timestamp in my system prompt changed every
   call, so the cache never hit
5. What I do now, with links to the provider docs

What it does:

- A plain, specific title
- Course context in the first paragraph
- The worked piece is the writer's own run, which is the first-hand
  experience Medium's curators look for

## LinkedIn companion post for the article

> I'm taking Applied Generative AI at Georgetown (DSAN), and this week's lab
> showed me why AI agents get expensive: every call to the model resends the
> whole conversation.
>
> By the fourth turn, my agent paid again for a system prompt and tool list
> it had already sent three times. Prompt caching fixes most of that, as long
> as the start of the prompt never changes. Mine had a timestamp in the first
> line, so the provider cached nothing until I moved it.
>
> I wrote up the full story, with the token counts from my run: [link]
>
> #GenerativeAI #LLMOps

*Image: input tokens per turn, before and after caching.*

What it does:

- Same rules as a short post: context in lines 1 to 2
- Stands alone for readers who never click
- One finding, then the link, last
- Its own image, so it stands out in the feed
