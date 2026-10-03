# tmux-conf

## Plugins

TPM only needs one manual clone. After that it pulls the rest into `~/.tmux/plugins/`.

**1. Clone the plugin manager (once):**

```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
```

**2. Start tmux and install the plugins listed in `~/.tmux.conf`:**

Inside tmux, press `Ctrl-p` then `Shift-I` (capital i).

TPM then clones these into `~/.tmux/plugins/`:

| Plugin | GitHub | Local path |
|---|---|---|
| tpm | https://github.com/tmux-plugins/tpm | `~/.tmux/plugins/tpm` |
| tmux-resurrect | https://github.com/tmux-plugins/tmux-resurrect | `~/.tmux/plugins/tmux-resurrect` |
| tmux-continuum | https://github.com/tmux-plugins/tmux-continuum | `~/.tmux/plugins/tmux-continuum` |

Your prefix is `C-p`, so the install shortcut is `Ctrl-p` `I`, not the default `Ctrl-b` `I`.

If you want to clone them yourself instead of using that shortcut:

```bash
git clone https://github.com/tmux-plugins/tpm ~/.tmux/plugins/tpm
git clone https://github.com/tmux-plugins/tmux-resurrect ~/.tmux/plugins/tmux-resurrect
git clone https://github.com/tmux-plugins/tmux-continuum ~/.tmux/plugins/tmux-continuum
```

Then reload the config:

```bash
tmux source-file ~/.tmux.conf
```
