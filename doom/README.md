# Doom Emacs configuration

This directory is the version-controlled Doom user configuration (`$DOOMDIR`).

The enabled modules cover Treemacs, Docker, LSP, LLM integration, Terraform,
Go, JavaScript/TypeScript, Python, and web/Vue files. The `web` module ensures
that `.vue` files use `web-mode`, including normal line-number behavior.

## Apply

Back up an existing Doom user configuration before linking this directory:

```sh
mv ~/.config/doom ~/.config/doom.backup
ln -s "$(pwd)/doom" ~/.config/doom
~/.config/emacs/bin/doom sync
```

Then restart the Emacs daemon. The `ep` shell function will start it again on
the next invocation.

For gptel/OpenAI integration, expose the key outside this repository:

```sh
export OPENAI_API_KEY="..."
```
