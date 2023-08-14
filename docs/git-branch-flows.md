git flow

```
                   +-----------------+
                   |   dev Branch   |
                   | (开发分支，特性分支) |
                   +-------+---------+
                           |
                           |
                           | 合并
                           |
                           v
                   +-----------------+
                   |   test Branch   |
                   | (测试分支，集成分支) |
                   +-------+---------+
                           |
                           |
                           | 合并
                           |
                           v
                   +-----------------+
                   | release Branch |
                   | (发布分支)       |
                   +-------+---------+
                           |
                           |
                           | 合并
                           |
                           v
                   +----------------+
                   |   main Branch  |
                   | (主分支，稳定分支) |
                   +----------------+
```

---
Sure! Here is the translation of the steps:

1. Development Phase:

   - Create a new feature branch (e.g., `feature1`) from the `dev` branch and perform development work on this branch.
   - Once the development is complete, merge the feature branch back into the `dev` branch.
   - Repeat the above steps, creating different feature branches for other features or tasks and merging them back into the `dev` branch.

1. Testing Phase:

   - Create a new `test` branch from the `dev` branch for integration testing.
   - Merge the code from the `dev` branch into the `test` branch.
   - Perform integration testing on the `test` branch to ensure compatibility between features and overall stability.
   - If any issues or errors are found, fix them and merge the fixed code back into the `test` branch.
   - Repeat the above steps until the code on the `test` branch passes integration testing.

1. Release Preparation Phase:

   - Create a new `release` branch from the `test` branch for release preparation.
   - Perform final preparations on the `release` branch, such as updating version numbers, generating release documentation, etc.
   - If any further fixes are required, make them on the `release` branch and merge the fixed code back into the `release` branch.

1. Merging to the Main Branch:

   - Once the `release` branch is ready, merge it into the `main` branch.
   - Ensure that the `main` branch is up to date and stable before the merge.
   - If any fixes were made on the `release` branch, merge the fixed code back into the `dev` branch after merging it into the `main` branch to ensure that the development branch also includes the fixes.

By following this process, you can manage and control the transition from the `dev` branch to the `test` branch, then to the `release` branch, and finally merging into the `main` branch. This ensures that stable code enters the main branch and prepares it for release versions.
