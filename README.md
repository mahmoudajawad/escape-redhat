# Escape Red Hat

[Red Hat is going closed source (Warning: YouTube link)](https://www.youtube.com/watch?v=Of18sAJgHxE) and those who choose to work with Red Hat because of its open nature, could need to re-evaluate their options.

On Jun, 21st. [Red Hat announced restricting RHEL packages sources to its paying customers only](https://www.redhat.com/en/blog/furthering-evolution-centos-stream), furthermore Red Hat affirmed its ToS to prohibit its customers from [re-sharing these sources with third-parties](https://twitter.com/GloriousEggroll/status/1672030372979412992) effectively preventing anyone from creating a binary-compatible RHEL clone.


## Articles
[Red Hat Now Limiting RHEL Sources To CentOS Stream](https://www.phoronix.com/news/Red-Hat-CentOS-Stream-Sources)

[Red Hat strikes a crushing blow against RHEL downstreams](https://www.theregister.com/2023/06/23/red_hat_centos_move/)

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


## Your Input
Your input is needed to create a complete reference to escaping Red Hat altogether for those who would like so. Such as more RHEL options, and cloud products and services that depend on Red Hat ecosystem (e.g. OpenShift).

Send in your input, feedback, or opinion via an issue or Merge/Pull Request to this repo.
