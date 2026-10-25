# Contributing

Thanks for taking the time to look at this project. Bug reports, questions and pull requests are all welcome.

## Before you start

- Search existing issues first; someone may already be on it.
- For anything larger than a small fix, open an issue describing the change so we can agree on the approach before you write code.

## Development workflow

1. Fork the repository and create a branch from `main` (`feat/...`, `fix/...`, `docs/...`).
2. Follow the Quick Start in the repository's README to get it running locally. Every project has a `.env.example`, a Dockerfile and, where it needs a database, a `docker-compose.yml`.
3. Make your change with tests. Each repository's README has a **Testing** section with the exact commands.
4. Run the same checks CI runs before pushing:
   - Python projects: `ruff check .`, `ruff format --check .`, `pytest`
   - TypeScript projects: `npm run lint`, `npm test`, `npm run build`
   - Go projects: `go vet ./...`, `go test -race ./...`
5. Open a pull request against `main` and fill in the template.

## Commit messages

Commits follow [Conventional Commits](https://www.conventionalcommits.org/): `feat:`, `fix:`, `perf:`, `refactor:`, `test:`, `docs:`, `ci:`, `chore:`. Keep the subject under about 72 characters and explain the *why* in the body when it isn't obvious.

## Code style

- Match the existing structure and naming in the project.
- No secrets or real credentials in code, tests or fixtures; the sandbox adapters exist for that.
- Money is handled in minor units or `Decimal`, never floats.
- Time-dependent logic takes an injectable clock so tests don't depend on the real date.

## License

By contributing you agree that your contributions are licensed under the repository's MIT license.
