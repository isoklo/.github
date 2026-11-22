<p align="center">
  <img src="https://raw.githubusercontent.com/isoklo/.github/main/assets/isoklo-banner.svg" alt="Isoklo: deterministic proof before merge for AI coding agents. An agent pull request passes unit tests, the Isoklo gate blocks it, and the branch ruleset blocks the merge." width="100%">
</p>

**Isoklo is a deterministic merge gate for AI-written pull requests.** It blocks a change, with the exact line as
evidence, when it weakens tests, invents a package, leaks a secret, or widens what agents and CI may do. No model is
asked for an opinion: the same change always gets the same verdict.

| Repository | What it is |
|---|---|
| **[isoklo](https://github.com/isoklo/isoklo)** · `v0.2.0` | The CLI, the GitHub Action and the GitHub App: 62 rules, no runtime dependencies. [npm](https://www.npmjs.com/package/isoklo) · [GitHub Marketplace](https://github.com/marketplace/actions/isoklo) |
| **[isoklo-demo](https://github.com/isoklo/isoklo-demo)** | Four live agent pull requests. Unit tests pass on all four; Isoklo blocks three. |
| **[isoklo-web](https://github.com/isoklo/isoklo-web)** | The interactive showcase at [isoklo.vercel.app](https://isoklo.vercel.app). |

```console
npx isoklo           # scan this repository, no setup
npx isoklo init      # add it to every pull request: hook, CI and a baseline
npx isoklo check     # check this branch before it merges
```

Try it in your browser first: [euklo.com/check](https://euklo.com/check/). Every rule: [euklo.com/isoklo](https://euklo.com/isoklo/).

Built by [Euklo](https://euklo.com), a developer-focused AI agent and LLM tooling studio.
