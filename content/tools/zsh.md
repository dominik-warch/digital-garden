---
title: Zsh
---
Als Standard auf MacOS überhaupt erst näher mit [Zsh](https://www.zsh.org/) als Shell auseinandergesetzt und anschließend überall installiert! Häufig wird in einem Atemzug noch Oh-My-Zsh als Plugin-Manager empfohlen, um Zsh überhaupt erst "nutzbar" zu machen. Als leichtgewichtigere Alternative gefällt mir [Prezto](https://github.com/sorin-ionescu/prezto) aber deutlich besser. Folgende Module sind standardmäßig geladen:

```
// .zpreztorc
# Set the Prezto modules to load (browse modules).
# The order matters.
zstyle ':prezto:load' pmodule \
  'environment' \
  'terminal' \
  'editor' \
  'history' \
  'directory' \
  'spectrum' \
  'utility' \
  'ssh' \
  'git' \
  'syntax-highlighting' \
  'completion' \
  'history-substring-search' \
  'prompt'
```
