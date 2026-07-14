# @testsigma/cli

The Testsigma CLI — author, run, and push **Testsigma script** (the `code` DSL)
end-to-end tests to Testsigma Arcus & Suite.

## Install

```bash
npm install -g @testsigma/cli@beta
```

Requires **Node.js >= 22**.

## Authenticate

```bash
testsigma login      # start a login session
testsigma whoami     # show the signed-in user
testsigma logout     # clear stored credentials
```

## Author & run tests

```bash
# Print the DSL reference / examples for an app type (web | mobile | api)
testsigma code reference --type web
testsigma code examples --type web

# Validate / compile a spec without running it
testsigma code validate path/to/test.spec.ts
testsigma code compile  path/to/test.spec.ts

# Run a spec via the Testsigma agent (mobile runs in-process)
testsigma code run path/to/test.spec.ts
```

## Push to Agentic Test

```bash
# Push session-authored specs to Testsigma
testsigma code push --sprint <sprint> --module <module>
```

## Browse your workspace

```bash
testsigma projects list
testsigma sprints list
testsigma sprints issues
testsigma modules list
testsigma devices list
```

## Configuration & diagnostics

```bash
testsigma config-list        # show resolved configuration
testsigma config-use <name>  # switch active profile
testsigma auth-status        # show auth state
testsigma --version          # print the CLI version
```

Run `testsigma --help` or `testsigma <command> --help` for the full option list
on any command.

## Support

Learn more at [testsigma.com/docs](https://testsigma.com/docs).
