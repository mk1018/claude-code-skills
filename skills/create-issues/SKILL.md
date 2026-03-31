---
name: create-issues
description: 指示されたタスクからGitHub Issuesを作成する
---

# Create Issues

Create GitHub Issues from instructed tasks.

## Repository

- org: nerochain
- repository: nero-line-points
- github projects: https://github.com/orgs/nerochain/projects/2/views/1

## Steps

1. **Confirm Tasks**
   - Confirm task content instructed by user
   - If there are multiple tasks, create separate Issues for each

2. **Create Issue**
   - Create Issue with the following command:

     ```bash
     gh issue create --repo nerochain/nero-line-points --title "Title" --body "Description"
     ```

   - Issue body should include:
     - Task overview
     - Detailed description or acceptance criteria as needed
     - If specific code lines are mentioned, include a link to the code:
       - Format: `https://github.com/nerochain/nero-line-points/blob/{commit-hash}/{file-path}#L{start}-L{end}`
       - Example: `https://github.com/nerochain/nero-line-points/blob/ec160609/lib/constants/map_tile_urls.dart#L5-L23`

   - Always link the issue to Project after creation
     - Command: `gh project item-add 1 --owner nerochain --url <issue-url>`
3. **Completion Report**
   - Display list of created Issue URLs

## Notes

- Name titles to be concise and clearly indicate the content
- Check if similar Issues already exist
- Use `--label` or `--assignee` options if labels or assignments are needed
- **Write Issue titles and content in Japanese**
