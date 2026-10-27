# nabd-updates

Update files for the **Nabd** clinic management app for Windows, by Fadi Hamad.

This repository only hosts the files the installed app downloads to update itself. Each GitHub
release holds exactly two files:

- `update.json`: a small manifest signed with Ed25519 (version, release notes, the installer's
  name, size and SHA-256);
- `Nabd-Setup-<version>-build<n>.exe`: the Windows installer.

The app checks the signature with public keys built into it, and the installer's size and
SHA-256, before it installs anything. A file that does not verify is never used.

There is **no source code** here and **no secrets**: no keys, no passwords, no configuration,
no clinic or patient data. Please do not open issues or pull requests with personal or patient
information.

## Rights

All rights reserved. The installers and the app are © Fadi Hamad. They are published here only
so that installed copies of Nabd can update themselves; no licence to copy, modify or
redistribute them is granted by this repository.

## Contact

Fadi Hamad, the publisher of Nabd.
