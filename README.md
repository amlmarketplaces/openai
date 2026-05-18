# amlmarketplaces/openai

Claude Code marketplace federating all `@amlplugins/openai-*` plugins.

## Install

Add to your project's `.claude/settings.json`:

```json
{
  "extraKnownMarketplaces": {
    "aml-openai": {
      "source": { "source": "github", "repo": "amlmarketplaces/openai" }
    }
  },
  "enabledPlugins": {
      "openai-assistants@aml-openai": true,
      "openai-audio@aml-openai": true,
      "openai-batch@aml-openai": true,
      "openai-chat@aml-openai": true,
      "openai-embeddings@aml-openai": true
    }
}
```

Then launch Claude Code in the project. The marketplace is fetched from `amlmarketplaces/openai`, cached under `~/.claude/plugins/cache/aml-openai/`, and each enabled plugin is loaded from its `amlplugins` source repo.

## Plugins (10 total)

- `openai-assistants` — [@amlplugins/openai-assistants](https://github.com/amlplugins/openai-assistants)
- `openai-audio` — [@amlplugins/openai-audio](https://github.com/amlplugins/openai-audio)
- `openai-batch` — [@amlplugins/openai-batch](https://github.com/amlplugins/openai-batch)
- `openai-chat` — [@amlplugins/openai-chat](https://github.com/amlplugins/openai-chat)
- `openai-embeddings` — [@amlplugins/openai-embeddings](https://github.com/amlplugins/openai-embeddings)
- `openai-files` — [@amlplugins/openai-files](https://github.com/amlplugins/openai-files)
- `openai-fine-tuning` — [@amlplugins/openai-fine-tuning](https://github.com/amlplugins/openai-fine-tuning)
- `openai-images` — [@amlplugins/openai-images](https://github.com/amlplugins/openai-images)
- `openai-moderations` — [@amlplugins/openai-moderations](https://github.com/amlplugins/openai-moderations)
- `openai-responses` — [@amlplugins/openai-responses](https://github.com/amlplugins/openai-responses)

## Related

- npm packages: `@amlplugins/openai-*` published to GitHub Packages (`https://npm.pkg.github.com`).
- Aggregating parent: [`amlmarketplaces/aml`](https://github.com/amlmarketplaces/aml) — federates every `@amlplugins/*` plugin under a single marketplace.
- AML topology: see `.claude/rules/definitions/ageni.md` § "GitHub Topology" — this repository is a Tier-4 HUB-INSTANCE under the `amlmarketplaces/` Tier-3 HUB-ORGANIZATION.

> Built by `.claude/skills/aml/metateam/marketplace/test/cross-org-amlmarketplaces-batch.mjs`.
