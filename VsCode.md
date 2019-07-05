# Introduction

Visual Studio Code is not officially built for *Raspberry Pi* but there is a project called *Code-OSS* that provide open source builds. These instructions are a condensed version of [How to Install Visual Studio Code on the Raspberry Pi](https://www.youtube.com/watch?v=6AIylZ_UvEA) by user "*MakeUseOf*" (*a big thumbs up for his video*).

# Preparation

## Public GPG key

You need a public GPG key to verify the package when you later install it with **apt**.

```bash
# Get key and pipe it to apt-key
$ wget -O - https://packagecloud.io/headmelted/codebuilds/gpgkey | sudo apt-key add -

# Update apt-get with new resource so that you can find Code-Oss (think "git fetch")
$ sudo apt-get update
```

# Installation

The following version should be "stable" on Raspberry Pi 4.

```bash
# Install Code-OSS
$ sudo apt-get install code-oss=1.29.0-1539702286

# Stop apt from updating Code-OSS
$ sudo apt-mark hold code-oss

# Inform apt to start updating Code-OSS again
$ sudo apt-mark unhold code-oss
```

