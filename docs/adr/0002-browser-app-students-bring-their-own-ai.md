# A browser app where students bring their own AI

The app is a website, not a downloadable app, because students of every age and background should be able to start without installing anything. Students pay for the AI themselves: they connect it with "Sign in with ChatGPT" (which spends their ChatGPT plan's allowance) or by pasting an API key from any major AI provider. The app owner does not pay for students' AI usage.

## Considered options

- **Downloadable app, like LearnHarness.** It could run AI the student already has on their computer, such as Claude Code. Rejected for now: most students don't have those tools installed, installing an app turns people away, and Anthropic's rules make using Claude subscriptions from other apps a gray area. A website can be wrapped into a downloadable app later if students ask for one.
- **Using students' Claude subscriptions from the website.** Not possible: Anthropic bans other apps from using Claude Free, Pro and Max plans. Claude is still available through an API key.
- **The app owner pays for the AI.** Rejected: costs grow with every student, and the project is academic research, not a business.

## Consequences

- The app has to work with AI from several providers, so connecting the AI must be built so that adding a provider is a small change.
- "Sign in with ChatGPT" was a limited preview at the time of this decision (November 2026), so access has to be applied for. API keys are the fallback.
- Different AIs teach differently, so every lesson records which model taught it (see ADR 0001).
