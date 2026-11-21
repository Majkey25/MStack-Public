---
name: bro-what
description: Re-explain an idea that failed to land. Use when the user asks for plain language, points to a confusing phrase, or repeats a question because the previous explanation skipped context.
license: MIT
---

# Bro, what?

Find the exact term, step, or relationship causing trouble. If the user points at a phrase, explain that phrase first. Otherwise pick the one missing fact that makes the rest understandable.

1. Give the missing context in one or two sentences.
2. Explain what happens in concrete terms. Define necessary jargon where it appears.
3. Change the angle if the first explanation failed. Use a tiny example or walkthrough and connect it to the actual mechanism.
4. Keep the original conditions, uncertainty, and exceptions that affect the answer. If the original claim was wrong, correct it before simplifying.

Match the user's language and level of detail. Give the direct answer before a longer explanation. Avoid baby talk and analogies that change how the thing works.

If the user asks what exponential backoff means for a worker, explain that the worker waits longer after successive failures so it stops hammering a troubled service. If the exact delays matter, look up the worker's retry settings.
