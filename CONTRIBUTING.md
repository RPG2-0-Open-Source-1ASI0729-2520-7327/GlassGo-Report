# Contributing Guidelines – RPG-Report
This document defines the collaboration rules for all members of the **RPG2.0 Startup** working on the GlassGo Project report.

## Branching Model – GitFlow
- **main** → Contains only stable, officially delivered versions.
- **develop** → Integration branch for ongoing work.
- **feature/** → Branches for each chapter or subsection.
- **release/** → Used when preparing deliverables (TB1, TP1, TB2, TF1).

## Commit Convention
We use [Conventional Commits](https://www.conventionalcommits.org/en/v1.0.0/):
- `feat:` → New content or section added.
- `docs:` → Documentation updates (README, guidelines, minor edits).
- `fix:` → Corrections (typos, formatting, references).
- `chore:` → Maintenance tasks (restructuring, renaming files, .gitignore).

**Examples:**
- `feat: add Lean UX Canvas to Chapter 1`
- `docs: update table of contents`
- `fix: correct figure reference in Chapter 2`
- `chore: reorganize images folders`

## Contribution Process
1. **Update your local repo**
   ```bash
   git checkout develop
   git pull origin develop
   ```

2. **Create a new feature branch**
   ```bash
   git checkout -b feature/chX-section-name
   git push -u origin feature/chX-section-name
   ```

3. **Make commits frequently** following commit conventions.

4. **Push changes to GitHub**
   ```bash
   git push
   ```

5. **Open a Pull Request (PR)**
   - PRs go to `develop`.
   - At least one peer review before merge.

6. **Merging to main**
   - Only from a `release/*` branch.
   - Managed by the team leader.

## File Organization
- All report content must go inside `docs/` in Markdown format.
- Images and diagrams must be stored in `src/images/chapterN` or `src/diagrams/`.
- Each figure in the report must reference files from `src/`.
- Official PDFs go into `versions/`.

## Reviews & Collaboration
- Each PR must have a clear description of what was added or fixed.
- No direct commits to `main` or `develop`.
- Use English for branch names, commit messages and filenames.
