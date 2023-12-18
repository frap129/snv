# snv (Switch eNVironment)
`snv` is a script that lets you choose a shell environment from a list of your distrobox containers + your host.

If `snv` is installed somewhere in your home directory and is in your path, it works both on host and in a container.

### Preview
The command used to generate the preview is customizable using environment variables.
| Variable     | Default Value                                                  |
|--------------|----------------------------------------------------------------|
| HOST_PREVIEW | `cat /etc/hostname`                                            |
| ENV_PREVIEW  | `distrobox list \| head -n 1 && distrobox list \| grep ' {}'"` |

As an example, to generate a simple preview for the host with neofetch, export

`HOST_PREVIEW="neofetch --backend off --color_blocks off"`

Dependencies:
- distrobox
- fzf

