## Continuous Delivery
<img src="images/release-cycle/release-cycle-release.png" style="background:none; border:none; box-shadow:none;"/>

----

### What is delivery

> Store a deliverable which could be deployed in production environment

----

### Deliverable tracability

* The deliverable can be tracked through preceding and following steps
* With a deliverable is associated:
  * An issue/ticket
  * some commits
  * A tag 
  * A friendly version known by user (to get bug reports)

----

### Versioning problematic

> To help with deliverable tracability, version number must be well thought

* Versioning sometimes challenges content and delivery deadline
* Versioning example: MAJOR.MINOR.PATCH-gitsha (5.21.12-8fds9h)

----

### Manual production deployment

* Continuous delivery does not automate production deployment
* Production deployment is launched manually after human validation

----

### Skills

Domain | Examples
--- | ---
Packaging appli | Maven, NPM, MsBuild, Python, Docker, Podman, Buildah
Artifact storer | Artifactory, Nexus, DockerHub
