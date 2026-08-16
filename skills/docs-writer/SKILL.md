---
name: docs-writer
description: Write docs that are clean, organize, and easy to understand. Use only when the user explicitly asks to write or update docs.
---

# Docs Writer

Write docs that are clean, organized, and extremely easy to understand for someone new to the project, whether engineer, designer, PM, or agent. Each of the writing rules has a before and after example.

## General guidelines

- Always favor the simplest, most direct, and easiest to understand plain English language. A new person to the project should be able to skim and understand very quickly.

- Use info-dense and precise writing. Every sentence should add new info or provide context to help with understanding. Avoid bloat like vague filler, corporate jargon, and empty statements that sound relevant but say little.

- Include reasoning, rationale, or other context to help with understanding. Explain why important points matter in plain English. The implication, or the "why" behind essential points.

- Avoid overly hard prescriptive language or narrow hard rules, unless truly needed. It's preferable to convey the approach, intent, rationale, etc., otherwise agents will blindly overfit to specific words/rules and end up at some loophole that completely misses the intent.

- Use simple and organized doc structure. Group and sequence ideas together logically so it is easy to follow and the overall doc is coherent. Avoid complex or messy formatting and random one-off points scattered around the doc.

- Avoid narrative framing and making implicit references to discussions or things the reader has zero knowledge of. E.g. saying "previously", "no longer", "used to" vs. just saying directly what it is. Don't mistake what YOU the writer know vs. what the reader knows.

- Lead with critical info for understanding. Don't mix irrelevant noise and low importance details into high-level framing, keep this separate.

## Writing style

- Use simple, everyday words. Don't pick a fancy synonym when a plain word works. Also avoid words AI tools overuse, e.g., "delve", "tapestry", "landscape", "robust", "leverage", and "reach". Before: We leverage the cache to unlock a more robust query experience. After: We use the cache to make repeated queries faster.

- No jargon. Always use human-understandable language, the way two people talk to each other. Don't invent jargon or shorthand. Use established technical terms when they are most precise. Before: The score is a calibrated proxy for whether the property holds. After: The score estimates how likely the property is to hold.

- No puffery or empty emphasis. Drop words that add emphasis but no information, e.g., "really", "real", "matters", "worth", "carries weight", "boasts", "a testament to", "pivotal", "renowned", and "quietly". State the actual point, or cut the sentence. Before: This result matters, and it carries weight for the design. After: The scores barely moved, so we can skip the model on most documents.

- Use consistent terminology and constrain your vocabulary. Before: Upload the document. The file is parsed, and the record is saved. After: Upload the document. The document is parsed and saved.

- Keep the writing boring, descriptive, and explanatory. Do not use a catchy phrase, slogan, clever label, or wording meant to sound memorable. This rule applies everywhere, including headings, topic sentences, summaries, etc. Before: Legal requirements as a floor. After: Applicable legal constraints.

- Do not give inanimate things fake agency. Do not write as if a system or object transforms, decides, or intends on its own when a person or process is the real actor. Ordinary factual verbs for tools and systems are fine, e.g., "The API returns JSON", "The job writes the file", or "The paper argues". Prefer a human or process subject when that is clearer. Before: The logs become searchable records, once the job finishes. After: You can search the logs, once the job finishes.
