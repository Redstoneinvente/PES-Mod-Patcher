# PES Mod Patcher

A responsive, football-inspired download page with a browser password gate, password visibility toggle, accessible feedback, and a download card.

## Hosting

Serve the repository root as a static website. For GitHub Pages, select Settings > Pages > Deploy from a branch > main > / (root).

Place the real `Patcher.zip` alongside `index.html`. The download uses the relative URL `./Patcher.zip`. The archive is not included yet.

## Access behavior

The supplied password is case-sensitive. Leading and trailing whitespace is ignored. Reloading or clicking Lock download closes the gate.

This is a browser-only convenience gate, not secure file authorization. Public repository files and directly hosted ZIP URLs remain accessible. Use a backend that checks authorization before serving the archive if protected downloads are required.

## Validation

Inline JavaScript syntax and password acceptance/rejection cases were checked. No external dependencies or build step are required.
