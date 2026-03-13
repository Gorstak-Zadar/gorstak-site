# Gorstak site

Static site for [gorstak.eu](https://gorstak.eu). Projects are loaded **dynamically** from GitHub.

## Config: `repos.json`

Edit `repos.json` to control which repos appear—no code changes needed.

| Field | Description |
|-------|-------------|
| **users** | Array of GitHub usernames. Repos from all listed users are fetched and merged. Example: `["Gorstak-Zadar", "OtherUser"]`. |
| **onlyRepos** | Optional. If set, only these repos are shown (e.g. `["Gorstak-Zadar/GEDR", "Gorstak-Zadar/GSecurity"]`). Use `null` to show all repos from `users`. |
| **excludeRepos** | Optional. Full names of repos to hide (e.g. `["Gorstak-Zadar/private-repo"]`). Use `null` for no exclusions. |

**Examples**

- Add another GitHub user: add their username to `users`.
- Show only selected projects: set `onlyRepos` to an array of `"owner/repo"` strings.
- Hide a few repos: set `excludeRepos` to an array of `"owner/repo"` strings.

If `repos.json` is missing or invalid, the site falls back to `users: ["Gorstak-Zadar"]` and shows all non-fork repos.
