# Next Technical Steering Committee Meeting Agenda

- Date: 2024-12-02
- Time: 19:00 UTC

Please file pull requests to add, or discuss items to add, to the agenda.

## Items to Discuss

### New major version of laminas-di (by @tuxrampage)

The `laminas-di` component should receive a new major version to improve its
future maintainability and to support new PHP features.

The details for this process are outlined (and discussed) in the following RFC: https://github.com/laminas/laminas-di/issues/95

### Release Mezzio Router v4 (by @gsteel)

Mezzio router v4 is good to go as far as I can see ([v4 milestone](https://github.com/mezzio/mezzio-router/issues?q=is%3Aclosed+milestone%3A4.0.0)).

The main changes are `final` everywhere and dropped support for callable factories such as StreamFactory and ResponseFactory.

Compat is looking fine with [Fast Route](https://github.com/mezzio/mezzio-fastroute/pull/40) and [Laminas Router](https://github.com/mezzio/mezzio-laminasrouter/pull/35).

Does anyone have any last-minute changes they want to see included or any problems that need highlighting?

### Stale issue/PR cleanup proposal (by @alexmerlin)

We should close PRs that fulfill all of these criteria:

* abandoned (no activity within 1-2 years, also author inactive on GitHub)
* targeting old branches (several versions behind the current/default branch)
* not linked with or created based on an existing issue (because in this case it could be a feature that is needed by someone, the PR might just need to target a newer branch)

Examples:

* https://github.com/mezzio/mezzio-csrf/pull/14
* https://github.com/laminas/laminas-i18n-resources/pull/8

@alexmerlin volunteers to run through the open Laminas/Mezzio issues/PRs and close the ones that match a set of criteria agreed upon.
