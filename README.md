# Resume

LaTeX source and automated publish pipeline for my resume.

## How It Works

Any push to `main` triggers a GitHub Actions workflow that:
1. Compiles `William_Ortiz_Resume.tex` to PDF
2. Pushes the output to [williamortizdev/williamortiz.dev](https://github.com/williamortizdev/williamortiz.dev) at `assets/files/William_Ortiz_Resume.pdf`


## Setup

1. Create a [Personal Access Token](https://github.com/settings/tokens) with `repo` scope on the portfolio repo
2. Add it as a repository secret named `PORTFOLIO_REPO_TOKEN` under **Settings → Secrets and variables → Actions**

That's it — the pipeline handles the rest on every push.

## Files

| File | Description |
|------|-------------|
| `William_Ortiz_Resume.tex` | LaTeX resume source |
| `.github/workflows/deploy-resume.yml` | Compile and publish workflow |
