# gh-actions

Hosts GitHub Actions for the BEAM Community.

Provides pre-built workflows and templates that can be easily
used to automate common tasks such as testing, building, and maintaining
libraries.

> **Note:** This repository is a work in progress. We would like to focus on
> providing actions that are useful across the BEAM ecosystem. But we will be
> starting with actions that are useful for the Elixir since that is the
> community we are most familiar with.
> Regardless, we welcome contributions from all BEAM communities.

## References

- [Contributing](./CONTRIBUTING.md) Guide.

## Explanations

### Composition over Configuration

We aim to provide actions that are composable. This means that you can combine
multiple actions to create a workflow that fits your needs and avoid having to
configure a single action to handle all possible use cases.
We are not opposed to providing actions that are more opinionated, or even
entire Workflows, but we will focus on getting the composition right first.

### Primary Audience

As of today, we are focusing on **Library Authors** as our primary audience.
We aim to provide actions that help library authors automate common tasks such as testing, building, releasing, and maintaining libraries.

As we grow, we **MAY** expand our focus to include other audiences such as
**Application Developers**, but that is not our primary focus at the moment
due to the complexity of the use cases involved.

### 80/20 Rule

We aim to provide actions that cover 80% of the use cases with 20% of the
effort. This means that we will focus on providing actions that are useful for
the majority of the BEAM community. We acknowledge that we will not be able to
provide actions for every possible use case. But we will try to provide actions
that are flexible enough to be customized to fit the remaining 20% of the use
cases.

### Launch Stage

- **Preview:** Actions are for testing. No guarantees are provided of any kind.
  You can find them in the `./preview` directory. Expect breaking changes and
  bugs. The intention is to gather feedback and iterate on the design.

- **Stable:** Actions are for production usage. They are supported and
  maintained. You can find them in the `./stable` directory. Expect proper
  SemVer versioning and changelogs.
