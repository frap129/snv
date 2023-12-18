# snv (Switch eNVironment)
`snv` is a script that lets you choose a shell environment from a list of your distrobox containers + your host.

If `snv` is installed somewhere in your home directory and is in your path, it works both on host and in a container.

### Preview
The preview section of the host is customizeable. It defaults to `cat /etc/hostname`, and setting the `SNV_FETCH`
environment variable will change what command is used. For example, to generate a simple preview with neofetch, export

`SNV_FETCH="neofetch --backend off --color_blocks off"`

Dependencies:
- distrobox
- fzf

