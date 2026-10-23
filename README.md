# ci-cd-lab

Small Express 5 app (ES Modules, Node 24, Yarn 4) with a GitHub Actions CI pipeline that runs ESLint, Mocha tests and c8 coverage.

## Commands

```bash
yarn install    # install dependencies
yarn start      # run the server on http://localhost:3000
yarn lint       # ESLint
yarn test       # Mocha + Chai + Supertest
yarn coverage   # c8 coverage report (coverage/index.html)
```

## CI

`.github/workflows/ci.yml` runs on pushes and pull requests to `main`, and uploads the HTML coverage report as the `code-coverage-report` artifact.
