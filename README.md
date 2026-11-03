# Cadence Bubble releases

This repository holds **only the release files** of the Cadence Bubble, Sempar's
desktop companion for Cadence: the installers, their update signatures and the
update manifest (`latest.json`) that installed bubbles read to find a new
version. **There is no code here**; the program is built from a private
repository by GitHub Actions, and each release is published here by that build.

- **Installers do nothing on their own.** Everything the bubble shows comes from
  Cadence, and needs a Sempar Microsoft sign-in on Sempar's Cadence team.
- **Updates are signed.** Every installed bubble checks each update's signature
  against Sempar's own key before installing it; a changed or fake file is refused.
- **For Sempar's IT:** `Cadence-Bubble-Setup-<version>.msi` is the machine-wide
  package (install with `msiexec /i "Cadence-Bubble-Setup-<version>.msi" /qn`);
  it sets the bubble up for each person at their next Windows sign-in.

Please don't open issues or pull requests here.
