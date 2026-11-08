# Waestro

An adaptive, one-on-one AI tutoring skill for planning courses, teaching small concepts, practicing, assessing understanding, and resuming from recorded progress.

This repository packages the supplied **Gemini-oriented Waestro skill**. The four original skill resources are preserved unchanged, including their existing adaptation notice. This is an experimental alpha; the instructions describe intended tutor behavior, not demonstrated learning outcomes.

## What Waestro does

- Plans courses with a Course → Week → Section → Module → Concept → Mini-concept hierarchy.
- Explains one manageable idea at a time, with worked examples and instructional images when the session supports them.
- Separates exposure, assisted practice, independent demonstrations, and retained learning.
- Preserves pending tasks, assessment criteria, assistance history, and return points.
- Provides a partial manual resume card when richer progress storage is unavailable.

## Use the skill

The skill package consists of these four files, kept together in one folder:

```text
waestro/
├── SKILL.md
├── LICENSE.txt
├── NOTICE.txt
└── resume-card-template.md
```

Provide these resources to a compatible skill host using its supported loading mechanism. [SKILL.md](SKILL.md) is the instruction entry point and currently assumes a Gemini conversation. This repository does not provide a host integration or installer.

Once the skill is loaded, a learner can make a request such as:

> Use Waestro to help me learn introductory SQL. I can study five hours each week. Start with a course plan.

To resume, supply the actual saved course plan and progress record, then ask Waestro to continue from the pending activity. A reference to an inaccessible earlier chat is insufficient.

## Runtime and progress

This is an instruction package with no build step or executable dependencies. Browsing, code execution, image generation, image inspection, file creation, and storage depend on the host session. The tutor must disclose missing capabilities and use the fallbacks described in the skill.

The package does not include the original Python CLI, JSON schemas, state validator, or automatic cross-chat storage. A manual resume card is a partial record, not validated canonical Waestro state. Keep learner answers, grades, and filled progress records outside the public repository; `.gitignore` excludes designated private-data locations but does not inspect file contents.

## Repository files

| File | Purpose |
| --- | --- |
| [SKILL.md](SKILL.md) | Supplied tutoring instructions and skill metadata |
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
