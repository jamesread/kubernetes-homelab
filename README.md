# kubernetes-homelab
A low hardware overhead, high-quality foundation for a Kubernetes homelab. Friendly forkable foundation. 

## Design goal: low hardware overhead 

* Target is a single x86 VM, 4Gb/RAM, but can be scaled.
* Emphasis on using as few projects as is practical, with low resource usage. 
* Targets full Fedora (not container distros like CoreOS or Talos), because it's easy to setup, manage snd debug. It's also readily available on many cloud providers. 
* Helm, because of zero overhead post-install, even though it sucks for Day2. 

## Design goal: high quality 

* Lots of static linting: precommit, yamlfix, etc.
* Initial deploy via ansible. 
* CI and aggressive testing via GitHub actions.
* CD via Flux.
* Use well established mature projects.
* Well documented via Mkdocs.
* Uses Semver, with the major version tracking Fedora. 

## Design goal: friendly forkable foundation. 

* Should be easy to fork, allowing more specialized homelabs to be built on top.
* Should be friendly to forks, allowing them to merge updates easily, with low risk of conflicts.
* This project should be a foundation for building more specialised environments - for security, or developers.

## Anti design goals

* Designed for homelabs, not cloud providers, so won't use any specialist CSI or CNI drivers.
* Prioritize low overhead and simplicity over scale (eg, Flannel over Calico, eg Flux over Argo).
* Won't support variations - eg not Ubuntu, or Talos, or CoreOS.

## This is a No-Nonsense Open Source project

- All code in this project is Open Source (AGPL), and dependencies must use OSI approved Open Source licenses. 
- No company is paying for development, there is no paid-for support from the developers.
- No separate core and premium version, no plus/pro version or paid-for extra features.
- No SaaS service or "special cloud version".
- No "anonymous data collection", usage tracking, user tracking, telemetry or email address collection.
- No requests for reviews in any "app store" or feedback surveys.
- No prompts to "upgrade to the latest version".
- No internet-connection required for any functionality.
