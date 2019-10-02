# in-toto Incubating Stage Review

in-toto is currently a CNCF sandbox project. Please refer to in-toto's initial
[sandbox proposal](../proposals/in-toto.adoc) for discussion on in-toto's
alignment with the CNCF and details on sandbox requirements.

In the time since being accepted as a sandbox project, in-toto has demonstrated
healthy growth and progress.

* [v0.4.0 is the latest release](https://github.com/in-toto/in-toto/releases),
  shipped on September 7th, marking our 7th major feature release. New features
  include:

  * Full artifact rule spec compliance[1](https://github.com/in-toto/in-toto/pull/269)[2](https://github.com/in-toto/in-toto/pull/280)
  * Enhanced OpenPGP key export and key expiration verification[1](https://github.com/in-toto/in-toto/pull/266)[2](https://github.com/in-toto/in-toto/pull/288)
  * Transitive PyNaCl dependency is now optional[1](https://github.com/in-toto/in-toto/pull/296)
  * Improved automatic test coverage analysis[1](https://github.com/in-toto/in-toto/pull/295)
  * Static analysis improvements[1](https://github.com/in-toto/in-toto/pull/279)[2](https://github.com/in-toto/in-toto/pull/296)
  * Improve upstream release packaging for Debian and Arch Linux[1](https://github.com/in-toto/in-toto/pull/279)[2](https://github.com/in-toto/in-toto/pull/290)
  
More changes and small improvements are mentioned in the current release
changelog. 

Beyond the current release other improvements to the broader reference
implementation have been achieved.

FIXME:
* A [formalized governance
policy](https://github.com/in-toto/docs/blob/master/GOVERNANCE.md) has been
instituted project-wide. This incldues not only the in-toto python reference
implementation, but the specifications, implementations in other languages and
cloud-native tooling.

## Incubating Stage Criteria

In addition to sandbox requirements, a project must meet the following
criteria to become an incubation-stage project:

* Document that it is being used successfully in production by at least three
independent end users which, in the TOC’s judgement, are of adequate quality
and scope.

  * We document adopters on the
    [ADOPTERS.md](https://github.com/in-toto/in-toto/blob/develop/ADOPTERS.md)
    file

* Have a healthy number of committers. A committer is defined as someone with
the commit bit; i.e., someone who can accept contributions to some or all of
the project.

  * Maintainers of the project are listed in our [MAINTAINERS.txt](https://github.com/in-toto/in-toto/blob/develop/MAINTAINERS.txt) file. There are currently 3 core maintainters plus X more maintainers from companies such as (Debian, Datadog, and VMWare)

  * Maintainers are added and removed from the project as per the policies
outlined in the project [GOVERNANCE.md](https://github.com/in-toto/docs/blob/master/GOVERNANCE.md) file.

* Demonstrate a substantial ongoing flow of commits and merged contributions.

  * Releases: There was one [release](https://github.com/in-toto/in-toto/releases) scheduled since the sandbox application as defined on our [release schedule](https://github.com/in-toto/in-toto/blob/develop/ROADMAP.md)

  * Roadmap: our [ROADMAP.md](https://github.com/in-toto/in-toto/blob/develop/ROADMAP.md) file describes our yearly roadmap. Since, we have had one roadmap [review](https://github.com/in-toto/in-toto/blob/develop/roadmap-reviews/2019/01-roadmap-review.md)

  * Contributors: [https://github.com/in-toto/in-toto/graphs/contributors](https://github.com/in-toto/in-toto/graphs/contributors)

  * Commit activity: [https://github.com/in-toto/in-toto/graphs/commit-activity](https://github.com/in-toto/in-toto/graphs/commit-activity)

  * CNCF DevStats: [https://intoto.devstats.cncf.io/](https://intoto.devstats.cncf.io/)
    * [Last 30 days activity on GitHub](https://intoto.devstats.cncf.io/d/8/dashboards?refresh=15m&orgId=1&from=now-30d&to=now-1h)
    * [Community Stats](https://intoto.devstats.cncf.io/d/3/community-stats?orgId=1&var-period=d7&var-repo_name=goharbor%2Fharbor)

FIXME: should we bother with this? or is it more worthwhile inlining this information in this document.
A more complete picture of in-toto's growth and progress since being accepted
as a sandbox project is described in the following [slide deck](TBD)

## Security

Given that in-toto is a security product, in-toto's codebase has been written,
designed and tested with security in mind. Some of the actions performed in
order to ensure the quality and security of the codebase, as well as in-toto's
design and specification include:

* Static analysis is performed using [pylint](FIXME) and [bandit](FIXME)
* Dependency vulnerability tracking using [UpdateBot](FIXME)
* Manual code analysis / review by a Maintainer for each included piece of
  code.
* [Security assesment](FIXME) by CNCF's SIG-SECURITY
* A peer-reviewed paper describing the threat model, it's
  security properties, was published in 
  [USENIX Security '19](https://www.usenix.org/conference/usenixsecurity19/presentation/torres-arias)
* in-toto's implementation has received the [CII Silver Criteria Badge](FIXME)
  for best development practices.

A more elaborated descritption of these security initiatives, as well as a
vulnerability report process is included in the [SECURITY.md](https://github.com/in-toto/in-toto/blob/develop/SECURITY.md) file.
