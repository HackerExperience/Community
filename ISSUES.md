# Base Issue Categorization Process

This document outlines the standard way we tag and categorize issues within a repository. Each team or repository may extend or overwrite this process. If no ISSUES.md is found, we can assume the repository follows this process.

**This is an initial draft and a lot is supposed to change.**

## Defining Priority

Issues may use any of the following two labels to increase/decrease priority:

- `Priority:High`
- `Priority:Low`

If an issue has normal priority, our recommendation is to simply not add any label to it. It reduces visual bloat and implies that the issue is neither low- nor high-priority.

## Defining difficulty

Difficulty tags are useful to inform contributors of the challenges they could be facing.

- `Difficulty:VeryHard`
- `Difficulty:Hard`
- `Difficulty:Normal`
- `Difficulty:Easy`
- `Difficulty:Unknown` - Difficulty hasn't been triaged yet.

Some tasks' difficulties are hard to quantify. The quality of the description, ease of replication and presence of clear "steps to fix" can turn a VeryHard task into an Easy one. On the other hand, lack of these details can turn an Easy task into a VeryHard one.

It's possible there may be disagreement on the actual difficulty of some tasks. In these cases we recommend multiple Difficulty tags be applied.

There's no need to categorize a task's difficulty unless it's ready to be listed as `UpForGrabs`.

## Defining Type

Issues may have completely different types. Here are the accepted labels:

- `Type:Problem` - Problem, flaw or bug relevant to the repository scope.
- `Type:Discussion` - Discussion towards a common subject.
- `Type:Feature` - Addition of something new to the repository. More relevant to software repositories.
- `Type:Enhancement` - Enhancement of something that already exists on the repository.
- `Type:Question` - Simple and direct question about something.

A single issue may have multiple types. For example, a `Question` may spark a `Discussion`.

## Misc

- `UpForGrabs` - Small, actionable task that can be worked on by external contributors. It may not be friendly (lacking description, steps to replicate, requires specific knowledge).
- `ContributorFriendly` - Task is friendly to external contributors. It means it has a nice description, it's easy to replicate and it doesn't require extensive knowledge of the software/project. `ContributorFriendly` tasks are not necessarily `Difficulty:Easy`. All `ContributorFriendly` tasks are also `UpForGrabs`.
- `NeedsTriage` - Issue still hasn't been tagged properly.
- `NeedsDescription` - Issue is lacking description, or its description is too vague.
- `NeedsFeedback` - Feedback/opinion from other contributors is wanted before reaching a conclusion.
- `NeedsInput` - Task resolution is blocked until it receives input from someone.

## Status

Status is a good way to represent workflow. It's usually more relevant to code implementations.

- `Status:Unconfirmed` - Task hasn't been confirmed by developers, meaning it may not be valid in some way (invalid report, already implemented, it's a feature not a bug, etc).
- `Status:Accepted` - Task was acknowledged by developers, it is something that must be worked on.
- `Status:Planned` - Task has been added to monthly, weekly or daily planning.
- `Status:InProgress` - Task is being worked on by developers and/or contributors.
- `Status:Blocked` - Work cannot continue without further input from someone.
- `Status:WaitingReview` - Work has been done and is waiting for review by a third party.
- `Status:Completed` - Work has been deployed to production.

## Special

- `CantReplicate` - Some issues cannot be replicated by anyone else, rendering it impossible to fix.
- `Duplicate` - The issue may have already been reported and undergoing discussion/implementation. The merged issue must be linking to the original one.
- `Invalid` - Sometimes the issue is invalid, maybe it was posted on the wrong repository or some other mistake has been done. Github does not allow us to delete issues. As such, it may be useful to mark the issue as `Invalid`, so it can be filtered out from searches.
