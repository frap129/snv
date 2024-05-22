# snv (Switch eNVironment)
`snv` is a script that lets you choose a shell environment from a list of your distrobox containers + your host.

If `snv` is installed somewhere in your home directory and is in your path, it works both on host and in a container.

![](docs/demo.gif)

### Preview
The command used to generate the preview is customizable using environment variables.
| Variable  | Default Value                                                  |
|-----------|----------------------------------------------------------------|
| HOST_PREV | `cat /etc/hostname`                                            |
| ENV_PREV  | `distrobox list \| head -n 1 && distrobox list \| grep ' {}'"` |

As an example, to generate a simple preview for the host with neofetch, export

`HOST_PREV="neofetch --backend off --color_blocks off"`

Dependencies:
- distrobox
- fzf

### Setup completions
Completions for BASH and ZSH are included in `snv`. Simply `source ~/.local/bin/snv` (or whatever path you installed it to) in your `~/.bashrc` or `~/.zshrc` respevtively
