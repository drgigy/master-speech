# Master Speech

Separate admin page for controlling shared speech settings.

## Admin Login

Allowed admin email is currently:

```text
drgigy@gmail.com
```

## Saved Settings

The page saves speech settings to:

```text
admin/settings/speech
```

The clinic app can later be changed to read this central setting or, preferably, call a backend that keeps the authorization key private.

## GitHub

GitHub CLI is installed, but the saved GitHub token was invalid when this was created. Re-authenticate with:

```sh
gh auth refresh -h github.com
```

Then create and push the repo:

```sh
git init
git add .
git commit -m "Create Master Speech admin page"
gh repo create master-speech --public --source=. --remote=origin --push
```
