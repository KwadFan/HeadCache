# HeadCache

> A low-overhead document system.

> Organize as little as possible. Retrieve as easily as possible.

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

## The COAST Workflow

The COAST workflow describes how HeadCache reduces friction when capturing knowledge, planning work and managing tasks.

- **C**apture -> Capture first. Decide later.
- **O**rganize -> Avoid organizing for hypothetical future needs.
- **A**ct -> Execute tasks when their time has come. Don't stress yourself.
- **S**tore -> Keep knowledge for future reference, like a Zettelkasten.
- **T**each -> Simply transform knowledge into output! Teach others or teach yourself new things.

This is also the "workflow" for this system.<br>
Capture -> Organize -> Act -> Store -> Teach

```
                  HEADCACHE

          ┌─────────────────────┐
          │ Capture Everything  │
          │      00_inbox       │
          └──────────┬──────────┘
                     │
                     ▼
          ┌─────────────────────┐
          │ Periodic Review     │
          └───────┬─────┬───────┘
                  │     │
     Need Action? │     │ Worth keeping?
                  │     │
                  ▼     ▼
         ┌────────────┐ ┌────────────────┐
         │ 01_active  │ │02_zettelkasten │
         │Projects    │ │ Connected Notes│
         │Routines    │ └────────┬───────┘
         └──────┬─────┘          │
                │                │
                ▼                │
          ┌──────────────┐       │
          │     Done     │◄──────┘
          └──────┬───────┘
                 │
                 ▼
          ┌──────────────┐
          │ 03_archive   │
          └──────┬───────┘
                 │
                 ▼
          ┌──────────────┐
          │ 04_output    │
          │ Share & Teach│
          └──────────────┘
```

The only decision you need to make is how often you review your inbox.

Everything that is no longer active, like a finished project, should be moved to the archive.

Capture quickly, organize only when necessary, act when needed, store what matters and teach what you've learned.

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

Once a recurring task becomes obsolete, move it in the archive!

### Zettelkasten

HeadCache uses the idea of small, connected notes.
You don't need to understand the full Zettelkasten methodology to benefit from it, but reading about it is definitely worth it.

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

This is not part of the core concept, just a convenience layer to reduce friction even further.
Having some handy templates should reduce overhead and work in one go.

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

1. Create the folder structure, or fork this repository.
2. Put every idea into `00_inbox`.
3. Review your inbox regularly.
4. Move actionable work to `01_active`.
5. Move long-term knowledge to `02_zettelkasten`.
6. Archive finished work.
7. Publish what you've learned.

## Finally ...

HeadCache doesn't try to organize everything. It tries to minimize the number of decisions required to stay organized.
Every organizational decision has a cognitive cost. HeadCache exists to keep that cost as close to zero as possible.

It helped me to solve my "writing docs" issue, I hope it can solve yours too.

## Further information

Please take a look at [ABOUT.md](ABOUT.md)
