# Security policy

## Reporting a vulnerability

Do not open a public issue for a security problem. Use GitHub's private
reporting instead:

- Open the affected repository and go to **Security → Report a vulnerability**
  (GitHub Security Advisories), or
- contact the maintainer listed in the repository.

Include the affected component and version, a description of the impact, and a
reproduction if you have one. You will get an acknowledgement as soon as
possible and credit in the advisory once a fix is published.

## Scope

The stack runs on the user's session and installs system pieces (packages,
SDDM theme, `/etc/pam.d/quickshell`). Reports about the shell, the Hyprland
scripts, the installers, the wallpaper engine or the scene runtime are welcome;
keep in mind that scenes execute user-authored code in the client by design
(the runtime sandbox is documented in `x-ports/xwww`).

## Supported versions

Only the latest release of each repository receives fixes; `dots update` keeps
an installation on the current releases.
