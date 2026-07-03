# Contributing

Thank you for contributing to the UCT Department of Electrical Engineering GitHub organisation. This guide explains how we work here. It applies as the default across every repository in the organisation, and appears automatically when you open an issue or pull request in any repository that does not provide its own guide.

For the higher-level purpose and policy of the organisation, see the [organisation profile](https://github.com/uct-eee-department).

## Before you start: does your work belong here?

The organisation is the home for finished and shared departmental work, not a scratchpad. Before creating a repository, decide where it belongs:

- A research group's own organisation, for example the African Robotics Unit, for work specific to that group.
- This departmental organisation, for department-wide teaching materials, shared tooling and cross-group work.
- Your personal GitHub account, for experiments, proofs of concept and work in progress, until it is ready to be [transferred](#transfer-of-ownership).

If you are unsure, ask your supervisor, the course convener or an administrator.

## Getting access

Access is managed through teams rather than individual grants. If you need access to a repository, or a team created for a new project or course, contact a repository administrator, failing which an organisation administrator. You will be given the minimum permissions needed for your role.

## Repository standards

Every repository should be maintained to an above-average standard. At a minimum:

- A clear, current `README.md` that states the purpose of the repository and how to use it.
- A `LICENSE` file for any public repository. Consult your supervisor or convener and the UCT Intellectual Property Guidelines before choosing one.
- A `.gitignore` appropriate to the languages and tools in use.
- A sensible description and topics, so the repository can be found.

Public repositories are held to a higher standard, as they represent the department. They should be well documented, reproducible and useful to others. Develop privately until the work is ready to be public.

## What to commit, and what not to

Repositories should contain text-based assets suited to version control: code, LaTeX, markdown, documentation, most experimental data and other text-based project files.

Do **not** commit:

- **Personal information.** This includes student names, student numbers, EMPL IDs, marks and submissions. This material must never enter a repository, both for privacy reasons and because GitHub is hosted outside South Africa. Keep it on UCT-controlled storage.
- Large or frequently changing binary files, such as images, video, audio and build outputs.
- Proprietary-format documents such as Word, Excel and PowerPoint, where a text-based alternative exists.
- Content tied to a local machine by absolute paths.
- Credentials, keys or tokens of any kind. If you commit one by accident, treat it as compromised, rotate it and tell an administrator.

Marking and analysis **tools** are welcome. Marking **data** is not.

## Workflow

- Work on a branch and open a pull request rather than pushing directly to the default branch of a shared repository.
- Write clear, imperative commit messages, for example "Add ..." or "Fix ...".
- Keep pull requests focused and reviewable.
- For public repositories under active development, maintain a basic continuous integration workflow so that the main branch stays in a working state.

## Transfer of ownership

All work generated as part of a UCT project is governed by the UCT Intellectual Property Policy. Valuable code and data should be transferred to the organisation before or upon graduation, so that it remains available to future students and researchers. Agree with your supervisor on what is valuable, transfer it through the GitHub interface or by pushing to a new organisation remote, and keep a personal fork if you wish to continue the work independently.

## Getting help

- For repository access or permissions: a repository administrator, then an organisation administrator.
- For what belongs where, or for licensing: your supervisor or course convener.
- For conduct concerns: see the [Code of Conduct](./CODE_OF_CONDUCT.md).
