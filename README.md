[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/Corveda/ddev-redash/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/Corveda/ddev-redash/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/Corveda/ddev-redash)](https://github.com/Corveda/ddev-redash/commits)
[![release](https://img.shields.io/github/v/release/Corveda/ddev-redash)](https://github.com/Corveda/ddev-redash/releases/latest)

# DDEV Redash

## Overview

This add-on integrates Redash into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get Corveda/ddev-redash
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Redash |
| `ddev logs -s redash` | Check Redash logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.redash --redash-docker-image="ddev/ddev-utilities:latest"
ddev add-on get Corveda/ddev-redash
ddev restart
```

Make sure to commit the `.ddev/.env.redash` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `REDASH_DOCKER_IMAGE` | `--redash-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@Corveda](https://github.com/Corveda)**
