# Waestro

An adaptive, one-on-one LLM tutoring skill for planning courses, teaching small concepts, practicing, assessing understanding, and resuming from recorded progress.

Waestro is a **provider-neutral instruction package** for LLM conversations and agent sessions. It uses the host's available capabilities and includes text-only fallbacks. Loading and instruction-following behavior vary by host; this repository does not claim tested compatibility with every model or application. This is an experimental alpha; the instructions describe intended tutor behavior, not demonstrated learning outcomes.

## What Waestro does

- Plans courses with a Course → Week → Section → Module → Concept → Mini-concept hierarchy.
- Explains one manageable idea at a time, with worked examples and instructional images using the host's available image-generation capability.
- Separates exposure, assisted practice, independent demonstrations, and retained learning.
- Preserves pending tasks, assessment criteria, assistance history, and return points.
- Provides a partial manual resume card when richer progress storage is unavailable.

## Use the skill

Keep the complete skill folder together so its conditional references and project guidance remain accessible:

```text
waestro/
├── SKILL.md
├── references/
│   ├── course-planning.md
│   ├── images.md
│   ├── progress.md
│   ├── human-testing.md
│   └── provenance.md
├── resume-card-template.md
├── CONTRIBUTING.md
├── SECURITY.md
├── LICENSE.txt
└── NOTICE.txt
```

[SKILL.md](SKILL.md) is the instruction entry point. Choose the route supported by your host:

- **Native skills:** register the folder through the host's supported skill-loading mechanism.
- **File or attachment context:** provide `SKILL.md` and make the referenced files accessible, then explicitly ask the assistant to apply Waestro.
- **Text input:** supply `SKILL.md` through the host's supported instruction or prompt input, together with the reference text needed for the active task. File links alone do not supply their contents. Provide the resume-card template when a partial progress export is needed.

The YAML frontmatter identifies the skill for hosts that support it; the Markdown body contains the tutoring instructions. This repository supplies no provider-specific integration or installer. When redistributing the package, retain its license and notices.

`SKILL.md` keeps the teaching loop, evidence rules, and navigation safeguards in the entry point. Its routing table identifies when the tutor must read planning, image, progress, or human-testing procedures. References already available in the current context can be reused.

Once the skill is loaded, a learner can make a request such as:

> Use Waestro to help me learn introductory SQL. I can study five hours each week. Start with a course plan.

To resume in the same or a different host, supply the actual saved course plan and progress record, then ask Waestro to continue from the pending activity. A reference to an inaccessible earlier chat is insufficient.

## Runtime and progress

This is an instruction package with no build step, provider SDK, or executable dependencies. Browsing, code execution, image generation, image inspection, file creation, and storage depend on the host session and its permissions. The tutor must disclose missing capabilities and use the fallbacks described in the skill. In a text-only session, it can teach through explanations and examples, use the documented image fallback, and provide copyable progress records.

For images, Waestro follows whatever generation and presentation route the host provides, including native tools that display results automatically. It requires no specific image model, service, or file workflow. The tutor checks rendered output when accessible, corrects observed errors, and discloses when visual inspection is unavailable.

The package does not include the original Python CLI, JSON schemas, state validator, or automatic cross-chat storage. A manual resume card is a partial record, not validated canonical Waestro state. Keep learner answers, grades, and filled progress records outside the public repository; `.gitignore` excludes designated private-data locations but does not inspect file contents.

## Repository files

| File | Purpose |
| --- | --- |
| [SKILL.md](SKILL.md) | Provider-neutral tutoring instructions and skill metadata |
| [references/course-planning.md](references/course-planning.md) | Curriculum, boundary assessments, projects, and subject adaptation |
| [references/images.md](references/images.md) | Host-native image generation, presentation, and accuracy checks |
| [references/progress.md](references/progress.md) | Resumption, bookmarks, storage, exports, and review scheduling |
| [references/human-testing.md](references/human-testing.md) | Explicit testing and maintained-project scope |
| [references/provenance.md](references/provenance.md) | Original adaptation notices |
| [resume-card-template.md](resume-card-template.md) | Blank partial progress-export template |
| [LICENSE.txt](LICENSE.txt) | Full GNU AGPL version 3 license text |
| [NOTICE.txt](NOTICE.txt) | Copyright, scope, and original notices |
| [CONTRIBUTING.md](CONTRIBUTING.md) | Contribution and review process |
| [SECURITY.md](SECURITY.md) | Private security and conduct reporting |
| [.gitignore](.gitignore) | Local files and private-data exclusions |

## Contributing and reporting

Ordinary project feedback starts in [Waestro Issues](https://github.com/Techienaut/Waestro/issues/new/choose). Read [CONTRIBUTING.md](CONTRIBUTING.md) before contribution work. Send sensitive reports through the private channel in [SECURITY.md](SECURITY.md).

## License

Distributed under **AGPL-3.0-only**. See [LICENSE.txt](LICENSE.txt) and [NOTICE.txt](NOTICE.txt). Referenced third-party materials retain their own terms. The original notice explains the distinction between covered project material and learner outputs.

Prior adaptation notices are retained verbatim in [the adaptation history](references/provenance.md). `SKILL.md` carries the current reorganization notice. The license, original notices, and blank resume-card template are unchanged.
