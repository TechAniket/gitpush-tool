# GitPush Generator 🚀

> Stop fighting git errors. Generate a custom push script for any GitHub repo in 10 seconds.

**Live Demo:** https://techaniket.github.io/gitpush-tool/

---

## What is this?

A free web tool that generates a custom `push.bat` / `push.sh` / `push.ps1` script for any GitHub repository.  
Paste it in your project folder, double-click, and your code is on GitHub — no errors.

## What errors does it fix?

| Error | How |
|---|---|
| `remote origin already exists` | Auto-detects and uses `set-url` instead of `add` |
| `not a git repository` | Auto-runs `git init` if `.git` missing |
| `src refspec main does not match` | Ensures commit exists before push |
| Secrets accidentally pushed | Scans staged files for `.env`, tokens, keys |
| Merge conflicts on push | Auto `pull --rebase` before push |
| `bash not found` on Windows | Generates native `.bat` for Windows |

## Features

- Windows `.bat`, macOS/Linux `.sh`, PowerShell `.ps1`
- Auto git init, remote setup, branch switch
- .gitignore auto-creation (Python, Node, secrets)
- Secrets scanner — blocks `.env` / tokens from being pushed
- Optional: git tag release, open repo in browser after push, force push
- Per-repo git user config
- SEO optimized, 100% client-side (no data sent anywhere)

## Tech Stack

Pure HTML + CSS + Vanilla JS. Zero dependencies. Zero frameworks.  
Deploy anywhere — GitHub Pages, Netlify, Vercel, Cloudflare Pages.

## Deploy Your Own

```bash
# Fork this repo, then enable GitHub Pages:
# Settings → Pages → Source: Deploy from branch → main → /root → Save
```

Live in 2 minutes.

## Local Development

```bash
git clone https://github.com/TechAniket/gitpush-tool.git
cd gitpush-tool
# Open index.html in browser — that's it. No build step needed.
```

## Contributing

PRs welcome! Ideas for new features:
- [ ] GitLab / Bitbucket support
- [ ] SSH remote URL option
- [ ] Multiple remotes
- [ ] Commit template presets

## License

MIT — free to use, fork, and modify.

---

Made by [TechAniket](https://github.com/TechAniket)
