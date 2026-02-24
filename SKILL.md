---
name: thought-sprout
description: Analyzes a collection of user notes to generate a "sprout report." Use when the user wants to find deeper connections and insights from their recent notes, or explicitly asks to "sprout" their thoughts. This skill transforms raw notes into a cohesive, insightful narrative using story-driven expansions.
---

# Thought Sprout

## Overview

This skill transforms a collection of raw, fragmented user notes into a polished, narrative "Sprout Report." It analyzes 3-5 notes from a recent period (e.g., the last 3 days), identifies underlying themes, and expands each note into a compelling story. The final output is a literary and philosophical exploration of the user's own thoughts, designed to spark new insights.

## Workflow

The process follows a 6-step workflow to generate the final report.

### Step 1: Note Aggregation and Time Window

First, gather the user's recent notes to form a "thought snapshot."

- **Time Window**: Default to the last 3 days of notes. This can be configured to 1, 3, or 7 days.
- **Note Selection**: Filter out very short notes (<20 words) or pure quotations. Prioritize notes that show depth of thought.
- **Quantity**: Aim for 3-5 notes. If more are available, select the most representative ones.
- **Order**: Arrange the notes chronologically.

### Step 2: Thematic Analysis & Poetic Opening

Next, analyze the collected notes to identify a central theme or trajectory. Based on this analysis, generate a literary, poetic opening that summarizes the user's recent train of thought.

- **Identify Patterns**: Look for the thinking style (e.g., focused on one topic vs. jumping between ideas), the emotional tone (e.g., curious, anxious), and cognitive characteristics (e.g., detail-oriented, philosophical).
- **Generate Opening**: Use the insights from the pattern analysis to craft a unique, metaphorical opening. 

> For detailed instructions and the prompt template, refer to:
> `/home/ubuntu/skills/thought-sprout/references/opening_prompt.md`

### Step 3: Story-Driven Expansion for Each Note

This is the core of the skill. Each individual note is expanded into a complete narrative with three parts: a Seed, a Story, and an Aha Moment.

1.  **🌱 Seed**: Reframe the user's original note, connecting it to a much larger, more profound concept. This creates a "cognitive surprise" and sets the stage for the story.
2.  **📖 Story**: Find a compelling historical event, scientific discovery, or cultural phenomenon that illustrates the concept introduced in the Seed. The story must be factual, dramatic, and relevant.
3.  **✨ Aha Moment**: Distill the core insight from the story into a single, memorable, and often paradoxical sentence.

> For the detailed structure, prompt templates, and generation strategies for this step, consult:
> `/home/ubuntu/skills/thought-sprout/references/expansion_prompt.md`

To find compelling stories, a specific research strategy is required. This involves using targeted search queries and filtering results for dramatic, authoritative, and relevant content.

> For the story research and selection process, see:
> `/home/ubuntu/skills/thought-sprout/references/story_search.md`

### Step 4: Golden Quote Resonance (Optional)

If a user's note contains a particularly insightful or "golden" quote, this optional module can be triggered. It expands on the user's idea by finding related quotes from different perspectives (e.g., science, history, culture).

> The multi-perspective search strategy is detailed in:
> `/home/ubuntu/skills/thought-sprout/references/story_search.md`

### Step 5: Report Assembly

Assemble all the generated components into a single, coherent Markdown document. This includes:

- The poetic opening.
- The expanded story for each note, presented in order.
- The optional "Golden Quote Resonance" section.
- A literary, engaging title for each note's section.

> For the title generation prompt, refer to:
> `/home/ubuntu/skills/thought-sprout/references/system_prompt.md`

### Step 6: Quality Control

Before delivering the final report, perform a rigorous quality check. The goal is to ensure the report is coherent, factually accurate, insightful, and written in a consistent, literary style.

> Use the comprehensive checklist to validate the report:
> `/home/ubuntu/skills/thought-sprout/references/quality_checklist.md`

## Core Principles

When executing this skill, adhere to the core system principles defined for the "Thought Sprout" persona.

- **Style**: Literary, narrative, and insightful over academic and theoretical.
- **Content**: Prioritize stories over facts, and aim for "Aha!" moments.
- **Tone**: Warm, encouraging, and philosophical.
- **Accuracy**: All stories, names, dates, and facts must be verifiable.

> The full system prompt is available for reference:
> `/home/ubuntu/skills/thought-sprout/references/system_prompt.md`
