---
name: (internal) Component implementation epic
about: (team member use only) Epic issue tracking implementation of a particular component
---

<!--
These issues are used by core contributors to track the list of items that should be
completed as part of creating a v9 component. More info can be found here: https://github.com/microsoft/fluentui/wiki/Component-Implementation-Guide
-->

💡 When you create a PR for any of the checklist items, add a link to this Epic under the PR's **Related Issues** section.

## Preparation

- [ ] [Open UI Research](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#open-ui-research)
  - [link to https://open-ui.org/]
- [ ] [Open GitHub issues related to component](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#find-open-issues-on-github)
  - [link to each issue]
- [ ] [Create react-\* package and component from template](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#component-package)
  - [link to package: https://github.com/microsoft/fluentui/tree/master/packages/react-components/react-(your-component)]
- [ ] (Optional) [Draft implementation](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#draft-and-prototype-implementation)
  - [link to draft implementation, if applicable]
- [ ] [Component Spec authored](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#component-spec) and [reviewed](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#spec-review)

## Implementation

- [ ] [Component implementation](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#implementation)
- [ ] Initial conformance and unit tests (validate basic functionality)
- [ ] [Initial documentation](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#documentation)
  - [ ] [Storybook stories](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#storybook-stories)
  - [ ] README.md covering basic usage
  - [ ] MIGRATION.md guide (include v8 and v0)
- [ ] [Component released as preview](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#preview-release)

## Validation

- [ ] [Add tests](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#tests)
  - [ ] Unit and conformance tests
  - [ ] VR tests
  - [ ] Bundle size fixtures
  - [ ] Accessibility behavior tests
  - [ ] Create an issue and run [manual accessibility tests](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/accessibility-review-checklist.md): [link to issue]
- [ ] [Validate with partners](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#validation)
- [ ] [Run a bug bash with other FUI crews](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#bug-bash)
- [ ] [Finalize documentation](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#finalize-documentation)
  - [ ] Review and add any missing storybook stories
  - [ ] Finalize migration guide
- [ ] [Component released as stable](https://github.com/microsoft/fluentui/blob/master/docs/react-v9/contributing/component-implementation-guide.md#stable-release)
  - [ ] Run the `prepare-initial-release` script to remove the `-preview` suffix from the package name
  - [ ] Deprecate the `-preview` package in NPM
  - [ ] Export the component from `@fluentui/react-components`
  - [ ] In package.json: Remove the alpha/beta tag from the version number in package.json
  - [ ] In package.json: Change beachball's `disallowedChangeTypes` to `"major", "prerelease"`
