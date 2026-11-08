# Lesson images

## Trigger and count

**Generate and display exactly one instructional image for every concept or mini-concept explanation.** A rendered diagram or chart counts when the host displays the actual image. Plain tables, code, ASCII diagrams, prompts, filenames, bare links, and captions cannot replace it.

- **Concept explanations:** include the image even when the turn ends with an ungraded comfort question.
- **Quizzes, homework, and practice tasks:** never generate or render images during these activities, including item-specific hints, worked solutions, or feedback. Keep these turns text only to avoid revealing answers.
- **Other turns:** readiness, setup, navigation, or progress updates alone need no image.

The task prohibition takes precedence in a mixed teaching/task turn. Separate teaching from learner-response tasks. If a task exposes an untaught prerequisite, explicitly pause the task activity and preserve its bookmark before starting a separate prerequisite lesson with a different example. Its image must not reveal the pending task's answer. Item-specific assistance cannot be relabeled as a lesson to bypass the ban.

Request a single image output, with no batches, variants, or candidate galleries. A comparison or sequence may use multiple panels within that one image. Generate or render a new or updated image for the current explanation; unchanged reuse alone does not meet the requirement.

## Choose an informational image

**Prioritize informational diagrams, flowcharts, architectural blueprints, and side-by-side comparisons that break down processes or relationships. Generic or decorative stock photos, including generated stock-photo-style scenes, are strictly forbidden.** Every visual element must serve the explanation. A labeled technical cutaway, chart, or schematic is suitable when it better conveys the current idea.

Choose the representation yourself using the teaching goal, learner feedback, and available tools. Balance how clearly it conveys meaning against likely generation time. Use a quicker diagram when it explains the idea fully; spend more time only when the added detail improves understanding. Base time estimates on observed session behavior.

Vary diagrams purposefully in style, format, and arrangement. Consider technical drawings or sketches; flows, cycles, hierarchies, or comparisons; and panels, layers, radial groups, nested parts, or close-ups. These are options, not a fixed rotation. Avoid repeatedly relabeling the same boxes-and-arrows template or changing only its colors. Preserve useful notation and labels for continuity when they remain relevant to the current step.

## Reveal only the current step

Before creation, identify the exact learning step and the labels, components, and relationships needed to explain it. Include only that content, plus previously taught context essential to understanding it. Hide future complexity: omit later stages, advanced branches, extra components, and labels the learner does not yet need. Do not show future details as faded previews or fill empty space with background information.

Add detail progressively in later explanations as the learner reaches it. Each explanation still receives one image focused on its own step.

## Create, narrate, and check

1. **Plan the image and narration together.** Establish the facts, example, and exact label strings before generation. Use those same terms, spelling, symbols, and units in the image and in text referring to its parts. Avoid switching to synonyms for visual labels.
2. **Create one image.** Use a supported image generator, diagram renderer, or drawing tool suited to the representation. Follow the host's tool requirements. No particular provider, API, file format, or separate installation is required. Native automatic display counts as delivery and needs no duplicate embed.
3. **Check the actual output when accessible.** Verify labels against the planned wording, then check facts, values, arrows, relationships, legibility, counts, proportions, and current-step scope. A prompt or tool-success message alone is not a visual check.
4. **Narrate the image explicitly.** Direct the learner's attention and explain what the image shows and why it matters. For example, if the labels are `Input` and `Output`: “Notice how the arrow from `Input` to `Output` shows the direction of the change.” Use the exact visual label terms in the explanation. A caption or an unexplained image drop is insufficient. Put narration before or after display as the host supports; check actual labels before finalizing it when possible.
5. **Correct within the one-image limit.** Correct the same artifact in place if the host supports this without creating or displaying a second image. Otherwise, identify the error and give an accurate text correction; do not generate another image for that explanation. Never repeat an incorrect label in the teaching text merely to make it match an erroneous image.

Choose routes that preserve specified labels. If the host does not expose the displayed output for inspection, disclose that labels and appearance could not be verified. Narrate only the intended relationship using the planned terms, without claiming to have observed unseen labels, arrows, or other details. Do not claim exact label agreement was verified when it was not.

If generation fails without creating an image, try another available route with one output requested. Once an image exists, use that artifact for delivery rather than generating another. If creation, display, correction, or label verification cannot be completed, state the specific limit and use accurate text as needed; do not claim the image requirements were fully met. An explicit request for text only or fewer/no images is a scoped learner override. Less waiting or a preference for tables alone does not waive the image requirement.

A normal concept-explanation turn is complete when exactly one image has been created and displayed, it contains only current-step content, and the text narrates it using matching labels, with available accuracy checks complete. Report actual limits honestly. Count answer-revealing help under [Fair tasks and learning evidence](../SKILL.md#fair-tasks-and-learning-evidence). Preserve previously delivered task context under [Portable record and storage](progress.md#portable-record-and-storage); these rules do not authorize rewriting saved work.
