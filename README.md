# QIIME2-Gitpod
Deployment of QIIME2 via Gitpod Workspaces

## Overview
This repository provides a ready-to-use Gitpod workspace configuration for QIIME 2 2025.4 Amplicon Distribution, including the q2-krona plugin for Krona visualizations.

## Features
- **QIIME 2 2025.4 Amplicon Distribution** - Latest version with all amplicon analysis tools
- **Tab Completion** - Full bash tab completion for all QIIME 2 commands
- **q2-krona Plugin** - Interactive taxonomic visualization with Krona
- **Pre-configured Environment** - Ready to use immediately upon workspace launch
- **Gitpod Classic Compatible** - Optimized for Gitpod Classic workspaces

## Quick Start
1. Fork this repository to your GitHub account
2. Open in Gitpod by prefixing the URL with `gitpod.io/#`
   ```
   https://gitpod.io/#https://github.com/YOUR_USERNAME/QIIME2-Gitpod
   ```
3. Wait for the automated setup to complete (approximately 10-15 minutes on first run)
4. The workspace will automatically activate the QIIME 2 environment

## What's Included
- Miniconda3 (latest version)
- QIIME 2 2025.4 Amplicon Distribution
- Full bash tab completion for QIIME 2 commands
- Krona visualization tools
- q2-krona plugin
- Python 3.10 environment
- VS Code extensions for Python development

## Verification Commands
Once the setup is complete, you can verify the installation:
```bash
# Check QIIME 2 version
qiime --version

# Test tab completion (type 'qiime ' and press TAB)
qiime [TAB]

# List installed QIIME 2 plugins
qiime --help

# Verify Krona installation
which ktImportText

# Check q2-krona plugin
qiime krona --help
```

## Environment Details
- **Conda Environment Name**: `qiime2-amplicon-2025.4`
- **Python Version**: 3.10
- **Installation Path**: `/workspace/miniconda3`

## Updates from Previous Version
This repository has been updated from QIIME 2 2024.10 to 2025.4:
- Uses new GitHub-hosted conda environment files
- Updated environment name to match version
- Maintains compatibility with existing workflows
- Continues support for q2-krona plugin

## Troubleshooting
If you encounter any issues:
1. Check that the conda environment is activated: `conda env list`
2. Manually activate if needed: `conda activate qiime2-amplicon-2025.4`
3. For Krona taxonomy issues, run: `ktUpdateTaxonomy.sh`
4. Clear conda cache if needed: `conda clean --all`

### Tab Completion Issues
If tab completion is not working:
1. Ensure the environment is activated: `conda activate qiime2-amplicon-2025.4`
2. Manually source the tab completion: `source $CONDA_DIR/envs/qiime2-amplicon-2025.4/bin/tab-qiime`
3. Refresh your bash session: `source ~/.bashrc`
4. Regenerate QIIME 2 cache: `qiime dev refresh-cache`

## Resources
- [QIIME 2 Documentation](https://docs.qiime2.org/)
- [QIIME 2 Amplicon Tutorial](https://amplicon-docs.qiime2.org/)
- [Krona Documentation](https://github.com/marbl/Krona/wiki)
- [q2-krona Plugin](https://github.com/kaanb93/q2-krona)

## License
This Gitpod configuration is provided as-is for educational and research purposes.
