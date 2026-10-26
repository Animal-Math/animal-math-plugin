# Animal Math

Free math worksheets, worksheet makers, quizzes, teaching tools and full-year curricula for Pre-K to
5th grade, from [animalmath.com](https://animalmath.com), handed to you by Claude as links that work.

## Use it

Add the plugin, then connect its **Animal Math** connector on the plugin's Connectors tab. It needs no
account and no sign-in. Then ask Claude for what your class or child needs, for example:

- "Find 2nd grade worksheets on subtraction with regrouping, with answer keys."
- "Make me a telling time worksheet maker set to drawing the hands, quarter hours, with an answer key."
- "Put together a week of 3rd grade fractions practice, one link for each day."
- "Give me lesson 4.3 of the 4th grade curriculum: the lesson plan, the sheets and the exit ticket."
- "What do you have for TEKS 3.4A?"

Claude finds the resources with the connector's tools, checks every link on animalmath.com, and gives you
one short link (animalmath.com/s/...) to a set page, which prints all its printables as one PDF, with or
without answer keys. A worksheet maker link opens the maker already set up, with new problems each time.

The connector also works on its own: in Claude, open Customize > Connectors, choose + Add, then Add custom
connector, paste `https://animalmath.com/mcp` and choose No sign in. Step by step:
[animalmath.com/use-with-chatgpt-claude](https://animalmath.com/use-with-chatgpt-claude/).

## What's in the plugin

- **The Animal Math connector** (`.mcp.json`): animalmath.com's MCP server at `https://animalmath.com/mcp`,
  with six read-only tools: find resources, a maker's settings, a maker link, the curricula, one
  curriculum lesson, and a set link.
- **The find-math-worksheets skill**: tells Claude when to use the connector and how to answer: find the
  best fits, set a maker up, put several things in one set, and give the short link first.

## Data

The connector's tools send animalmath.com what Claude asks them for: topic words, a grade, a standard's code,
a worksheet maker's settings, or a set's title, note and items. Animal Math answers and keeps only a count of
each call (which tool and how many results, never the words), and each set link's title, note and items,
saved under its short code so the link keeps working. Nothing else is stored, and nothing is sent anywhere
else. Privacy policy: https://animalmath.com/about/#privacy. Terms of use: https://animalmath.com/about/#terms.

## License

Apache License 2.0 (see `LICENSE`), for the files in this repository. The worksheets themselves are free for
personal, educational and classroom use under Animal Math's [terms of use](https://animalmath.com/about/#terms),
and the license gives no right to use the Animal Math name or logo.
