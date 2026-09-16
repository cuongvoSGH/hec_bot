---
name: document-search-and-summary
description: "Search long documents, find specific information, answer material-based questions, and summarize documents. Use when the user asks to search lecture notes, locate a topic or keyword, extract evidence, compare passages, or produce a concise summary from workspace files."
argument-hint: "Enter a topic, question, keyword, or document to search and summarize"
user-invocable: true
---

# Document Search and Summary

## Purpose

Search documents in the workspace and produce concise, evidence-grounded answers or summaries. Use only the provided documents unless the user explicitly asks for outside information.

## When to Use

- Find a keyword, economist, theory, concept, or phrase in long documents.
- Identify which document, lecture, section, or passage contains specific information.
- Answer a question using one or more provided documents.
- Summarize a long document, lecture, chapter, or a selected section.
- Compare how a topic appears across multiple documents.

## Procedure

1. **Clarify the target**
   - Identify the document scope, topic, question, and desired output length.
   - If no document is named, search the relevant workspace files.
   - Preserve the user's wording and search related forms of the term when useful, such as singular/plural or common spelling variants.

2. **Search before answering**
   - Search filenames, headings, and document text for the target terms.
   - For long documents, locate relevant sections first instead of reading every unrelated passage.
   - Read enough surrounding context to understand the passage and avoid quoting an isolated sentence.

3. **Extract evidence**
   - Record the smallest passages that directly support each factual claim.
   - Note the exact source filename and the most precise available location: heading, page, paragraph, or line.
   - Separate direct statements from clearly labeled interpretation.

4. **Answer targeted questions**
   - Give the direct answer first.
   - Support each important claim with a source reference.
   - When comparing documents, identify similarities and differences using evidence from each source.
   - If the material does not answer the question, say: "The material does not provide enough information to answer this." Then state what information is missing.
   - Do not fill gaps with general knowledge or invented details.

5. **Summarize long documents**
   - State the document title and its main purpose or subject.
   - Identify the central argument, major themes, important people or concepts, and significant conclusions.
   - Organize the summary using short headings or bullet points when that improves readability.
   - Keep the summary proportional to the user's requested length.
   - Distinguish material-supported conclusions from interpretation.

6. **Check the result**
   - Verify that every factual claim is supported by the searched material.
   - Confirm that citations point to the passage being described.
   - Remove unsupported assumptions, repeated details, and irrelevant background.
   - Mention ambiguity or contradictions instead of silently choosing one interpretation.

## Response Format

### For a Search

**Found**
- State what was found and where.
- Include a short exact quote when it clarifies the result.

**References**
- Source: `path or document title`
- Location: `heading, page, paragraph, or line`

### For a Specific Question

**Answer**
Give the concise answer supported by the material.

**Reference**
- Source: `path or document title`
- Location: `heading, page, paragraph, or line`
- Evidence: "short exact quote"

**Evidence note**
State whether the answer is directly stated, supported by multiple passages, ambiguous, or not found.

### For a Summary

**Summary**
Provide the requested summary, organized around the document's main ideas.

**Key points**
List the most important supporting ideas or terms.

**Reference**
Identify the source and the relevant headings or sections used.

## Quality Rules

- Never invent an answer, citation, quote, page number, or search result.
- Never claim to have searched a document that was not available.
- Prefer exact evidence over broad paraphrase.
- Use plain language, while preserving important technical terms.
- Keep the answer focused on the user's question.
