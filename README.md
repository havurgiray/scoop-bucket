# havurgiray/scoop-bucket

[Scoop](https://scoop.sh) bucket for [agent-history-tether (aht)](https://github.com/havurgiray/agent-history-tether).

```powershell
scoop bucket add havurgiray https://github.com/havurgiray/scoop-bucket
scoop install aht
aht install --here    # logon watcher + Claude Code hook, referencing scoop's exe
aht adopt --apply     # tether this machine's existing projects
```

Both x64 and ARM64 builds are provided. The exes are unsigned, so
SmartScreen may show "unknown publisher" on first run (More info > Run
anyway). After `scoop update aht`, run `aht install --here` again so the
watcher and hook use the new exe. `aht uninstall` removes the automation
(no agent's history is ever touched); then `scoop uninstall aht`.
