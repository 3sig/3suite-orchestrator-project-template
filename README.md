# 3suite-orchestrator-project-template

this repository serves as a template for 3suite-orchestrator projects. see [3lib-orchestrator](https://github.com/3sig/3lib-orchestrator) for more information.

as of writing, it includes:

- 3lib-config setup
- workflow actions for automated building and releasing via tags
- 3lib-orchestrator example setup

## usage

### creating a new project

fork the repository--any changes that we make to the build workflows should be merged upstream to this template.

enable workflows in github so that the build workflows can run.

### creating a release

ensure that you are in a fully committed state before creating a tag.
run `npm run release` (or `bun run release`) and follow the prompts.

### macOS builds

we currently do not support notarization for macOS builds.
to run mac builds, flag them as safe for gatekeeper with the following command:

`xattr -c <path_to_mac_executable>`
