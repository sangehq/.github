<div align="center">
  <a href="https://sange.sh">
    <picture>
      <source media="(prefers-color-scheme: dark)" srcset="banner-dark.svg">
      <img alt="sange — a git safety layer by Simtabi" src="banner-light.svg" width="888">
    </picture>
  </a>
</div>

# Git that checks before it lets go.

sange is a version-control workspace that keeps the wrong identity, the wrong
files and the wrong data from leaving your machine. It sits in front of every
repository as git hooks and checks each commit and push against the identity
bound to that repository and the rules you set for it. This organisation holds
the Go rewrite: one binary for macOS, Linux, Windows and FreeBSD, released on
GitHub and nowhere else.

Most leaks are not attacks. They are a commit made under a client's identity
from a personal laptop, an `.env` that slipped past `.gitignore`, a customer's
email pasted into a fixture. Each is cheap to catch on the machine where it
happens and expensive everywhere after, so sange checks locally and fails
closed: when it cannot decide, it stops and says why.

sange itself is private while the rewrite settles; the tools it is built with
are public here.

## Get in touch

- Trying sange or following it: [sange.sh](https://sange.sh).
- Security: [security@simtabi.com](mailto:security@simtabi.com) — never a public issue.
  See the [security policy](https://github.com/sangehq/.github/security/policy).
- Anything else: [opensource@simtabi.com](mailto:opensource@simtabi.com). A human
  reads it.

Built and maintained by the team at [Simtabi](https://simtabi.com).
