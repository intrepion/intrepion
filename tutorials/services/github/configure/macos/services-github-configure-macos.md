[Tutorials](../../../../tutorials.md) > [Services](../../../services.md) > [GitHub](../../services-github.md) > [Configure](../services-github-configure.md) > macOS

# Services GitHub Configure macOS

## Configure

### Connecting to GitHub with SSH

#### Checking for existing SSH keys

```bash
ls -al ~/.ssh
```

#### Generating a new SSH key

```bash
ssh-keygen -t ed25519 -C "your_email@example.com"
```

#### Adding your SSH key to the ssh-agent

```bash
eval "$(ssh-agent -s)"
ssh-add --apple-use-keychain ~/.ssh/id_ed25519
```

#### Adding a new SSH key to your account

```bash
pbcopy < ~/.ssh/id_ed25519.pub
```

1. In the upper-right corner of any page on GitHub, click your profile picture, then click  Settings.
1. In the "Access" section of the sidebar, click  SSH and GPG keys.
1. Click New SSH key or Add SSH key.
1. In the "Title" field, add a descriptive label for the new key. For example, if you're using a personal laptop, you might call this key "Personal laptop".
1. Select the type of key, either authentication or signing. For more information about commit signing, see About commit signature verification.
1. In the "Key" field, paste your public key.
1. Click Add SSH key.
1. If prompted, confirm access to your account on GitHub. For more information, see Sudo mode.
