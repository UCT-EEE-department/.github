# UCT EEE Department GitHub Organisation

Welcome to the GitHub organisation for the Department of Electrical Engineering at the University of Cape Town. This page is for members and outlines what this organisation is for and how to use it.

> [!IMPORTANT]
>
> ## Noticeboard
>
> Nothing scheduled at the moment.

## Purpose

This organisation hosts **valuable** code and other assets produced across the Department of Electrical Engineering, spanning teaching, research and departmental tooling. It is the recommended place for staff and postgraduate students to store, version and share work that is well suited to git-based version control.

> [!NOTE]
> Several research groups within the department maintain their own organisations for group-specific work, for example the [African Robotics Unit](https://github.com/African-Robotics-Unit). Where such a group organisation exists, please use it for group-specific work. Use this departmental organisation for department-wide teaching materials, shared tooling and work that does not belong to a single research group.

This organisation is **not** intended as a personal storage space, nor for hosting throwaway proof-of-concept or experimental projects. Please use your own personal GitHub account for such purposes, even when collaborating with other members of the department.

> [!TIP]
> As a member of UCT you have access to the [GitHub Student Developer Pack](https://education.github.com/pack) (students) and comparable resources for staff, which include tools such as GitHub Copilot and GitHub Pro that you can use with virtually no constraints.

## Membership

Membership of this organisation is restricted to EEE staff and postgraduate students. Undergraduates and other external collaborators should be added as collaborators to individual repositories, or to a [team](#teams), as required. Course conveners may add an undergraduate cohort to teaching repositories through a course team for the duration of a course.

Supervisors may make an exception for final-year undergraduate students who will continue to work on a project as a postgraduate student.

> [!WARNING]
> Please refrain from displaying your membership of this organisation on your public GitHub profile unless you are actively contributing to it. Admins can disable this badge if it is misused.

## Teaching Repositories

Because this is a department-wide organisation, course materials are one of its primary uses. This includes lecture notes, LaTeX sources, tutorial and problem sets, and other teaching assets.

- Group each course under a clearly named team (for example `EEE2046F`) and grant access through that team rather than to individuals.
- Keep **student submissions, marks, EMPL IDs and other personal information out of repositories**. These are sensitive and are not appropriate for git hosting. See [Appropriate Contents](#appropriate-contents).
- Memoranda, unreleased assessments and other material that must not reach students should live in **private** repositories with access limited to the teaching team.
- Archive a course repository when a course is retired or substantially restructured, so that the active version is unambiguous.

## Code of Conduct

This code of conduct outlines the required practices for data management and repository standards. It also outlines the [transfer of ownership](#transfer-of-ownership) of valuable code and data from students to the university.

The scope of this is limited to this UCT EEE Department GitHub organisation and its repositories. It does not apply to any other departmental assets or intellectual property hosted elsewhere.

### Repository Standards

Repository-based development is a core skill of modern engineering. All repositories in this organisation should, in general, be maintained to an above-average standard.

#### Public Repositories

In the spirit of open collaboration, staff and students are encouraged to publish their repositories publicly whenever possible. Public repositories will however be held to a very high standard, as they are a reflection of the department and the university. They should be **well documented**, have a **clear purpose**, be **reproducible** and be **useful to others**. They should be considered a publication in their own right.

As a bare minimum, public repositories should have the following:

- A `README.md` file that outlines the purpose of the repository, how to use it, and other essential information.
- A `LICENSE` file that describes the licence under which the repository is released.

> [!CAUTION]
> Please consult with your supervisor or course convener and the [UCT Intellectual Property Guidelines](http://www.rci.uct.ac.za/rcips/ip/overview) before choosing a licence and publishing publicly.

- An appropriate GitHub description, topics and other settings to make the repository discoverable.
- Marked as archived if it is no longer maintained, for example after a student has graduated or a course has been retired.

> [!WARNING]
> If you are actively developing in a public repository, that development should be of a semi-professional standard with regard to [**continuous integration**](https://aws.amazon.com/devops/continuous-integration/).
>
> Otherwise please develop privately, or within your personal GitHub account, until [transferring ownership](#transfer-of-ownership) once done.

Any public repository that does not meet these standards may be made private during regular [audits](#audit). In rare instances, ownership may be pushed back to the contributor. Note that only organisational administrators can change the visibility of, delete or transfer repositories in this organisation.

#### Private Repositories

Private repositories are intended for code and other assets that are valuable but not suitable for sharing publicly. This includes:

- Unpublished research data.
- Code, models, algorithms, designs and other assets that are **proprietary**, **confidential**, in a **patent** process or for whatever reason cannot be in the public domain.
- Unreleased assessments, memoranda and other teaching material that must not reach students.
- Personal information and other content sensitive to ethical and legal considerations.
- Property co-owned with external collaborators without explicit agreement to share publicly.
- Any other information that is valuable but not suitable for sharing publicly.

Although private repositories are not held to the same standard as public repositories, they should still be well maintained and useful to future members. Private repositories are visible to all members of the organisation. To limit clutter, repositories still in early development should only be placed here if truly necessary. Otherwise, please develop within your personal GitHub account until [transferring ownership](#transfer-of-ownership) once done.

> [!TIP]
> You can access most GitHub features through the [GitHub Student Developer Pack](https://education.github.com/pack) without the need for this organisational account.

### External Repositories

Any research or teaching work conducted in collaboration with internal or external partners that involves git-based repositories hosted outside of this organisation should still be mirrored within this organisation where the department retains an interest in it.

> [!NOTE]
> A mirror is a copy of a repository that is kept up to date with the upstream repository. This can be done manually or automatically using GitHub Actions or similar.
>
> A mirror is not a fork. A fork is a copy of a repository made under a new owner, used to propose changes to the upstream project or as a starting point for a new line of development. The two differ in purpose and function.

### Appropriate Contents

Repositories in this organisation should only contain code and other assets that are appropriate for git-based version control. This includes:

- Code.
- Most forms of experimental data.
- Documentation, markdown and simple webpages.
- LaTeX documents.
- Other text-based assets, for example KiCad projects.

Repositories should **not** contain:

- Large binary files that are frequently modified, for example images, videos, audio and build outputs.
- Personal information, including student marks and identifiers, and other content sensitive to ethical and legal considerations.
- Word, Excel, PowerPoint and other proprietary file-format documents.
- Content with absolute paths or other constraints that tie it to a local file system.
- Extremely large amounts of data.

Please maintain a `.gitignore` file in your repository to exclude inappropriate files from being pushed to the remote.

> [!TIP]
> Please consider alternative cloud storage services, such as the 1TB OneDrive storage provided by UCT, or other services offered via [UCT Research Contracts & Innovation](https://uct.ac.za/rci), for files not suitable for GitHub.

### Transfer of Ownership

All UCT projects are governed by the [UCT Intellectual Property Policy](http://www.rci.uct.ac.za/rcips/ip/policy). In general, all code and data generated as part of a research project is the property of UCT. The department implements this for valuable GitHub-hosted IP by transferring ownership from the student to the departmental organisational account before or upon graduation. This ensures that the code and data is maintained and accessible to future researchers and students.

This can be done by either:

- Transferring ownership via the GitHub interface.
  <https://docs.github.com/en/repositories/creating-and-managing-repositories/transferring-a-repository>
- Creating a new remote within this organisation and pushing the code to the new remote.

```zsh
cd /path/to/your/repo
gh repo create uct-eee-department/$REPO_NAME_HERE --source . --remote uct --private --push
```

> [!NOTE]
> When working with multiple remotes, remember to push to all remotes as required.
> e.g. `git push origin && git push uct`
> You can alternatively create a remote with multiple push URLs.

Not all code and data generated as part of a project is valuable. This should be determined between the student and their supervisor, or between staff for teaching material. If the code and data is not valuable, it should not be hosted in this organisation.

Students may maintain their own remote, especially if work is still in progress, or fork back into their personal GitHub account if they wish to continue working on it independently long-term. This is a good way to keep a personal copy for future reference, especially if the original is made private in this organisation.

> [!CAUTION]
> Forks of private repositories are enabled by default, but may be disabled for repositories containing sensitive content. In which case, GitHub will delete all such existing forks.

## Administration

### Member Removal

By default, members will be removed from the organisation upon graduation, or when otherwise deregistered from or no longer employed by UCT. This keeps the organisation membership up to date and easy to maintain.

### Teams

Almost all projects and courses involve more than one person. The recommended approach is to create a team for each project or course, add the relevant members to that team, and assign repository privileges to the team rather than to each individual. This allows fine-grained access control to be applied consistently.

> [!NOTE]
> A dedicated "security" team is granted read permissions to all repositories by default, as shown in the repository settings. This is an organisational setting that cannot be modified by repository admins.

### Permissions

Members and teams should be granted the minimum permissions required to perform their duties. This keeps the organisation secure and reduces the risk of members accidentally performing actions they are not authorised to do.

Creators of teams and repositories are granted admin permissions by default, and are expected to maintain that resource appropriately. Organisational administrators will only exercise repository-level actions when necessary, and are not responsible for administering individual repositories and teams.

Should you require additional repository permissions, please contact one of the repository administrators, failing which you can ask an organisational administrator.

### Audit

The organisation will be audited on a regular basis by the administrators to ensure that it remains secure and that repositories are well maintained. This may be done at any time without notice.

The default action of these audits is to archive stale repositories, and to make private any public repositories that do not adhere to the standards outlined in this document. Any other actions may be taken as required, or otherwise assigned via a repository issue.

### Deleting Repositories

Repositories should only be deleted if:

- The repository is empty or has thoroughly been determined to have no value.
- The repository has been duplicated or otherwise moved.
- There is a legal or ethical reason to do so.

Before doing so, any past contributors still present within the university should be informed of the intent to delete the repository. An organisational administrator may then exercise this deletion.

### Administrators

The following are administrators of this organisation:

- [Robyn Verrinder](https://github.com/robynverrinder) - [robyn.verrinder@uct.ac.za](mailto:robyn.verrinder@uct.ac.za)

___

> [!TIP]
> This landing page lives in a special `.github` repository within the organisation, at `profile/README.md`. It is what visitors see on the organisation's main page.
