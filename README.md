# VOLT — Household Control Center (Live Demo)

This is the standalone, interactive demo of **VOLT**, an autonomous
household resource operator built for the AWS **Agents for Humans
Hackathon 2026** using the Strands Agents SDK.

**Live demo:** deployed via Vercel — see the link on this repo's GitHub page,
or run it yourself: this is a single self-contained `index.html`, so you can
also just open the file directly in any browser. No build step, no server,
no dependencies.

## What this is

A working, interactive Household Control Center: live status cards, an
energy-flow diagram, a plan timeline, a "Plan Replacement" panel that shows
VOLT re-planning when conditions change, an activity feed, and simulation
controls (price spike, solar forecast drop, EV charger failure, etc.) so you
can trigger the same events the full agent responds to and watch VOLT adapt
in real time.

Everything here — the household state, the optimizer logic, the event
handling — is a JavaScript port of the real Python implementation in the
main project repo, so the numbers you see reacting on screen are driven by
the same optimization logic, not a scripted animation.

## The full project

This repo is the UI only. The complete system — domain model, household
simulator, constrained optimizer, Strands agent tools, and device adapter
layer (with a documented, honest breakdown of what's simulated vs. what a
real integration would require) — lives in the main project repo:

**https://github.com/Abdullah49645/volt** *(update this
link once both repos are pushed)*

See that repo's README for the architecture, the "how VOLT would see and
control a real house" integration breakdown, and how to run the full
scenario test suite.

## License

MIT — see [LICENSE](./LICENSE).
