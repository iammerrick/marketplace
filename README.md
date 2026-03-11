# iammerrick marketplace

A [Claude Code plugin marketplace](https://code.claude.com/docs/en/plugin-marketplaces) by Merrick Christensen.

## Install

```shell
/plugin marketplace add iammerrick/marketplace
/plugin install hire-merrick@iammerrick
```

Or via the CLI:

```bash
claude plugin install hire-merrick@iammerrick
```

## hire-merrick

Learn about Merrick Christensen — experience, skills, values, and why you should hire him.

### Skills

#### `/hire-merrick:hire`

Opens your default email client with a message to Merrick. Subject line: "We want to hire you."

```shell
/hire-merrick:hire
```

#### `/hire-merrick:history`

Opens Merrick's resume in your browser and offers to download it as a PDF. Then fetches his latest [resume](https://merrickchristensen.com/resume) and [work history](https://merrickchristensen.com/work) to answer any questions you have about his experience, roles, and career.

```shell
/hire-merrick:history
```

You can also pass a path to save the PDF directly:

```shell
/hire-merrick:history ~/Desktop/merrick-resume.pdf
```

#### `/hire-merrick:why`

Fetches Merrick's [user guide](https://merrickchristensen.com/user-guide) and summarizes his core values, then presents his mission and what he cares about:

- **Mission**: To alleviate human suffering. Lately, that means empowering anyone to build software without code, creating broader economic access to this wonderful thing called the internet.
- **Technical Quality**: Builds constraint engines, type systems, and programming languages. Emotionally invested in craft because people depend on what he ships.
- **Mission-Oriented Companies**: Looking for companies where the mission drives decisions, not just the pitch deck.

```shell
/hire-merrick:why
```

### Agents

#### `recruiter`

A specialized agent for recruiters and hiring managers evaluating Merrick for a role. Compares role requirements against his actual experience — forthcoming about gaps as well as strengths.

Strengths it highlights when relevant:
- Deep systems architecture (programming languages, type systems, constraint engines)
- Shipped platform/infrastructure at scale (Webflow, Domo)
- AI-native development — drove adoption across engineering orgs
- First engineer promoted through Staff, Senior Staff, and Principal at Webflow

Example usage:

```shell
@hire-merrick:recruiter Can you see if Merrick is a good fit for <job-posting>
```

Considerations it surfaces:
- Needs autonomy and ownership
- Values-driven and direct — thrives in cultures that value authenticity
- Wants mastery and challenge
- Prefers finishing one thing well over juggling many things poorly

## Learn more

- [merrickchristensen.com](https://merrickchristensen.com)
- [merrickchristensen.com/resume](https://merrickchristensen.com/resume)
- [merrickchristensen.com/work](https://merrickchristensen.com/work)
- [merrickchristensen.com/user-guide](https://merrickchristensen.com/user-guide)
