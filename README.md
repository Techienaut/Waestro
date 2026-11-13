> <a href="https://buymeacoffee.com/techienaut"><img src="https://cdn.buymeacoffee.com/buttons/v2/default-yellow.png" alt="Buy Me a Coffee" width="145" height="40"></a>
>
> 💵 Hey guys! 👋 I’m a techie and aspiring programmer/prompt engineer with ADHD and bipolar I. I’m currently unemployed and building open-source tools for education and personal productivity, like Waestro and TechieNotes.
>
> My housing program covers my apartment, so I only need help with my ChatGPT subscription, internet, and basic toiletries (that’s literally all I need to stay afloat lol—I’m very cheap).
>
> ☕ Click the **Buy Me a Coffee badge** to support—even a small donation helps keep these projects going! Thanks for the support 💛

# 🎓 Waestro

[![License: AGPL-3.0-only](https://img.shields.io/badge/License-AGPL--3.0--only-blue.svg)](LICENSE.txt)

## 🧭 1. What Waestro does

- ✨ **Vibe coded:** built with **AI assistance**.
- 🧑‍🏫 **Waestro** helps an AI teach you **one step at a time**: plan a course, explain small ideas, and provide practice.
- 🖼️ Each **concept** gets **exactly one helpful image**, focused on the current step with clear diagrams and useful variety.
- 🏷️ The AI explains each image using **matching labels**.
- 📝 **Quizzes, homework, and practice use text only**.

## 🎬 2. Watch it in action

- 🎞️ **28-second preview:** see **Waestro** in action.

[![Waestro in action: choose Python, review a course plan, learn with diagrams, answer a knowledge check, and request a starter project](docs/media/waestro-skill-highlight.gif)](https://www.youtube.com/watch?v=Q7Tt1KzbnS4)

- 📺 [**Watch the full YouTube demo (21 minutes)**](https://www.youtube.com/watch?v=Q7Tt1KzbnS4).
- 🕰️ The walkthrough shows **v0.0.7**: skill setup, shaping a **Python** curriculum, learning **list comprehensions**, and requesting projects.
- 🔄 The skill continues to change; use this repository’s **current instructions** for its latest behavior.
- 🧰 **Setup and available tools** depend on your **AI app**.

## 📦 3. Set it up

1. 📥 [**Download the ZIP file**](https://github.com/Techienaut/Waestro/archive/refs/heads/main.zip), unzip it, and **keep its files together**.
2. 🧩 If your AI app **supports skills**, add the **whole folder** as a skill.
   - 📎 If it supports **file uploads instead**, attach [**SKILL.md**](SKILL.md), all files in `references/`, and [**resume-card-template.md**](resume-card-template.md).
3. 💬 Start a chat and ask the AI to **use Waestro**, as in the example below.

- 📖 The AI must be able to **read the files**; if it cannot open them, **paste their text when asked**.
- 🖼️ The GIF in `docs/media/` is **documentation only** and can be left out of the skill upload.

## 🐍 4. Example: learn Python

1. ⌨️ **Paste this prompt:**

   > Use Waestro to teach me Python. I am a beginner and can study five hours a week. Make a course plan first. Then teach me one small step at a time.

2. ▶️ **Read the plan.** When you are ready, say:

   > Start the first lesson.

- 🎛️ During a lesson, say **“Go slower,” “Use simpler words,”** or **“Show another example.”**

## 🗺️ 5. Shape the course before you start

- 🎯 Share your **goal, experience, available study time, and preferred difficulty**.
- 🌐 You can learn **subjects beyond programming**.
- ⏭️ If you **skip setup questions**, ask the AI to **state its assumptions before planning**.
- 🗓️ The current **full-course starting estimate** is **16 weeks at 20 hours a week**; your goals, workload, and subject coverage can change the plan.
- 📋 Ask for the **complete plan before lessons begin**:

  > Show the entire curriculum, including every week, section, and module, with outcomes, instructional parts, time estimates, homework, and project plans. Wait for me to review it before teaching.

- 🔎 Review **missing topics, unnecessary repetition, and realistic workload**.
- 🛠️ Request a **harder course**, a **focused refresher**, or a plan based on a **syllabus you supply**.
- 🧗 **Example: make the course more challenging.**

  > Make this Python course more challenging. Include list comprehensions, reduce repetition, and preserve the agreed topic coverage and study time. Explain any tradeoffs before changing the plan.

- 🆕 **Start fresh** rather than continuing an earlier course:

  > Start a new course. Do not use my previous course records or personal memory to choose its content; use only the goals and background I give you here.

## 🧪 6. Learn, check, and practice

### 🎛️ 6.1. Lessons and controls

- 🧠 **Lessons** use short explanations, analogies, examples, and narrated diagrams.
- 🧪 **Knowledge checks** ask you to **explain or apply an idea** and receive feedback.
- 🕹️ **Steer the lesson at any time:**
  - 🔁 **Another explanation:** “Explain list comprehensions using grocery prices as a real-world example.”
  - 🔬 **More depth:** “Explain why this works and show a case where it would fail.”
  - ⏱️ **A different pace:** “Go slower,” “Make this more challenging,” or “Give me a focused review.”
  - 🧭 **Navigation:** “Go to the module on list comprehensions,” then “Back to the course” when you finish the detour.
- ⏭️ **“Skip”** skips the **current question or smallest activity**; name a **module explicitly** to move past the whole module.
- 📌 **Skipped work** stays **unassessed** and does not count as **mastery or completion**.

### 🏗️ 6.2. Homework and projects

- 📚 The course includes **module homework, projects, and assessments**.
- 🪜 **Continuing projects** can grow through **milestones** as you learn more.
- 💻 For **programming**, request a practical assignment with a **clear goal and starter code**:

  > Give me a challenging real-world project using the concepts taught so far. Provide a starter file with TODOs where I write the code and tests for normal and edge cases. Show it in one code block and leave the implementation for me.

- 🛒 **Demo examples:** a **grocery-order project** and a **command-line expense-tracker capstone**; these are examples, not fixed assignments for every course.
- 🔍 Ask for **milestones and feedback** as you build.
- ⚠️ **Generated starter code** and **passing supplied tests** alone do not establish **independent competence**.

## ⏸️ 7. Stop and come back

1. 💾 Before stopping, request your **course plan and progress record**:

   > Pause. Give me my course plan and a progress record, including my next task.

2. 🗂️ **Save or copy both**.
3. 🔄 In a new chat, **load Waestro the same way**, share both records, and say:

   > Continue my course from this record.

- 🧪 **Waestro is an experimental alpha** and still needs **feedback and steering**.
- 🧰 Capabilities depend on your **AI app and model**; **image generation, code execution, and saving files** depend on the tools available in your session.

## 🤝 8. Give feedback or contribute

- 🐛 Describe **what you expected, what happened, and which course or task exposed the problem**.
- 🕶️ Use **synthetic or anonymized examples**.
- 🧪 As discussed in the video, trying a proposed **teaching change on a different subject** can help reveal whether it **generalizes**.
- 📋 Follow the current [**contribution process**](CONTRIBUTING.md), including **maintainer approval before contribution work or opening a pull request**.
- 🤝 [**Help improve Waestro**](CONTRIBUTING.md).
- 🛡️ [**Report a security issue**](SECURITY.md).

## ⚖️ 9. License and notices

- ⚖️ **License:** [**AGPL-3.0-only**](LICENSE.txt).
- 📜 See the repository’s [**notices**](NOTICE.txt).
