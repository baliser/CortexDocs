![](images/cortex-logo.png)

[![Join the chat at https://gitter.im/TheHive-Project/TheHive](https://badges.gitter.im/TheHive-Project/TheHive.svg)](https://gitter.im/TheHive-Project/TheHive)

Cortex solves a common problem frequently encountered by SOCs, CSIRTs and security researchers in the course of threat intelligence, digital forensics and incident response: how to analyze observables they have collected, **at scale, by querying a single tool** instead of several? Thanks to its many analyzers and to its RESTful API, Cortex makes observable analysis a breeze, particularly if called from [TheHive](https://github.com/TheHive-Project/TheHive/), our highly popular, free and open source Security Incident Response Platform.

Starting from Cortex version 2, you can create and manage multiple organizations (i.e multi-tenancy), manage the associated users and give them different roles. You can also specify per-org analyzer configuration and rate limits to avoid consuming all your quotas at once. We have also added a cache so that an analysis is not re-executed for the same observable if a given analyzer is called on that observable several times within a specific timespan (10 minutes by default).

**Note:**  This is the Cortex documentation repository. If you are looking for its source code, please visit [https://github.com/CERT-BDF/Cortex/](https://github.com/TheHive-Project/Cortex/).

**Note:** [Cortex4py](https://github.com/TheHive-Project/Cortex4py), the Python lib to submit observables in bulk mode through the Cortex REST API from alternative SIRP platforms & custom scripts, does not support Cortex 2 yet. It will be updated soon. 

## Hardware Pre-requisites
Cortex uses a Java VM. We recommend using a virtual machine with 8vCPU, 8 GB of RAM and 10 GB of disk. You can also use a
physical machine with similar specifications.

## What's New

- [Quick Start Guide](quick-start.md)
- [How to Configure Analyzers](analyzer_requirements.md)
- [How to Create an Analyzer](api/how-to-create-an-analyzer.md)
- [Training Material](https://github.com/TheHive-Project/TheHiveDocs/blob/master/training-material.md)
- [Changelog](https://github.com/TheHive-Project/Cortex/blob/master/CHANGELOG.md)

## Installation Guides

Cortex can be installed using:
- An [RPM package](installation/rpm-guide.md)
- A [DEB package](installation/deb-guide.md)
- [Docker](installation/docker-guide.md)
- [Binary](installation/binary-guide.md)

Cortex can also be [built from sources](installation/build-guide.md).

Once you have installed Cortex, you need to [install the analyzers](installation/analyzers.md)
and [configure them](analyzer_requirements.md).

## User Guides

- [Cortex Analyzer Requirements Guide](analyzer_requirements.md)

## Developer Guides

- [API Documentation](api/README.md) (**OUTDATED**, will be updated soon)
- [How to Create an Analyzer](api/how-to-create-an-analyzer.md)

## Other
- [Training Material](https://github.com/TheHive-Project/TheHiveDocs/blob/master/training-material.md)
- [FAQ](FAQ.md)

# License
Cortex is an open source and free software released under the [AGPL](https://github.com/TheHive-Project/TheHive/blob/master/LICENSE) (Affero General Public License). We, TheHive Project, are committed to ensure that TheHive will remain a free and open source project on the long-run.

# Updates
Information, news and updates are regularly posted on [TheHive Project Twitter account](https://twitter.com/thehive_project) and on [the blog](https://blog.thehive-project.org/).

# Contributing
We welcome your contributions. Please feel free to fork the code, play with it, make some patches and send us pull requests using [issues](https://github.com/TheHive-Project/Cortex/issues).

We do have a [Code of conduct](code_of_conduct.md). Make sure to check it out before contributing.

# Support
Please [open an issue on GitHub](https://github.com/TheHive-Project/Cortex/issues/new) if you'd like to report a bug or request a feature. We are also available on [Gitter](https://gitter.im/TheHive-Project/TheHive) to help you out.

If you need to contact the Project's team, send an email to <support@thehive-project.org>.

**Important Note**:

- If you have troubles with a Cortex analyzer or would like to request a new one or an improvement to an existing analyzer, please open an issue on the [analyzers' dedicated GitHub repository](https://github.com/TheHive-Project/cortex-analyzers/issues/new).
- If you encounter an issue with TheHive or would like to request the addition of a feature in it, please [open an issue on its dedicated GitHub repository](https://github.com/TheHive-Project/TheHive/issues/new).
- If you have problems with [Cortex4py](https://github.com/TheHive-Project/Cortex4py), please [open an issue on its dedicated repository](https://github.com/TheHive-Project/Cortex4py/issues/new).

# Community Discussions
We have set up a Google forum at <https://groups.google.com/a/thehive-project.org/d/forum/users>. To request access, you need a Google account. You may create one [using a Gmail address](https://accounts.google.com/SignUp?hl=en) or [without it](https://accounts.google.com/SignUpWithoutGmail?hl=en).

# Website
<https://thehive-project.org/>
