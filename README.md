# Values Check

**What if you could vote based on your values, and not by party affiliation?**

Most people inherit a party before they ever examine whether that party's actual voting record matches what they believe. This tool flips the order: it asks you 21 plain-language questions about everyday things, tallies which party's *recorded floor votes* line up with your answers, and shows you the receipts, bill number, vote count, and a link to the roll call, for every single question.

No candidates. No campaign rhetoric. Just how Congress actually voted.

**Scope: this is built around the U.S. two-party system and U.S. federal legislation. It is not applicable to other countries' political systems.**

## Why this exists

I wanted to test my own assumption: does the party I identify with actually vote the way I think it does? The only honest way to answer that is to go question by question, value by value, and check it against the real record instead of what any candidate says on TV.

## Methodology

- Each question is a plain-language version of a real piece of federal legislation.
- "True" or "False" is scored against how each party's members actually voted on that bill, not against campaign platforms or public statements.
- Every question links to its source (congress.gov or original reporting) so you can verify it yourself.
- Every vote count and bill citation was checked against primary sources (congress.gov, House Clerk roll calls, or contemporaneous reporting) during development, not taken from memory.
- Skipped questions count as "no stated opinion", they are not silently dropped from the math or divided between the two parties.

## Known limitations (read this before you take it too literally)

- **Selection bias**: these 21 bills were chosen because they had a clean, near-party-line vote. Most legislation in Congress doesn't split that cleanly. This tool oversamples the moments where the two parties look most like opposing teams, and can't show the much larger amount of governing where that isn't true.
- **Not all "sources" are equal weight**: 3 of the 21 questions (Family leave, Right to work, Balanced budget amendment) reflect a consistent one-party sponsorship pattern on a bill that never got an up-or-down floor vote, rather than an actual recorded vote. The source note says so explicitly for each.
- **Parties change over time**: these votes span roughly 2010 to the present. A party's coalition and priorities shift. A vote that defined the party at one point isn't necessarily still the thing that defines it years later. This tool is a snapshot, not a live feed, it won't automatically reflect new floor votes or a party realignment unless someone updates the question set.
- **21 issues is not the whole picture.** This is a sample, not a comprehensive platform comparison.

## How this differs from similar tools

A few tools already do something adjacent to this. Worth naming them so it's clear what's actually different here, rather than pretending this is the first of its kind:

- **[PartyLine](https://www.mypartyline.org/)** matches you to individual incumbents and candidates using real voting records for incumbents and public positions for candidates. Closest existing tool to this one in spirit.
- **[isidewith.com](https://www.isidewith.com/)** and **[Vote Compass](https://votecompass.com/)** match you to candidates or parties based on *stated positions*, campaign platforms, endorsements, not floor votes. That's the exact gap this tool is trying to avoid.
- **[Pew's Political Typology Quiz](https://www.pewresearch.org/politics/quiz/political-typology/)** sorts you into one of nine values-based clusters, but doesn't map to either party's voting record at all.
- **[VoteSee](https://www.votesee.org/)** is a lookup/tracking tool for how your specific representatives vote, not a values quiz that scores you against the two parties.

What's different about this one:

1. **Party-level, not legislator-level.** This isn't "which of 535 people matches you," it's a narrower question: does the party you'd pick actually vote the way you think it does, based on how that party's members voted as a bloc.
2. **Every answer is sourced inline**, bill number, vote count, and a link to the roll call, not just an aggregate score you have to trust.
3. **Skipped questions are their own category, not silently dropped or split.** Answering "no opinion" on most questions doesn't get inflated into a confident partisan lean, see the results logic for details.
4. **Fully open source and auditable**, every question's source is linked inline, rather than a black-box scoring engine.
5. **Deliberately narrow scope.** 21 issues, one country, one legislature. It doesn't try to be a comprehensive platform comparison, just a check on one specific question.
6. **No data collection, by architecture, not just policy.** This is a single static HTML file with no server, no account system, and no network requests. There's no email field to fill in and no way for one to be added later without the code itself changing, visibly, in a public repo.

## Running it

Open `values_check.html` in any browser. No build step, no dependencies.

## Contributing

PRs are welcome, new questions on issues not yet covered, corrections to existing ones, fixed links. Every submission gets checked against a standard, see [CONTRIBUTING.md](./CONTRIBUTING.md) before opening one.

## License

MIT. Fork it, adapt it, add more questions, use it for your own state or country. Just don't misrepresent the vote data.

---

*This tool is not affiliated with any political party, candidate, or campaign. It reflects a fixed snapshot of recorded Congressional votes, most from 2010–2025, and is not updated automatically as new votes happen or parties change.*
