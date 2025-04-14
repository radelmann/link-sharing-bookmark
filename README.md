# Universal Link Sharer Bookmarklet

This bookmarklet copies a clean, Markdown-formatted link to your clipboard based on the current page you're viewing. It's optimized for Jira tickets, GitHub PRs (including Adobe's internal GHE), and any general webpage.

## Features

- ✅ **Jira**: Copies `[TICKET-123 - Ticket Title](https://...)`
- ✅ **GitHub PRs** (public or Adobe GHE): Copies `[Fix title - org/repo#123](https://...)`
- ✅ **Any other webpage**: Copies `[Page Title](https://...)`
- ✅ Uses the native clipboard API with a fallback for broader compatibility
- ✅ Shows a toast notification on success or error

## Installation

1. Create a new bookmark in your browser
2. Set the name to something like `Copy Markdown Link`
3. Paste the **minified JavaScript** as the URL (see code.js.min)

## Usage

- While viewing a page (Jira ticket, GitHub PR, or any web page), click the bookmark
- The Markdown link will be copied to your clipboard
- You'll see a small toast notification confirming the copy

## Example Output

For different types of pages, the bookmarklet will generate the following formats:

### Jira Ticket
```
[PROJ-123 - Implement new feature for user authentication](https://jira.example.com/browse/PROJ-123)
```

### GitHub PR (Public or Adobe GHE)
```
[Add dark mode support - org/repo#456](https://github.com/org/repo/pull/456)
```

### General Webpage
```
[Example Page Title](https://example.com/page)
```

The bookmarklet will show a small toast notification in the top-right corner when the link is successfully copied to your clipboard.

