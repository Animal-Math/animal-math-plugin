---
name: find-math-worksheets
description: Find free Animal Math worksheets, worksheet makers, quizzes, teaching tools and curriculum lessons for Pre-K to 5th grade, and hand them over as checked links. Use when a teacher or parent asks for math worksheets or printables, practice on a math skill, a worksheet generator set up a certain way, a math quiz, a lesson plan, a unit test or exit tickets, a week of math practice, or resources for a math standard (Common Core, TEKS, B.E.S.T., SOL and other state codes).
---

# Animal Math worksheets and lessons

Animal Math (animalmath.com) is free: every printable, maker, quiz, tool and curriculum, with no account.
The Animal Math connector's tools find them and check every link, so give only links its tools return.
Never build an animalmath.com address by hand.

## What there is

- **Printables**: ready-made PDF packs, most with answer keys. The curricula's lesson plans, exit tickets,
  pre-checks, unit reviews and unit tests are printables too.
- **Worksheet makers**: pages that draw a new worksheet each time, with settings (numbers, problem type,
  answer key, the title).
- **Quizzes**: on-screen quizzes with levels.
- **Tools**: on-screen teaching tools (ten frames, base ten blocks, a teaching clock, ...).
- **Curricula**: a full year for kindergarten to 5th grade, in units of numbered lessons (4.3). Each lesson
  has a lesson plan, an exit ticket and the sheets, maker, quiz and tool its plan names.

## How to answer

1. **Find what fits** with `search_resources`: the skill in a teacher's words, the grade, and the kind when
   they named one. For a standard, pass its code as `standard` (and `standard_set` when the state is known).
   Pick the few best fits rather than listing every result.
2. **A maker set up a certain way**: `get_maker_settings`, then `build_maker_link` with the settings that
   match the request (`answerKey: 1` for answer keys, `headerText` for the title on the sheet). If
   anything comes back under `not_used`, fix it from the values listed and call again.
3. **A curriculum lesson or unit**: `get_curriculum` (with a grade, then a `unit` for its pre-check,
   review and test) and `get_lesson` for one lesson.
4. **More than one thing**: put them in one set with `make_set_link`, using the `item` of each result
   (a lesson's `item` brings its plan page, sheets, maker and exit ticket with it). Give the set a short
   title. Use `days` for a plan of several days. If items come back under `not_found`, swap in the
   `did_you_mean` item or drop them and call again: the short link is made once every item is found.
5. **Reply** with the short link first (animalmath.com/s/...), then one short line for each thing in it:
   what it is and why it fits. Say that the set page prints all its printables as one PDF, with or
   without answer keys.

## Good to know

- A maker gives new problems every time it opens, so the same link makes a fresh sheet for each day.
- Grades: printables, makers, quizzes and tools go from Pre-K to 5th grade; the curricula go from
  kindergarten to 5th grade. Lessons marked ★ are taught in that grade only in some states.
- Animal Math also has iPad apps, which cost money; the tools never list them, so don't offer them.
- When nothing fits, say so plainly, offer the closest worksheet maker, and mention that teachers can ask
  for a new worksheet at https://animalmath.com/suggest/.
- Without the connector (its tools missing), read https://animalmath.com/llms.txt, which says how to build
  the same links by hand, and open each link before giving it.
