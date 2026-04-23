# Vincy Global Plugin

## Purpose

The Vincy global plugin lets Vince invoke SecondMe from outside the `~/SecondMe` repository.

When Vince says `Vincy` in any Codex workspace, Codex should load the global Vincy skill, then use `/Users/vince/SecondMe` as SecondMe's operating home.

## Installed Location

- Plugin root: `/Users/vince/.codex/plugins/vincy`
- Manifest: `/Users/vince/.codex/plugins/vincy/.codex-plugin/plugin.json`
- Skill: `/Users/vince/.codex/plugins/vincy/skills/vincy/SKILL.md`
- Local marketplace: `/Users/vince/.codex/.agents/plugins/marketplace.json`
- Codex config: `/Users/vince/.codex/config.toml`
- Config backup: `/Users/vince/.codex/config.toml.before-vincy`

## Activation

Use:

```text
Vincy, 按 SecondMe 流程处理这个任务。
```

Expected behavior:

1. Codex recognizes the Vincy skill.
2. Codex enters SecondMe mode.
3. Codex reads only the necessary files from `/Users/vince/SecondMe`.
4. Codex acts through the CEO office by default.
5. Codex respects the permission boundaries in `00-governance/permission-boundaries.md`.

## Permission Boundary

The plugin only defines behavior and routing. It does not grant automatic permission to:

- operate the computer
- send external messages
- delete or overwrite important content
- change permission rules
- change core agent identity

Those actions still require explicit approval from Vince.

## Troubleshooting

If `Vincy` does not work outside `~/SecondMe`:

1. Restart Codex so it reloads local plugins and config.
2. Confirm `/Users/vince/.codex/config.toml` contains `vincy@vince-local`.
3. Confirm `/Users/vince/.codex/plugins/vincy/skills/vincy/SKILL.md` exists.
4. Reinstall the plugin from the files in this document if needed.

