[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/brookemahoney/ddev-vtracer/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/brookemahoney/ddev-vtracer/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/brookemahoney/ddev-vtracer)](https://github.com/brookemahoney/ddev-vtracer/commits)
[![release](https://img.shields.io/github/v/release/brookemahoney/ddev-vtracer)](https://github.com/brookemahoney/ddev-vtracer/releases/latest)

# DDEV Vtracer

## Overview

This add-on integrates Vtracer into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get brookemahoney/ddev-vtracer
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Vtracer |
| `ddev logs -s vtracer` | Check Vtracer logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.vtracer --vtracer-docker-image="ddev/ddev-utilities:latest"
ddev add-on get brookemahoney/ddev-vtracer
ddev restart
```

Make sure to commit the `.ddev/.env.vtracer` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `VTRACER_DOCKER_IMAGE` | `--vtracer-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@brookemahoney](https://github.com/brookemahoney)**
