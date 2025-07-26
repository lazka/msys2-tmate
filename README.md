# MSYS2 on GitHub Actions

Simple workflow to get SSH access to MSYS2 on GitHub Actions runners using [action-tmate](https://github.com/mxschmitt/action-tmate).

## Usage

1. **[Click here to start a workflow](../../actions/workflows/start.yml)** (or go
   to Actions → main → Run workflow)
2. Select your desired runner image, MSYS2 environment, and additional packages
   to install
3. Click "Run workflow"
4. Wait for the SSH connection information to appear in the logs
5. Connect using the provided SSH command

## Requirements

You need to have an SSH public key registered on your GitHub account. Check if
you have one at:
```
https://github.com/<your-username>.keys
```

If empty, [add an SSH key to your GitHub
account](https://github.com/settings/keys) first.

## Switching Shells

Once connected, you can switch between MSYS2 environments:

```bash
. shell clang64
```
