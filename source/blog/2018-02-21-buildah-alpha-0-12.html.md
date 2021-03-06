---
title: Buildah Alpha version 0.12 Release Announcement
author: tsweeney
date: 2018-02-21 00:00:00 UTC
published: true
comments: false
tags: atomic, buildah, containers
---

We're pleased to announce the release of Buildah Alpha version 0.12 on both Fedora 26 and Fedora 27. As always, the latest Buildah can also be acquired from [GitHub](https://github.com/projectatomic/buildah) for any other Linux distribution.

The Buildah project has been building some steam over the past several weeks, welcoming several new contributors to the mix, launching new functionality and creating a number of improvements and bug fixes. The major highlights for this release are:

READMORE

* Added better handling of error messages for Unknown Dockerfile instructions.
* Set the default certificate directory to /etc/containers/certs.d.
* Vendored in the latest containers/image and containers/Storage packages.
* The build-using-dockerfile (bud) command now sets the images 'author' field to the value provided by MAINTAINER in the Dockerfile.
* Return exit code 1 when 'buildah rmi' fails.
* Improve lookups of a variety of image name formats.
* Adds the --format and --filter parameters to the 'buildah containers' command.
* Adds the --prune,-p option to the 'buidah rmi' command allowing dangling images to be pruned.
* Adds the --authfile parameter to the 'buildah commit' command.
* Fix the --runtime-flag for the 'buildah run' and 'buildah bud' commands when global flags are used.
* The format parameter now overrides the quiet parameter for 'buildah images'.
* Provide authentication parameters to the build-using-docker-file (bud) command.
* Directory permissions are no longer overwritten when using the --chown parameter.
* HTML character output to the terminal is no longer escaped.
* The container name is now always set to the image's name.
* The username or password are prompted for if they are not supplied with the --creds parameter.
* Return a better error message when bad credentials are used to pull a private image.
* Plus several small bug fixes.

If you haven’t yet,  install Buildah from the Fedora repository and give it a spin.  We’re betting you'll find it’s an easy and quick way to build containers in your environment without a daemon being involved!

If you haven't joined our community yet, don't wait any longer!  Come join us in [GitHub](https://github.com/projectatomic/buildah), where Open Source communities live.

**Buildah == Simplicity**
