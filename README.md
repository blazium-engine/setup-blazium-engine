# Blazium Setup Action

Reusable Action that downloads and installs the Blazium Engine or the Blazium Templates. Example usage:

```yml
- uses: blazium-engine/setup-blazium-engine@master
  name: 🤖 Setup Blazium
  with:
    version: 0.3.74-nightly
    download_template: true # if true, downloads templates
    platform: linux # eg. linux, macos, windows

- name: 🔬 Verify Setup
  run: |
    Blazium --version
    $BLAZIUM_EDITOR --version
    ls $BLAZIUM_TEMPLATE
```
