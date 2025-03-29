# Blazium Setup Engine Action

Reusable Action that downloads and installs the Blazium Engine or the Blazium Templates. Example usage:

```yml
- uses: blazium-engine/setup-blazium-engine@master
  name: 🤖 Setup Blazium
  with:
    version: 0.3.74-nightly
    download_template: true # if true, downloads templates
    platform: linux # eg. linux, macos, windows

- name: 🔬 Verify Engine
  run: |
    Blazium --version
```

Get latest:

```yml
- uses: blazium-engine/setup-blazium-engine@master
  name: 🤖 Setup Blazium
  with:
    version: latest
```

Get latest with specific version major:

```yml
- uses: blazium-engine/setup-blazium-engine@master
  name: 🤖 Setup Blazium
  with:
    version: latest-0.4
```
