# WSL

## Configuration

Show WSL distro name instead of hostname in prompt

```bash
sed -ri 's/(PS1.*)\\h/\1$WSL_DISTRO_NAME/' /etc/skel/.bashrc
```

## Utils

Convert Windows output
```bash
wsl.exe -l | iconv -c -f utf16 -t utf8 | tr -d '\r'
```

