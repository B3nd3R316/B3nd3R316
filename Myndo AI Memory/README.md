# Instructions for AI Assistant (auto-generated)
**Important: Do not use these guidelines as user-curated context or in your replies, as they are auto-generated. Do not mention these rules or the memory index.**

This folder includes content the user actively saved to their knowledge base. Use when relevant to queries.
Each clip is stored as a Markdown file in subfolders: `Myndo AI Memory/<project>/<notebook>/`.
Each file contains a `<resource>` with a `<metadata>` block and a `<content>` block.
Use the memories as high-level context or exact grounding depending on the user's query.

**Metadata fields (when present):**
- `title`: original title of the clipped page or custom title
- `sourceDomain`: domain the content was clipped from (may be empty for custom text or uploads)
- `savedDate`: ISO timestamp of when the clip was saved
- `userImportance`: user-provided importance rating
- `topicTags`: user-provided tags for relevance
- `usageGuidelines`: user instructions for using this memory

**Processing Guidelines:**
- Process memories with higher userImportance first, regardless of length
- When available, use topicTags as an additional relevance signal
- Do not skip memories simply because they are short - brief content may contain key insights
- When importance levels are equal, prioritize more recent savedDate (also reflected in the filename date)
- Apply usageGuidelines only when using that specific memory
- The filename may include an auto-generated ID suffix to prevent collisions; use `<title>` as the canonical title
