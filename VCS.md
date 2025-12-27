# VCS
A version control system (VCS) tracks changes to files over time, allowing developers to manage code versions, collaborate effectively, and revert mistakes easily. It serves as a safety net for software projects by recording who made changes, when, and why. Common examples include Git for distributed control and older systems like SVN for centralized setups.
## Types of VCS
- **Centralized (CVCS):** Relies on a single server repository where users check out files, make changes, and commit back; examples include Subversion.
- **Distributed (DVCS):** Each user has a full local copy of the repository, enabling offline work and local commits; Git is the leading example.
## GIT
Git serves as a distributed version control system (DVCS) that tracks changes in codebases, enabling developers to collaborate, experiment safely, and maintain project history locally and remotely. Unlike centralized systems, Git gives every user a complete repository copy for offline work, fast operations, and resilience against server issues.
## GIT Commands
### git init 
> **git init** initializes a new Git repository in the current directory by creating a hidden **.git** folder that stores all metadata, configuration, and history for version control. This command sets up the essential structure for tracking changes but does not add or commit any files yet. After running it, use git add and git commit to start versioning your project files.

```git log```

```git log --oneline```
