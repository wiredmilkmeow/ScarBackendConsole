# ScarBackendConsole

A backend console application for automating Roblox client tracking, build
analysis, Git repository management, and update workflows.

ScarBackendConsole is designed to handle the backend-side tooling required
to analyse Roblox client builds, maintain tracked repositories, and publish
detected changes through Git.

---

## Overview

ScarBackendConsole operates as a command-line backend service that connects
Roblox build data with Git-based repositories.

It can be used to:

- Track Roblox client builds
- Track Roblox FastFlags
- Analyse client updates
- Manage Git branches and repositories
- Automatically commit detected changes
- Rebase tracked branches against their parents
- Process manually assembled client builds
- Configure automated update intervals
- Provide verbose Git operation logging

The application is intended to run as a backend/developer utility rather
than as a user-facing Roblox application.

---

## Features

### Roblox Client Tracking

Automatically processes Roblox client builds and tracks changes between
versions.

The tracker can analyse a newly detected build and update the corresponding
repository when changes are found.

### FastFlag Tracking

Supports a separate tracking mode for Roblox FastFlags.

```text
-trackMode FastFlags