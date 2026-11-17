# Contributing

This guide applies to every repo in the MSPGC-Demo org that doesn't have its own `CONTRIBUTING.md`. It lives in the org's `.github` repo.

## How a change gets made

1. **Start with an issue.** Every bug or request gets an issue, the same way work starts with a ticket.
2. **Create a branch for the issue.** Name it after what it does, such as `fix/zero-size-disk` or `feature/low-disk-warning`.
3. **Commit small, clear changes.** Write the message as what the commit does: "Add CSV export option", not "updates".
4. **Open a pull request.** Fill in the template, and link the issue with `Closes #123` so it closes when the PR merges.
5. **Wait for checks and a review.** Checks must pass, and someone other than the author should review.
6. **Merge, then delete the branch.**

## Rules for scripts

- Never put credentials, API keys or client data in any file. See [SECURITY.md](SECURITY.md).
- Use approved verbs (run `Get-Verb` to list them) and include comment-based help.
- Return objects, not formatted text, so output can be filtered, sorted or exported.
- Use `Write-Warning`, `Write-Verbose` or `Write-Output` instead of `Write-Host`.
