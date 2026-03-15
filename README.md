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

---

## Disclaimer

**NO WARRANTY.** THERE IS NO WARRANTY FOR THE PROGRAM, TO THE EXTENT PERMITTED BY APPLICABLE LAW. EXCEPT WHEN OTHERWISE STATED IN WRITING THE COPYRIGHT HOLDERS AND/OR OTHER PARTIES PROVIDE THE PROGRAM "AS IS" WITHOUT WARRANTY OF ANY KIND, EITHER EXPRESSED OR IMPLIED, INCLUDING, BUT NOT LIMITED TO, THE IMPLIED WARRANTIES OF MERCHANTABILITY AND FITNESS FOR A PARTICULAR PURPOSE. THE ENTIRE RISK AS TO THE QUALITY AND PERFORMANCE OF THE PROGRAM IS WITH YOU. SHOULD THE PROGRAM PROVE DEFECTIVE, YOU ASSUME THE COST OF ALL NECESSARY SERVICING, REPAIR OR CORRECTION.

**Limitation of Liability.** IN NO EVENT UNLESS REQUIRED BY APPLICABLE LAW OR AGREED TO IN WRITING WILL ANY COPYRIGHT HOLDER, OR ANY OTHER PARTY WHO MODIFIES AND/OR CONVEYS THE PROGRAM AS PERMITTED ABOVE, BE LIABLE TO YOU FOR DAMAGES, INCLUDING ANY GENERAL, SPECIAL, INCIDENTAL OR CONSEQUENTIAL DAMAGES ARISING OUT OF THE USE OR INABILITY TO USE THE PROGRAM (INCLUDING BUT NOT LIMITED TO LOSS OF DATA OR DATA BEING RENDERED INACCURATE OR LOSSES SUSTAINED BY YOU OR THIRD PARTIES OR A FAILURE OF THE PROGRAM TO OPERATE WITH ANY OTHER PROGRAMS), EVEN IF SUCH HOLDER OR OTHER PARTY HAS BEEN ADVISED OF THE POSSIBILITY OF SUCH DAMAGES.
