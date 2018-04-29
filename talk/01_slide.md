!SLIDE[bg=_images/backgrounds/white_bg.png] incremental
# Definitions

* Project: Usually one git repo, open source

* Upstream: The open source code base and community

* Production: Collection of services that your organization is responsible for

* Downstream: Code written and/or used by your organization

* Master: The master git branch, trunk in svn terms. Can be upstream or downstream


!SLIDE[bg=_images/backgrounds/white_bg.png] incremental
# Definitions

* Local Fork: A downstream copy of an upstream project, with local changes


!SLIDE[bg=_images/backgrounds/white_bg.png] incremental
# How do you get to local forks

* Performance
* Bug
* Fix/Integration that isn't being accepted by upstream
* Packaging bug
* Old packaging
* Security issue/patch
* Stuck on old version, but need new feature


!SLIDE[bg=_images/backgrounds/white_bg.png]

.huge Open Source <span class="teal">consumption </span> has changed in the past few years. Companies and organizations are using <span class="teal">smaller and smaller</span>  projects.


!SLIDE[bg=_images/backgrounds/white_bg.png] incremental
# How do you Deploy and work with local forks

* Package?
* Git?
* Compiled?
* Build Package?

!SLIDE[bg=_images/backgrounds/white_bg.png] incremental
# CI / CD

* How much validation do you do on your deploys?
* How much of the process is automated?
* What is your risk tolerance?

!SLIDE[bg=_images/backgrounds/white_bg.png] incremental
# Working with upstream

* Don't be bad - contribute!
* What are the barriers to contributing?
* Is this a time issue?
* Are there licensing/approval issues?
* Open Source experience?


!SLIDE[bg=_images/backgrounds/black_bg.png]

.blockwhite The most basic case:

.blockteal A single pull request


!SLIDE[bg=_images/github_conversation.png] background-fit


!SLIDE[bg=_images/backgrounds/white_bg.png] incremental
# Two strategies

* Merge
* Rebase


!SLIDE[bg=_images/backgrounds/white_bg.png] incremental
# Three examples I've worked on


* Puppet module
* CI software
* OpenStack


!SLIDE[bg=_images/backgrounds/white_bg.png] incremental
# Five examples I've worked on

* Pull Request
* Puppet Module
* IBM Kubernetes
* CI Software
* OpenStack


!SLIDE[bg=_images/backgrounds/white_bg.png] incremental
# Details on Rebase Strategy

* Bad - Destroys history
* Bad - Must constantly redo conflicts
* Bad - "Too easy", ends up being big diffs
* Good - Much simpler


!SLIDE[bg=_images/backgrounds/white_bg.png] incremental
# Details on Merge Strategy

* Bad - Must do the work to merge
* Bad - Difficult to tell what the diff is
* Bad - No path to 'pure sync'
* Good - Conflicts resolved usually once
* Good - preserves deployment history


!SLIDE[bg=_images/backgrounds/white_bg.png] incremental
# Lessons

* Keep diff small if you can
* Start with rebase strategy
* Sync often or fail
* Work with upstream, always worth it
* Build a drift dashboard
* Automate the syncing, push that through some CI/valiation
* Be mindful of dependencies


!SLIDE[bg=_images/backgrounds/black_bg.png]

.blockwhite Thank You!

.blockteal Spencer Krum // IBM

.blockteal @nibalizer
