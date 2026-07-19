# HeadCache

> A low-overhead document system.

> Organize as little as possible. Retrieve as easily as possible.

> HeadCache is a system of connected feedback loops.

Just like a CPU cache keeps frequently needed data close for faster access, HeadCache keeps your knowledge accessible without requiring constant mental effort.

Your brain is for thinking, not for remembering or organizing files.

Many productivity systems become projects of their own. You spend more time refining folders, tags and workflows than actually getting work done.

HeadCache exists to prevent exactly that.

**Your notes should support your work, not become your work.**

It is a low-overhead document system built around one simple idea:

Let your brain COAST...

## About HeadCache

Most knowledge management systems fail for a surprisingly simple reason:

They require too many decisions.

Should this become a new folder?
A tag?
A project?
A permanent note?

Every additional decision creates cognitive overhead.

HeadCache intentionally reduces those decisions to a minimum.
It favors writing over organizing, searching over browsing and shipping over polishing.

## What HeadCache is not

HeadCache is not:

- another productivity system to maintain.
- a replacement for your editor.
- a database with a custom format.
- a complex organization framework.

It is simply a way to keep your thoughts accessible with minimal overhead.

## Inspired by

HeadCache is inspired by several well-established ideas:

- **PARA (Tiago Forte)** – project-oriented organization.
- **Zettelkasten (Niklas Luhmann)** – connected knowledge through atomic notes.
- **Kanban (Taiichi Ohno)** – reducing work in progress and focusing on flow.

HeadCache does not attempt to replace these systems.
Instead, it borrows the ideas that reduce cognitive overhead while intentionally leaving out unnecessary complexity.

## Design Principles

- Capture first. Organize later.
- Search beats hierarchy.
- One idea, one note.
- Every new category must justify its existence.
- The file system is your database.
- Markdown is future-proof.
- Plain text beats vendor lock-in.
- Prefer doing over organizing.
- Solve today's problems, not hypothetical ones.

## COAST - The four Loops

COAST is a acronym for the following words:

- **C**apture -> Capture first. Decide later.
- **O**rganize -> Avoid organizing for hypothetical future needs.
- **A**ct -> Execute tasks when their time has come. Don't stress yourself.
- **S**tore -> Keep knowledge alive. Refine it. Expand it. Reuse it.
- **T**each -> Share what you've learned through articles, documentation, tutorials or talks.

HeadCache has no "workflow" as in other systems like PARA or Kanban.
Think about it more like feedback loops.

### The Capture Loop

Everything starts with an idea or thought that "flashes" through your mind.
Hold it! Write a quick and dirty note in your inbox.
No refining or overthinking, just use your own words, small as possible, what runs through your head and distracts you.

**Never keep ideas in your head!**

Triage your inbox regularly. Now decide what has to be done with that idea.
Is it worth to create a project? Create it.
Is it long-term knowledge, that may help in future projects? Create a refined zettel out of it.

The only decision you need to make is how often you review your inbox.

### The Knowledge Loop

Knowledge is not something you collect once and store forever.
It is something that grows through use.

A zettel starts as an answer to a question, a solution to a problem or an insight from a project.

Over time, connect it with related ideas, refine your understanding and reuse it in new situations.

A good zettel saves future you from solving the same problem twice.

Knowledge compounds.

### The Action Loop

> Projects are the main place where this loop happens, but the same principle applies to any task that requires learning.

You created a project. Great! What now?
Ask yourself "Do I have all knowledge I need to finish it?"
If your answer is no, keep doing research.
While doing research don't forget to capture the things you have learned.
Just put it in your inbox or create a refined zettel out of it and link it to your project.

Capture your research steps inside your project folder, you have to be able to read what you had to do to gain that knowledge later on.

**Keep in mind your zettel should not contain the steps you needed to gain that knowledge, only the knowledge about a specific topic you needed.**

Ones you have finished that project move it to the archive.
During or after a project, decide if the gained knowledge should become reusable output.
This can happen as documentation, tutorials, blog posts or other forms of teaching.
Decision depends on your time and current "workload".

### The Output Loop

Knowledge becomes valuable when it leaves your personal system.

Writing an article, creating documentation or teaching someone else forces you to organize your thoughts and exposes gaps in your understanding.

Those gaps create new questions.

New questions create new knowledge.

Teaching is not the end of learning. It is another way learning continues.

### Conclusion

Capture quickly, organize only when necessary, act when needed, store what matters and teach what you've learned.

These loops are not independent processes. They constantly feed each other.

The Capture Loop prevents ideas and questions from getting lost.

The Action Loop turns intentions into real-world experience and reveals gaps in your knowledge.

The Knowledge Loop transforms those discoveries into reusable understanding.

The Teaching Loop turns understanding into value and creates new questions, ideas and improvements.

HeadCache is not about storing information.
It is about creating a system where knowledge continuously evolves through action.

```
                  CAPTURE
                     ○
                  ↙    ↘
                 /       \
                ▼         ▼
          PROJECT  ◄──► KNOWLEDGE
                ▲         ▲
                 \       /
                  ↖    ↙
                     ○
               TEACH / OUTPUT

```

Projects expire.
Knowledge evolves.
Projects are temporary workloads. Knowledge is the cache that makes future work faster.

## Folder structure

The following folder structure is the reference implementation of HeadCache.

Feel free to adapt it to your own needs without changing the underlying principles.

```
.
├── 00_inbox
│   └── README.md
├── 01_active
│   ├── projects
│   ├── routines
│   │   ├── 00_daily
│   │   ├── 01_weekly
│   │   ├── 02_monthly
│   │   └── 03_yearly
│   └── README.md
├── 02_zettelkasten
│   └── README.md
├── 03_archive
│   └── README.md
├── 04_output
│   └── README.md
├── 99_templates
│   ├── inbox.md
│   ├── zettel.md
│   └── output.md
└── README.md
```

### Inbox

Think of the Inbox as Dumbledore's Pensieve.

Whenever a thought distracts you, don't keep it in your head.
Put it into the Inbox and continue working.

### Active

Here is the place for your tasks or projects.

Time to take action, but don't overwhelm yourself.
Limit the amount of active things you keep here.

**Important:** Keep your routines healthy before adding more projects.

#### projects

Projects are "one-time" things with a defined output. Put active projects here.

Use a subfolder for each project, give it a strong memorable name.

As soon as you have finished, move them to the archive.

#### routines

An important view on routines, think of routines as never-ending projects with a periodic renewal.

Here is the place for your recurring tasks.
Use one file per routine, describe it like you had forgotten everything about it.

Once a recurring task becomes obsolete, move it to the archive!

### Zettelkasten

HeadCache uses the idea of small, connected notes.
You don't need to understand the full Zettelkasten methodology to benefit from it, but reading about it is definitely worth it.

Unlike projects, knowledge is never "finished".

As your understanding grows, your notes evolve with it.
Over time they become the foundation for articles, documentation, tutorials and other forms of output.

### Archive

Pretty self-explanatory. Store things here that are no longer active, but might still be useful someday.
Think of it like "cold storage" on a NAS.

### Output

This is meant to store your output, like blog posts, tutorials, documentation and even possible books.

Knowledge that never leaves your notebook has limited value.

Write articles.
Create documentation.
Share tutorials.
Explain concepts.

**Teaching is how knowledge becomes useful.**

### Templates (Optional)

This folder is entirely optional and can be customized or trimmed to fit your workflow.

The examples included here are designed to work well with Obsidian and Hugo.

What is the purpose?

Since the system is designed to minimize mental overhead, it also makes sense to rely on templates.

The goal is not only to reduce the mental effort required to organize your notes but also to minimize interruptions to your workflow. We want to capture ideas as quickly as possible. Having to stop and think about which type of Markdown file to create adds unnecessary friction.

Instead, simply start with an appropriate template and focus on the idea you want to capture.

## File naming

There is no required file naming convention. However, it is recommended to choose descriptive, memorable names so files are easy to recognize and find later.

For consistency and improved searchability, consider using [snake_case](https://developer.mozilla.org/en/docs/Glossary/Snake_case) for file names.

For example:

`idea_create_second_brain.md`

or

`blog_article_about_my_second_brain.md`

## Your notes, your tools

HeadCache works with any editor.

Use Vim.
Use VS Code.
Use Obsidian.
Use Notepad.

It doesn't matter.
Your notes belong to you. Your tools are just interfaces.

HeadCache assumes that searching is faster than navigating deep folder hierarchies.
Organize just enough to find things again and let your search tool do the rest.

## Quick Start

1. Create the folder structure, clone or fork this repository.
2. Put every idea into `00_inbox`.
3. Review your inbox regularly.
4. Move actionable work to `01_active`.
5. Move long-term knowledge to `02_zettelkasten`.
6. Archive finished work.
7. Publish what you've learned.

As a first step, I recommend learning about `git` and the Zettelkasten Method.

Use these topics as your first projects:

- Learn the basics.
- Capture your discoveries.
- Create reusable zettel from the knowledge you gain.
- Link those zettel to related ideas.

Afterwards, create an article, tutorial or documentation about `git` or the Zettelkasten Method.

You do not have to publish it.

The goal is to experience the complete HeadCache cycle:

Capture → Learn → Create Knowledge → Teach → Improve Knowledge

This is how HeadCache is meant to be used.

## Finally ...

HeadCache doesn't try to organize everything. It tries to minimize the number of decisions required to stay organized.
Every organizational decision has a cognitive cost. HeadCache exists to keep that cost as close to zero as possible.

It helped me to solve my "writing docs" issue, I hope it can solve yours too.

## Further information

Please take a look at [ABOUT.md](ABOUT.md)
