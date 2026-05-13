[![add-on registry](https://img.shields.io/badge/DDEV-Add--on_Registry-blue)](https://addons.ddev.com)
[![tests](https://github.com/mikaykun/ddev-seaweedfs/actions/workflows/tests.yml/badge.svg?branch=main)](https://github.com/mikaykun/ddev-seaweedfs/actions/workflows/tests.yml?query=branch%3Amain)
[![last commit](https://img.shields.io/github/last-commit/mikaykun/ddev-seaweedfs)](https://github.com/mikaykun/ddev-seaweedfs/commits)
[![release](https://img.shields.io/github/v/release/mikaykun/ddev-seaweedfs)](https://github.com/mikaykun/ddev-seaweedfs/releases/latest)

# DDEV Seaweedfs

## Overview

This add-on integrates Seaweedfs into your [DDEV](https://ddev.com/) project.

## Installation

```bash
ddev add-on get mikaykun/ddev-seaweedfs
ddev restart
```

After installation, make sure to commit the `.ddev` directory to version control.

## Usage

| Command | Description |
| ------- | ----------- |
| `ddev describe` | View service status and used ports for Seaweedfs |
| `ddev logs -s seaweedfs` | Check Seaweedfs logs |

## Advanced Customization

To change the Docker image:

```bash
ddev dotenv set .ddev/.env.seaweedfs --seaweedfs-docker-image="ddev/ddev-utilities:latest"
ddev add-on get mikaykun/ddev-seaweedfs
ddev restart
```

Make sure to commit the `.ddev/.env.seaweedfs` file to version control.

All customization options (use with caution):

| Variable | Flag | Default |
| -------- | ---- | ------- |
| `SEAWEEDFS_DOCKER_IMAGE` | `--seaweedfs-docker-image` | `ddev/ddev-utilities:latest` |

## Credits

**Contributed and maintained by [@mikaykun](https://github.com/mikaykun)**
