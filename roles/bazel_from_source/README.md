# Ansible Role: Bazel from Source

This Ansible role builds Bazel from source on ARM-based systems (e.g., Raspberry Pi) or other systems where prebuilt binaries are not available or unsuitable.

## Purpose

- **Build Bazel from source**: This role is specifically designed for cases where you need to compile Bazel from source rather than installing it from prebuilt binaries or package managers.

## Requirements

- Ansible 2.9+
- ARM-based system (e.g., Raspberry Pi) or other compatible environments
- Sufficient disk space and processing power to compile Bazel

## Role Variables

| Variable          | Default   | Description                                  |
|--------------------|-----------|----------------------------------------------|
| `bazel_version`   | `6.3.0`   | The version of Bazel to build.               |
| `bazel_git_repo`  | `https://github.com/bazelbuild/bazel.git` | Git repository for Bazel. |

## Example Playbook

```yaml
- hosts: all
  roles:
    - bazel-from-source