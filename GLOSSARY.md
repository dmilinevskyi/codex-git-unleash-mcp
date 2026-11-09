# Git Operation Policy

The language used to describe which Git and GitHub operations a caller may perform and where they apply.

## Language

**Repository**:
A Git repository whose history and branches may be shared by multiple worktrees.
_Avoid_: Worktree when referring to the shared repository

**Worktree**:
A checkout of a repository with its own working files, staging area, and current branch.
_Avoid_: Repository when referring to a particular checkout

**Effective Policy**:
The permissions and preferences that apply to a repository after its policy base and repository overrides are combined.
_Avoid_: Config when referring to the resulting policy

**Policy Base**:
The starting policy supplied by the repository itself, or by global defaults when no repo-local policy exists.
_Avoid_: Policy source when referring to the origin of every effective value

**Repository Override**:
A repository-specific policy value supplied through global configuration that takes precedence over the policy base.
_Avoid_: Global default

**Preferred Workflow**:
The recommended way to begin work in a repository: use a linked worktree, use a feature branch in the current worktree,
or remain on the current branch.
_Avoid_: Allowed workflow when expressing a preference

**Allowed Workflows**:
The permitted ways to set up work in a repository, including whether branch creation and switching are permitted.
_Avoid_: Workflow preference

**Allowed Branch Pattern**:
A rule identifying branch names permitted as mutation targets or as branches to create or switch to.
_Avoid_: Branch naming template

**Branch Naming Template**:
A suggested form for a new branch name that does not itself grant permission to use that name.
_Avoid_: Allowed branch pattern

**Base Branch**:
The branch from which a new branch starts, into which a pull request proposes changes, or from which base
synchronization brings changes.
_Avoid_: Policy trust reference when describing an operation's base

**Policy Trust Reference**:
The authoritative version of repo-local policy against which local policy copies are checked.
_Avoid_: Operation base when referring to policy authority
