# Bash

## Configuration

Make root use `/etc/skel/.bashrc` (colors)

```bash
cp /etc/skel/.bashrc ~
source ~/.bashrc
```

## Utils

Read markdown from stdin and run the bash parts
```bash
awk '/```/{f=0}f;/^```bash/{f=1}' | bash -xe
```

