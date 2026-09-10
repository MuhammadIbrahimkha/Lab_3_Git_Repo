# Lab 3: Python Configuration Merge Conflict

## Goal
Practice Git merge conflicts using Python and Bash.

## Your task
1. Create branch `feature-staging`.
2. Change the target environment in `config.py` to `staging`.
3. Commit the change.

Then create/switch to another branch from the original main:
4. Create branch `feature-production`.
5. Change the same configuration value to `production`.
6. Commit the change.

7. Merge one branch into the other.
8. Resolve the conflict manually.
9. Run `python3 config.py`.
10. Run `./deploy.sh`.
11. Commit the conflict resolution.
12. Push the result to GitHub.

## Deliverable
Document in this README which version you selected and why.

## Conflict Resolution

A merge conflict occurred in `config.py` because both `feature-staging` and `feature-production` modified the same `ENVIRONMENT` configuration line.

The `production` version was selected because the final configuration represents the production deployment target. The conflict was resolved manually by removing the Git conflict markers and keeping the production value.

After resolving the conflict, `python3 config.py` and `./deploy.sh` were executed successfully.
