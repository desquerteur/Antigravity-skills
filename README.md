# Antigravity-skills

**455 AI coding skills in 14 categories**, including 427 imported packages and 28 original skills.

Browse the [Markdown skill index](CATALOG.md) to find a skill.

## Structure

- `skills/<category>/<skill-name>/`: imported skills with their supporting scripts, references, templates, legal notices, and `SOURCE.json` source records.
- Root-level skill directories: the original 27 skills, kept at their existing paths.

Read a skill's `SKILL.md` and prerequisites, then copy its whole directory into your agent's supported skill location. Keep its resources, source records, and legal notices together. Skills may require additional tools, credentials, or platform-specific dependencies.

## Claude Code

Install the focused router as a Claude Code marketplace plugin:

```text
/plugin marketplace add EpicNori/Antigravity-skills
/plugin install antigravity-skills@antigravity-skills
```

The plugin downloads this library once, then automatically routes substantive software tasks to the most relevant bundled skills. It exposes only the router to Claude Code and loads selected skill instructions on demand, avoiding the context cost and name collisions of registering all 455 skills at once.

Third-party marketplaces do not auto-update by default. Open `/plugin`, select the `antigravity-skills` marketplace, and choose **Enable auto-update**. Claude Code will then refresh the marketplace after sessions start and apply updated plugin files on the next session or after `/reload-plugins`.

To update immediately from a shell:

```text
claude plugin update antigravity-skills@antigravity-skills
```

## Sources and licenses

Imported packages are pinned to upstream commits in their `SOURCE.json` files. These records include the original entrypoint hash and any local adaptations. See [THIRD_PARTY_ATTRIBUTION.md](THIRD_PARTY_ATTRIBUTION.md) and each package's legal notices for its license. Upstream terms remain in effect.

The original 27 packages retain their previous attribution status and have not received a full retrospective dependency or provenance audit. Static import checks do not establish runtime correctness.
