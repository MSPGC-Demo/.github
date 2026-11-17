# Security

This policy applies to every repo in the MSPGC-Demo org that doesn't have its own `SECURITY.md`.

## Secrets

Never commit passwords, API keys, tokens, certificates or client data. Scripts should read secrets at run time from your RMM's secure variables, a secrets vault, or GitHub Actions secrets.

## If a secret gets committed

1. **Rotate it immediately.** Treat it as leaked the moment it's pushed. Removing it from the file or rewriting history does not make it safe again, because clones and forks may already have it.
2. Remove it from the code and replace it with a secure lookup.
3. Tell the repo maintainers so they can check where else it was used.

## Reporting a vulnerability

If you find a security problem in one of these scripts, don't open a public issue. Contact the maintainers privately instead.
