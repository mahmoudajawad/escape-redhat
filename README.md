# Escape Red Hat

> Red Hat employees are mad at me on Reddit because I wrote "going closed source". While technically they are not, there's nothing about all the recent moves by Red Hat that goes well with the spirit of free software.

[Red Hat is paywalling access to RHEL source code (Warning: YouTube link)](https://www.youtube.com/watch?v=Of18sAJgHxE) and those who choose to work with Red Hat because of its open nature, could need to re-evaluate their options.

On Jun, 21st. [Red Hat announced restricting RHEL packages sources to its paying customers only](https://www.redhat.com/en/blog/furthering-evolution-centos-stream), furthermore Red Hat affirmed its ToS to prohibit its customers from [re-sharing these sources with third-parties](https://twitter.com/GloriousEggroll/status/1672030372979412992) effectively preventing anyone from creating a binary-compatible RHEL clone.


## Resources
[Red Hat Now Limiting RHEL Sources To CentOS Stream](https://www.phoronix.com/news/Red-Hat-CentOS-Stream-Sources)

[Red Hat strikes a crushing blow against RHEL downstreams](https://www.theregister.com/2023/06/23/red_hat_centos_move/)

[Red Hat Responds To The RHEL Source Code Drama (Warning: YouTube link)](https://www.youtube.com/watch?v=p6wP-6-2XwA)

[Why Corporate Owned Linux Distributions are a Bad Idea (Warning: YouTube link)](https://www.youtube.com/watch?v=fqfyM7zE6KM)

[Red Hat: why I'm going all in on community-driven Linux distros (Warning: YouTube link)](https://www.youtube.com/watch?v=vUXYbt1eLTA)

## Red Hat Products Alternatives
While the announcement is related to users who are interested in community-supported RHEL clones such as [AlmaLinux](https://almalinux.org/) and [Rocky Linux](https://rockylinux.org/), it might be a chance for users to re-consider every offering from Red Hat and understand what alternatives have.

### RHEL
Red Hat Enterprise Linux is the flagship product from Red Hat. This is the only product affected with Red Hat recent announcement, and users of RHEL clones will need to plan their next move soon before they are left without security updates on their running hosts, be it workstations or servers.

The easiest path is to migrate to RHEL and become a paying customer. However, this is not what this document is discussing but what alternatives outside of Red Hat realms are.

#### RHEL Alternative: Debian
[Debian](https://www.debian.org/) is the project behind one of the two factions in GNU/Linux distros world with its own `deb` package format. Debian has been running steadily by the community for almost three decades. That's a decade over RHEL. Debian distro doesn't see any commercial support from Debian project, but enough service providers around the globe do. Debian runs a very stable release for its distro. Its current release, [Debian 12 (codename bookworm)](https://www.debian.org/News/2023/20230610), will be supported for five years until mid 2028.

Debian is already very common for running demanding production loads. Many of the `Docker` images are based on Debian as it is also common among the developers.

Past releases of Debian stable had the problem of the packages being very late to be updated for non-security updates. As such, developers and engineers could have avoided it in the past because they are looking for more frequent updates to the [packages provided and maintained by the project](https://packages.debian.org/stable/), however, Debian 12 marked a significant change in this policy making feature updates to packages seeing faster track than it used to be.

Moving to Debian from RHEL clones is best if your work will not be affected by the change of package formats on host (from `RPM` to `deb`). This includes:
- Systems built with interpreted languages (Python, Ruby, PHP, ..etc.).
- Systems built with Java (JVM provides portability to systems).
- Containerized systems (Docker, LXC, ...etc.).

However, if your work is tightly tied to RHEL structure and its features this might not be the best option.

#### RHEL Alternative: openSUSE and SLES
SUSE is the company behind one of the flagship Enterprise Linux releases; [SUSE Linux Enterprise Server](https://www.suse.com/products/server/). SUSE offers community-supported [openSUSE](https://www.opensuse.org/) distro as well which [has become binary-compatible to the commercial offering](https://en.opensuse.org/Portal:Leap/FAQ/ClosingTheLeapGap) with the release of openSUSE Leap 15 and SLES 15. This offers a clear path to individual and businesses who need to run their workloads with community-supported Enterprise Linux release, but still would want to have that option to simply flip the switch to a commercially supported release.

Another feature of openSUSE and SLES is the wide hardware support. Historically, Red Hat didn't conquer every new hardware corner, Unlike SUSE which is not afraid of providing support to almost any form of hardware where Linux kernel could run.

Moving to openSUSE and SLES, is best if:
- You anticipate need of commercial support along your journey.
- Your systems are built and tied to `RPM` package format.
- You plan use of hardware that is supported by SUSE wide hardware support portfolio.

However, it should be clear that moving to openSUSE and SLES isn't like switching between a RHEL clone and another, as it isn't binary-compatible with RHEL, however migrating to it should be easier than migrating to a non-`RPM` distro.

### Fedora
Fedora is the testing playground for Red Hat. Red Hat doesn't like this title, though, and keep tooting "Red Hat supported community". Now, [Red Hat wants to add telemetry to Fedora](https://discussion.fedoraproject.org/t/f40-change-request-privacy-preserving-telemetry-for-fedora-workstation-system-wide/85320/118). While this is presented as a topic to discuss it follows suit; Red Hat wants to squeeze any commercial opportunity from the community that made Red Hat. Users of Fedora need to find the alternative.

#### Fedora alternative: NixOS
If you are a developer, NixOS will probably be the distro you've always been looking for. It has been best [explained by Chris Titus in this video (Warning: Youtube link)](https://www.youtube.com/watch?v=fuWPuJZ9NcU), so, switch from Fedora to NixOS if:
- You are a developer who wants to drive your GNU/Linux installation by configuration, just like you do with your code.
- You are leading a development team, that needs to be able to launch re-producible environments the way VMs are.
- You are a GNU/Linux advanced user who wants an operating system that is built around an easy to use packages format (Nix) to build his own.

However, consider peeking at what NixOS and Nix are before making that jump as the experience is not the same, and a sudden switch might leave you with certain software that don't work the way they did on regular distros, and the live USB media is a great opportunity to test it all.

#### Fedora alternative: Debian
Before this documents becomes a celebration for Debian, it is needed to be stated that if your use of Fedora is because of how stable it is, then the stability of Debian is the only thing that is comparable. However, Debian doesn't cover it all, so moving to Debian on workstation from Fedora is best if:
- You are after stability on the workstation.
- You like to have access to large catalogue of programs and applications.
- You want to streamline your experience across personal workstation and business servers and computers.

However, Debian doesn't offer latest software by default as it eyes stability, and while Flathub covers this spot, not all programs and applications are best experienced via Flatpak.

#### Fedora alternative: Arch Linux
Arch is a rolling-release GNU/Linux distro, what this means is Arch doesn't have versions, but rather snapshots of some recent build that can be installed and be updated for ever with every new release of a package. This is great by principle because it omits the necessity to follow an upgrade-pipe every few months like with most of GNU/Linux distros. This approach also guarantees having most of packages be up-to-date as there are no restrictions about software versions whatsoever (HUGE ASTERISK HERE). So, switch to Arch if:
- You want to move around telling everyone "I use Arch, BTW!".
- You want cutting-edge experience with programs and applications.
- You understand what rolling-release gives you in both of powers and responsibilities towards keeping your installation working.

However, if you are not ready for a rolling-release model, as it exposes compatibility issues with time, you need to avoid switching to Arch, but it might still be a great experience as a VM or a side distro.

## Your Input
Your input is needed to create a complete reference to escaping Red Hat altogether for those who would like so. Such as more RHEL options, and cloud products and services that depend on Red Hat ecosystem (e.g. OpenShift).

Send in your input, feedback, or opinion via an issue or Merge/Pull Request to this repo.


## Mirrors
This document is mirrored on:
- GitLab: [https://gitlab.com/mahmoudajawad/escape-redhat](https://gitlab.com/mahmoudajawad/escape-redhat)
- GitHub: [https://github.com/mahmoudajawad/escape-redhat](https://github.com/mahmoudajawad/escape-redhat)
