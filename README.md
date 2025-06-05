# Tags Automation

This repository contains a GitHub Actions workflow that automates tag creation:

- For non-main branches: Automatically creates tags with branch name and timestamp
- For main branch: Requires manual tag name input

## Usage

1. For regular branches:
   - Just push to any branch, and it will automatically create a tag
   - Example: Pushing to `feature-branch` will create a tag like `feature-branch-20240315123456`

2. For main branch:
   - Provide a tag name when pushing
   - Use GitHub UI or CLI to specify the tag name
   - Example: `gh workflow run tag-creation.yml -f tag_name=v1.0.0`

## Testing
This README was updated to test the main branch workflow. 