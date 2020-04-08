BigBlueButton Minimal
=====================

*Objective:*

* Provide mock `deb`s for all red5 components
* Provide mock `deb`s for `kurento-media-server` (install it on a separate machine)
* Provide mock `deb`s for `FreeSWITCH` (install it on a separate machine)
* Work with what's left (mostly portable Java/Scala JavaScript/Meteor components)

*Method:*

* Use [equivs][1] to build mock packages for unwanted / external dependencies.
* Use docker to verify whether the result leads to an installable
  `bigbluebutton` metapackage (See Dockerfiles and build logs on [travis][2]).

[1]: https://packages.debian.org/buster/equivs
[2]: https://travis-ci.org/github/znerol/bbb-minimal
