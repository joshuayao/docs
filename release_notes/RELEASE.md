# Releasing OPEA

## Release Cadance

The following release candance is for year 2024/2025. Please note that the dates listed below may not reflect the most up-to-date information

| Version | Feature/Dockerfile Freeze | Code/Doc Freeze | Release Date |
| --- | --- | --- | --- |
| 0.6 | WW20 2024 | WW21 2024 | WW22 2024 |
| 0.7 | WW24 2024 | WW25 2024 | WW26 2024 |
| 0.8 | WW29 2024 | WW30 2024 | WW31 2024 |
| 0.9 | WW33 2024 | WW34 2024 | WW35 2024 |
| 1.0 | WW36 2024 | WW37 2024 | WW38 2024 |
| 1.1 | WW45 2024 | WW46 2024 | WW47 2024 |
| 1.2 | WW02 2025 | WW03 2025 | WW04 2025 |
| 1.3 | Mar 2025 | Mar 2025 | Mar 2025 |
| 1.4 | May 2025 | May 2025 | May 2025 |
| 1.5 | July 2025 | July 2025 | July 2025 |
| 1.6 | Sep 2025 | Sep 2025 | Sep 2025 |
| 1.7 | Nov 2025 | Nov 2025 | Nov 2025 |

## General Overview

Releasing a new version of OPEA generally involves the following key steps:

1. Feature/Dockerfile Freeze (2 weeks before the release)
2. Code/Doc Freeze, and Creating the RC(Release Candidate) Branch (1 week before the release)
3. Merging Cherry Picks to the RC Branch
4. Creating Tag from RC Branch

## Feature/Dockerfile Freeze

Generally, this marks a point in the OPEA release process where no new features or Dockerfile updates are added to the `main` branch of OPEA projects. It typically occurs two weeks before the scheduled OPEA release.

## Code/Doc Freeze, and Creating the RC Branch

This is the point in the OPEA release process where no code changes or document changes are updated to the `main` branch of OPEA projects. It typically occurs one week before the scheduled OPEA release.

### Preparing Creating RC Branch
Following requirements needs to be met prior to creating the RC branch:
- Implement all features and functionalities targeting this release.
- Resolve all the known outstanding issues targeting this release.
- Validation?? TODO

### Creating RC Branch
The RC branch are typically created from the `main` branch. The branch name must follow the following format: 
```
v{MAJOR}.{MINOR}rc
```
An example of this would look like:
```
v1.1rc
```

## Merging Cherry Picks to the RC Branch
Fixes typically are necessary for bugs and regressions after code freeze. 

### How to do Cherry Picking
TODO

### Cherry Picking Reverts
TODO

## Creating Tag from RC Branch
The following requirements need to be met prior to creating final Release Candidate:
- No outstanding issues in the milestone. No open issues/PRs whose has the milestone of this release(e.g. v1.1).
- All the closed milestone PRs should be present in the release branch.

You can use the following commands to create release tag.
TODO


