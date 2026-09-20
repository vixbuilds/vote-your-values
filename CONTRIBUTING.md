# Contributing

Pull requests are welcome, especially new questions covering issues not already in the set, or corrections to existing ones. Before opening a PR, please read this.

Every question in this project maps a plain-language value statement to a real, verified Congressional floor vote. That's the whole premise, so every submission gets checked against the same standard before it's merged.

## Checklist for new or edited questions

**1. Real recorded vote, independently verified**
Cite the bill number, the Congress, and the vote count, and link a primary source (congress.gov, clerk.house.gov, senate.gov) or contemporaneous reporting. A vote count that can't be verified against a primary source won't be merged, no matter how confident the citation sounds. "This bill was mostly party-line" is not a citation; a specific roll call is.

**2. Root-goal-first wording**
Write the value tension in plain language first, then find the bill that proves it played out in a real vote. Don't reverse-engineer a sentence from a bill's technical mechanics; that's how jargon and mischaracterizations creep in. A good test: would someone with no policy background understand the question without needing the source note to parse it?

**3. No loaded premises, no false dichotomies**
Don't state a contested empirical claim as settled fact inside a T/F question (e.g. "X is working, so..."). Don't bundle two separate claims into one statement, if someone could agree with the first half and disagree with the second, split it into two questions. Don't frame two policies as mutually exclusive if they aren't.

**4. Sympathetic, not a strawman**
A question should read the way someone who actually holds that position would describe their own view, not a caricature of it. If a question reads like it was written by someone who disagrees with that side, it'll be rejected regardless of whether the vote citation checks out.

**5. Balance**
Before merging, the maintainer will recheck the overall split of "True = Democratic-aligned" vs. "True = Republican-aligned" questions across the full set. A PR that adds one side without the other may be asked to include a counterpart, or an existing question may be flipped to compensate. The goal is that blindly answering "True" to every question should land close to 50/50, not favor either party.

**6. No unnecessary topic overlap**
Check the existing question list before adding a new one. If a topic is already covered, propose a genuinely distinct angle on it, or don't duplicate it.

## What happens to PRs that don't meet this bar

They'll get feedback, not a silent close. If a question is a good idea but poorly sourced or worded, the maintainer may suggest a rewrite rather than rejecting it outright. This is a judgment call every time, not an automated check, so response times may vary.

## Fixing an existing question

If you spot an error, a stale link, a mischaracterized bill, or an unbalanced question, open a PR or an issue. Every citation was checked against primary sources during development, but new errors can still surface, especially as bills age or get amended. That's expected, not embarrassing.
