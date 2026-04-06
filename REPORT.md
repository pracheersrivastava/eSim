# eSim Task 4 – Ubuntu 25.04 Compatibility Report

## Environment
- Platform: GitHub Codespaces
- OS: Ubuntu 25.04
- Repo: fork of FOSSEE/eSim
- Branch: master
- Commit: d4859de7

## Issues Found
1. install-eSim.sh did not support Ubuntu 25.04
2. xz-utils install command missing `install -y`
3. KiCad 6 PPA incompatible with 25.04
4. libcanberra-gtk-module removed in Ubuntu 25.04
5. NGHDL/GHDL/Verilator scripts assumed tar archives not present in repo clone
6. IHP optional install blocked headless flow
7. Desktop shortcut creation failed in Codespaces

## Fixes Applied
- Added Ubuntu 25.04 installer routing
- Added install-eSim-25.04.sh
- Fixed KiCad 8 PPA routing
- Updated libcanberra dependency
- Skipped archive-based NGHDL/GHDL/Verilator builds for repo clone testing
- Fixed NGHDL softlink path
- Skipped IHP for Ubuntu 25.04 testing
- Skipped Desktop icon creation in headless environment

## Final Result
eSim installed successfully on Ubuntu 25.04 in Codespaces.

## Repository
https://github.com/pracheersrivastava/eSim
