# Pre-flight checklist

## Know the repo
- [ ] Framework and version
- [ ] Package manager and scripts (lint, types, test, build)
- [ ] Routing and page structure
- [ ] Where content lives
- [ ] Where tokens and shared components live
- [ ] Existing patterns for similar UI

## Scope the change
- [ ] Which files change? Which others are affected indirectly?
- [ ] Does a component already do this?
- [ ] Is there a token for every value I am about to write?
- [ ] Can I do it without a new dependency? (see `libraries`)

## While building
- [ ] Semantic element first, ARIA only if needed
- [ ] States covered (see `design` references)
- [ ] Dimensions stable across states
- [ ] Media sized to prevent layout shift
- [ ] Motion has a job and honours reduced motion (see `motion`)
- [ ] No secrets in client code

## Forms
- [ ] Clear labels, plain-language errors tied to fields
- [ ] Input preserved after errors
- [ ] Clear success state and next step
- [ ] No mailing list signup without clear consent
- [ ] Existing behaviour preserved unless asked to change it

## Pages
- [ ] Accurate title, description and social metadata
- [ ] Descriptive headings and links
- [ ] Structured data only if it accurately represents the page

## After building
- [ ] Lint, types, tests, build run, results recorded
- [ ] Keyboard pass done
- [ ] Narrow and wide checked
- [ ] Untested items listed

## Do not
- Add analytics, tracking or third-party scripts without approval
- Assume which CMS, host or form service is used
- Copy raw values into components when a token exists
- Ship placeholder claims
