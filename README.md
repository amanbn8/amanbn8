# Hi, I'm Aman Bansal

I'm a third-year BTech student in Robotics & AI at Manipal University Jaipur, based in Mumbai.
I contribute to open-source projects (CNCF, OpenWISP, Sugar Labs, AOSSIE, Zulip) and build
developer tools, most recently a CI failure triage agent with an MCP server and AWS Lambda webhook.

## Projects

**[ci-triage-agent](https://github.com/amanbn8/ci-triage-agent)** · Python, MCP, AWS Lambda, Amazon Bedrock

Reads a raw GitHub Actions log and says *why* the run failed and whether a re-run will help.
Fifteen rule signatures (test failures, compile errors, missing deps, network flakes, rate limits,
macOS BSD-vs-GNU tool mismatches, ...), error fingerprinting across runs, flaky-test detection from
JUnit XML, and an LLM fallback on Bedrock only when the rules are unsure. Runs as a CLI, as an MCP
server for AI assistants, and as a Lambda webhook that comments the diagnosis on the pull request.

**[plate](https://github.com/amanbn8/plate)** · Node.js, OpenAI-compatible vision API, Upstash Redis, Vercel

Photo-based calorie and nutrition tracker. Snap a meal, a vision model identifies each food and
estimates grams, and it is matched against a built-in database of 348 Indian and world foods and
drinks. Logs calories, protein, carbs, fat, fibre, sugar and sodium. Zero npm dependencies,
installable as a PWA, with a file store locally and Redis on Vercel.

## Open-source contributions

### Merged

| Repository | Change |
|---|---|
| [cncf/automation](https://github.com/cncf/automation/pull/739) | Fail the maintainers validator on an empty or misspelled `maintainers.yaml` in repo-root mode |
| [cncf/automation](https://github.com/cncf/automation/pull/727) | Fix `check-go-version.sh` false failures on macOS runners |
| [openwisp/netjsonconfig](https://github.com/openwisp/netjsonconfig/pull/419) | Fix truncation of non-ASCII file contents in generated tar archives |
| [sugarlabs/musicblocks](https://github.com/sugarlabs/musicblocks/pull/9113) | Declare missing globals in four widget headers |
| [AOSSIE-Org/Gitcord](https://github.com/AOSSIE-Org/Gitcord-GithubDiscordBot/pull/110) | Validate LinkedIn hostname and profile ID to block phishing URL injection |

### Open

| Repository | Change |
|---|---|
| [openwisp/netjsonconfig](https://github.com/openwisp/netjsonconfig/pull/421) | Add `tls-crypt` support to the OpenVPN backend |
| [zulip/zulip](https://github.com/zulip/zulip/pull/40295) | Use `Intl.RelativeTimeFormat` for the "last seen" status |
| [mesa/mesa](https://github.com/mesa/mesa/pull/3914) | Keep one `GridCell` class for all cells after unpickling a Grid |
| [neuroinformatics-unit/movement](https://github.com/neuroinformatics-unit/movement/pull/1135) | Connect napari widget callbacks only while the widget is visible |
| [cncf/automation](https://github.com/cncf/automation/pull/726) | Fix the glossary reminder guard so the Slack post is skipped on non-Thursdays |
| [AOSSIE-Org/OrgExplorer](https://github.com/AOSSIE-Org/OrgExplorer/pull/279) | Reset pull request data when exploring a new organization |
| [aboutcode-org/alpine-secdb mirror](https://github.com/aboutcode-org/aboutcode-mirror-alpine-secdb/pull/4) | Fetch every secdb file on each sync instead of trusting mtimes |
| [52North/WeatherRoutingTool](https://github.com/52North/WeatherRoutingTool/pull/214) | Make `Boat.get_weather_data()` actually cache the weather dataset |

### Bugs found and reported

- [cncf/automation#737](https://github.com/cncf/automation/issues/737): validator exits 0 on a `maintainers.yaml` with no entries
- [cncf/automation#736](https://github.com/cncf/automation/issues/736): vm-runner pods use a no-permission service account, so preemption auto-rerun never records
- [cncf/automation#735](https://github.com/cncf/automation/issues/735): single matrix `digest` output leaves the `jammy` image with no SLSA provenance
- [aboutcode-org/alpine-secdb#3](https://github.com/aboutcode-org/aboutcode-mirror-alpine-secdb/issues/3): sync never picks up upstream changes that keep the file size the same
- [AOSSIE-Org/OrgExplorer#272](https://github.com/AOSSIE-Org/OrgExplorer/issues/272): analytics page keeps the previous organization's PR data
- [52North/WeatherRoutingTool#213](https://github.com/52North/WeatherRoutingTool/issues/213): weather file reopened and reloaded on every call

## Contact

- Email: [amanbn@icloud.com](mailto:amanbn@icloud.com)
- LinkedIn: [aman-bansal-952093328](https://www.linkedin.com/in/aman-bansal-952093328)
