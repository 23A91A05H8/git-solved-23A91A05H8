# My Git Mastery Challenge Journey

## Student Information
- Name: Likhitha Palisetti
- Student ID: 23A91A05H8
- Repository: https://github.com/23A91A05H8/git-mastery-challenge-template.git

- Date Started: 27-10-2025
- Date Completed: 28-10-2025

## Task Summary
Cloned instructor's repository with pre-built conflicts and resolved all 
merge conflicts across multiple branches using proper Git workflows.

## Commands Used

| Command | Times Used | Purpose |
|---------|------------|----------|
| git clone | 1 | Clone instructor's repository |
| git checkout | 20+ | Switch between branches |
| git branch | 10+ | View and manage branches |
| git merge | 2 | Merge dev and conflict-simulator into main |
| git add | 30+ | Stage resolved conflicts |
| git commit | 15+ | Commit resolved changes |
| git push | 10+ | Push to my repository |
| git fetch | 2 | Fetch updates from instructor |
| git pull | 1 | Pull updates |
| git stash | 2 | Save temporary work |
| git cherry-pick | 1 | Copy specific commit |
| git rebase | 1 | Rebase feature branch |
| git reset | 3 | Undo commits (soft/mixed/hard) |
| git revert | 1 | Safe undo |
| git tag | 2 | Create release tags |
| git status | 50+ | Check repository state |
| git log | 30+ | View history |
| git diff | 20+ | Compare changes |

## Conflicts Resolved

### Merge 1: main + dev (6 files)

#### Conflict 1: config/app-config.yaml
- **Issue**: Production used port 8080, development used 3000
- **Resolution**: Created unified config with environment-based settings
- **Strategy**: Keep production as default, add dev as optional
- **Difficulty**: Medium
- **Time**: 15 minutes

#### Conflict 2: config/database-config.json
- **Issue**: Different database hosts and SSL modes
- **Resolution**: Created separate profiles for production and development
- **Strategy**: Restructured JSON to support both environments
- **Difficulty**: Medium
- **Time**: 10 minutes

#### Conflict 3: scripts/deploy.sh
- **Issue**: Different deployment strategies (production vs docker-compose)
- **Resolution**: Added conditional logic based on DEPLOY_ENV variable
- **Strategy**: Made script handle both environments dynamically
- **Difficulty**: Hard
- **Time**: 20 minutes

#### Conflict 4: scripts/monitor.js
- **Issue**: Different monitoring intervals and log formats
- **Resolution**: Environment-based configuration object
- **Strategy**: Used process.env.NODE_ENV to determine behavior
- **Difficulty**: Medium
- **Time**: 15 minutes

#### Conflict 5: docs/architecture.md
- **Issue**: Different architectural descriptions
- **Resolution**: Merged both descriptions into comprehensive document
- **Strategy**: Created sections for each environment
- **Difficulty**: Easy
- **Time**: 10 minutes

#### Conflict 6: README.md
- **Issue**: Different feature lists and version numbers
- **Resolution**: Combined all features with clear environment labels
- **Strategy**: Organized features by category
- **Difficulty**: Easy
- **Time**: 10 minutes

### Merge 2: main + conflict-simulator (6 files)

### Conflict Set 2 (Merge: main ← conflict-simulator)

### Conflict #1 (main ← conflict-simulator)
**File:** conflict.txt  
**Issue:** Both branches added different content in the same lines.  
**Resolution:** Combined both changes to preserve details.  
**Strategy:** Mixed resolution (took parts from both sides).  
**Commit:** 0f1ad03  


#### Conflict #2: README.md
- **Issue:** Different descriptions of the project purpose.
- **Resolution:** Combined both descriptions to make the README more complete.
- **Strategy:** Mixed resolution (kept content from both branches).
- **Commit:** 1a27a60

#### Conflict #3: docs/architecture.md
- **Issue:** Different architectural diagrams and environment descriptions.
- **Resolution:** Created a unified architecture explanation referencing both parts.
- **Strategy:** Merge + reorganize content.
- **Commit:** 479c163

#### Conflict #4: scripts/deploy.sh
- **Issue:** Two different deployment methods (manual vs automated).
- **Resolution:** Kept automated method but added manual mode as fallback.
- **Strategy:** Integrated both approaches for flexibility.
- **Commit:** 479c163

#### Conflict #5: package.json
- **Issue:** Version numbers and dependencies conflict between branches.
- **Resolution:** Updated to latest version and included all necessary dependencies.
- **Strategy:** Chose newer dependency set.
- **Commit:** 02011a5

#### Conflict #6: .env.example
- **Issue:** Different environment variable naming conventions.
- **Resolution:** Standardized names to consistent uppercase snake_case.
- **Strategy:** Normalize naming across environments.
- **Commit:** (No dedicated commit; changes merged as part of merge resolution)


