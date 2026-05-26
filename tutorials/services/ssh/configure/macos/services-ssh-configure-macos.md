[Tutorials](../../../../tutorials.md) > [Services](../../../services.md) > [SSH](../../services-ssh.md) > [Configure](../services-github-configure.md) > macOS

# Services GitHub Configure macOS

## Configure

### Checking for existing SSH keys

```bash
ls -al ~/.ssh
```

### Generating a new SSH key

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

### Adding your SSH key to the ssh-agent

```bash
eval "$(ssh-agent -s)"
ssh-add --apple-use-keychain ~/.ssh/id_ed25519
```

### Adding a new SSH key to your account

```bash
pbcopy < ~/.ssh/id_ed25519.pub
```
