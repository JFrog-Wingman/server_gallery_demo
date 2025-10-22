# Available MCP Tools

This document lists all the MCP (Model Context Protocol) tools that are currently connected and available in this environment.

## Overview

The following MCP servers and tools are available for use:

## 1. GitHub MCP Server
Comprehensive GitHub integration with extensive repository management capabilities.

### Repository Management
- `github-mcp-server-get_file_contents` - Get contents of files or directories from GitHub repositories
- `github-mcp-server-list_branches` - List branches in a GitHub repository
- `github-mcp-server-list_tags` - List git tags in a GitHub repository
- `github-mcp-server-get_tag` - Get details about a specific git tag
- `github-mcp-server-get_commit` - Get details for a commit (with optional diff/stats)
- `github-mcp-server-list_commits` - Get list of commits from a branch

### Issues and Pull Requests
- `github-mcp-server-list_issues` - List issues with advanced filtering and pagination
- `github-mcp-server-get_issue` - Get details of a specific issue
- `github-mcp-server-get_issue_comments` - Get comments for a specific issue
- `github-mcp-server-list_sub_issues` - List sub-issues for a specific issue
- `github-mcp-server-list_pull_requests` - List pull requests with filtering
- `github-mcp-server-pull_request_read` - Comprehensive PR operations (get details, diff, status, files, reviews, comments)

### Search Capabilities
- `github-mcp-server-search_repositories` - Find repositories by name, description, topics, etc.
- `github-mcp-server-search_code` - Fast code search across all GitHub repositories
- `github-mcp-server-search_issues` - Search for issues using GitHub's search syntax
- `github-mcp-server-search_pull_requests` - Search for pull requests
- `github-mcp-server-search_users` - Find GitHub users by username, location, etc.

### Releases and Labels
- `github-mcp-server-list_releases` - List releases in a repository
- `github-mcp-server-get_latest_release` - Get the latest release
- `github-mcp-server-get_release_by_tag` - Get a specific release by tag
- `github-mcp-server-list_label` - List labels from repository or issue
- `github-mcp-server-get_label` - Get a specific label

### Security Scanning
- `github-mcp-server-list_code_scanning_alerts` - List code scanning alerts with filtering
- `github-mcp-server-get_code_scanning_alert` - Get details of specific code scanning alert
- `github-mcp-server-list_secret_scanning_alerts` - List secret scanning alerts
- `github-mcp-server-get_secret_scanning_alert` - Get details of specific secret scanning alert

### GitHub Actions and Workflows
- `github-mcp-server-list_workflows` - List workflows in a repository
- `github-mcp-server-list_workflow_runs` - List workflow runs with filtering
- `github-mcp-server-get_workflow_run` - Get details of a specific workflow run
- `github-mcp-server-list_workflow_jobs` - List jobs for a workflow run
- `github-mcp-server-get_job_logs` - Download logs for workflow jobs
- `github-mcp-server-get_workflow_run_logs` - Download complete workflow run logs
- `github-mcp-server-get_workflow_run_usage` - Get usage metrics for workflow runs
- `github-mcp-server-list_workflow_run_artifacts` - List artifacts for workflow runs
- `github-mcp-server-download_workflow_run_artifact` - Get download URL for artifacts
- `github-mcp-server-summarize_job_log_failures` - Analyze failed job logs
- `github-mcp-server-summarize_run_log_failures` - Analyze why workflow runs failed

### Issue Types
- `github-mcp-server-list_issue_types` - List supported issue types for organizations

## 2. JFrog Remote MCP Server
Comprehensive JFrog platform integration for artifact and package management.

### Project Management
- `jfrogremotemcpserver-create_project` - Create JFrog projects with repositories
- `jfrogremotemcpserver-list_projects` - List existing JFrog projects
- `jfrogremotemcpserver-get_project_info` - Check if specific project exists

### Repository Management
- `jfrogremotemcpserver-create_repository` - Create JFrog repositories (local, remote, virtual, federated, distribution)
- `jfrogremotemcpserver-list_repositories` - List repositories with filtering by package type, project, and type

### Package and Vulnerability Management
- `jfrogremotemcpserver-list_catalog_vulnerabilities` - Get vulnerability information by CVE ID
- `jfrogremotemcpserver-list_catalog_version_vulnerabilities` - Get vulnerabilities for specific package versions
- `jfrogremotemcpserver-list_catalog_package_versions` - List package versions with vulnerability filtering
- `jfrogremotemcpserver-get_catalog_package_entity` - Get package information (description, license, latest version)
- `jfrogremotemcpserver-get_curation_package_status` - Check curation status (approved/blocked/inconclusive)

### Artifactory Integration
- `jfrogremotemcpserver-get_rt_package_versions` - Get package versions used in organization
- `jfrogremotemcpserver-get_rt_package_version` - Get repositories where specific package version is used
- `jfrogremotemcpserver-get_artifacts_summary` - Get artifact summaries by checksum or path

### Environment Management
- `jfrogremotemcpserver-get_jfrog_global_environments` - List global JFrog environments

**Supported Package Types:** pypi, npm, maven, golang, nuget, huggingface, rubygems, bower, cargo, chef, cocoapods, composer, conan, cran, debian, docker, gems, gitlfs, go, gradle, helm, ivy, opkg, p2, pub, puppet, rpm, sbt, swift, terraform, vagrant, yum, generic

## 3. Playwright Browser Automation
Web browser automation and testing capabilities.

### Navigation and Control
- `playwright-browser_navigate` - Navigate to URLs
- `playwright-browser_navigate_back` - Go back to previous page
- `playwright-browser_close` - Close the browser
- `playwright-browser_resize` - Resize browser window
- `playwright-browser_tabs` - List, create, close, or select browser tabs

### Interaction
- `playwright-browser_click` - Perform clicks (left, right, middle, double-click)
- `playwright-browser_type` - Type text into elements
- `playwright-browser_press_key` - Press keyboard keys
- `playwright-browser_hover` - Hover over elements
- `playwright-browser_drag` - Drag and drop between elements
- `playwright-browser_select_option` - Select dropdown options

### Forms and File Handling
- `playwright-browser_fill_form` - Fill multiple form fields
- `playwright-browser_file_upload` - Upload files

### Page Analysis
- `playwright-browser_snapshot` - Capture accessibility snapshot
- `playwright-browser_take_screenshot` - Take screenshots
- `playwright-browser_evaluate` - Execute JavaScript on page/elements

### Debugging and Monitoring
- `playwright-browser_console_messages` - Get console messages
- `playwright-browser_network_requests` - Get network requests
- `playwright-browser_handle_dialog` - Handle browser dialogs
- `playwright-browser_wait_for` - Wait for conditions (text, time)

### Setup
- `playwright-browser_install` - Install browser if needed

## 4. System and Development Tools

### Terminal/Shell
- `bash` - Run Bash commands (sync/async/detached modes)
- `write_bash` - Send input to running Bash sessions
- `read_bash` - Read output from async Bash commands
- `stop_bash` - Stop running Bash commands

### File Operations
- `view` - View files and directories with line numbers
- `create` - Create new files
- `str_replace` - Make string replacements in files

### Security
- `gh-advisory-database` - Check GitHub advisory database for vulnerabilities in dependencies
- `codeql_checker` - Discover security vulnerabilities using CodeQL analysis

### Progress Reporting
- `report_progress` - Report task progress and commit changes

## 5. Custom Agents

### Available Custom Agents
- `mcp_checker` - Agent that lists connected MCP tools (used to generate this documentation)
- `my-agent` - DevSecOps agent for automated security remediation

## Summary

This environment provides comprehensive tooling for:

1. **GitHub Integration** - Complete repository management, CI/CD monitoring, security scanning
2. **JFrog Platform** - Artifact management, vulnerability scanning, package curation
3. **Browser Automation** - Full web testing and interaction capabilities
4. **Development Environment** - File editing, shell access, security scanning
5. **Security Focus** - Multiple vulnerability scanning and advisory tools

These MCP tools enable complete software development lifecycle management from code development through security scanning and deployment.

---
*This document was generated automatically by the mcp_checker agent.*