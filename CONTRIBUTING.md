# Contributing

Thank you for taking the time to contribute! This is a curated list — quality matters more than quantity. Please read these guidelines before opening a pull request.

## What belongs here

- The resource must be **MV3-relevant**. Tools, libraries, or guides that only work with Manifest V2 don't fit.
- It must be **actively maintained**. As a rough rule: a commit or release in the last 12 months, or active issue triage. Stale projects get removed.
- It must be **substantial**. Toy demos, single-blog-post tutorials, or thin wrappers without traction don't belong.
- It must be **free of malware and trackers**. No analytics-laden CLIs, no obfuscated bundles.

## What does NOT belong

- MV2-only tools.
- Personal extensions or one-off projects (unless they're a notable example others would copy from).
- Tutorials older than 2 years (the platform shifts too fast).
- Anything you're paid to promote without disclosure.

## How to add an entry

1. Fork this repository.
2. Add your entry to the relevant section.
3. Use this exact format:

   ```markdown
   - [Name](URL) - Short description ending with a period.
   ```

   - Name should match the project's canonical name (with capitalization).
   - Description should be **one sentence**, start with a capital letter, end with a period, and stay under ~100 characters.
   - Don't use marketing language ("the best", "ultimate", "blazing fast"). Describe what it does, not why it's great.

4. Keep each section **alphabetized** by entry name (ignoring `@` prefixes and articles).
5. Run `npx awesome-lint` locally before submitting — CI will run it on your PR.

## Suggesting a new section

Open an issue first. Sections need at least 3 high-quality entries to exist.

## Removing entries

If you spot a stale, abandoned, or broken resource, open an issue or a removal PR. Removing dead links keeps the list trustworthy.

## Code of conduct

By participating, you agree to abide by the [Code of Conduct](CODE_OF_CONDUCT.md).
