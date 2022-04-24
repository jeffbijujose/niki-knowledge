---
title: NixOS
---

# [NixOS](https://nixos.org)

NixOS is a Linux distro built around the Nix package system. Nix is built around the idea of immutability. It makes all packages immutable by giving them their own directory identified by a hash that is derived from ALL of that package's dependencies. This has a number of desirable properties:

- It makes it trivial to have multiple versions of the same package installed at the same time and allows you to switch between them at will.
- It is trivial to roll back your system after a failed upgrade. Difficult system recovers after you upgrade to a new unstable version are a thing of the past.
- Non-privileged users can install software completely securely.
- Projects packaged with nix have the best possible build reproducibility because nix accounts for ALL of your dependencies all the way down to the lowest level system libraries, compilers, etc.

Whilst I don't use NixOS as my primary OS. I use [nix package manager](../../package-managers/nix/nix.md) on macOS. And I am exploring using NixOS for servers I use.

[NixOS Weekly](https://weekly.nixos.org/) is useful newsletter. [NixOS MicroVMs](https://github.com/astro/microvm.nix) seem neat.

## Nix configs (NixOS)

- [Mitchell Hashimoto](https://github.com/mitchellh/nixos-config) - Work for both Intel and Apple Silicon. ([Tweet](https://twitter.com/mitchellh/status/1452721115009191938)) ([NixOS VM on Mac Setup](https://www.youtube.com/watch?v=ubDMLoWz76U))
- [Infrastructure](https://github.com/rvolosatovs/infrastructure) ([How to use it](https://github.com/rvolosatovs/infrastructure/issues/3))
- [Rehno Lindeque](https://github.com/rehno-lindeque/wip)
- [Bob nix-home](https://github.com/bobvanderlinden/nix-home)
- [Brian McKenna Nix Files](https://github.com/puffnfresh/nix-files) - NixOS configuration and custom Nix derivations.
- [William A. Kennington III](https://github.com/wkennington/nixos) - NixOS configurations for my local cluster of machines.
- [Arian van Putten](https://github.com/arianvp/nixos-stuff)
- [Michael Peyton Jones](https://github.com/michaelpj/nixos-config)
- [Grégoire Martinache's Infrastructure](https://github.com/M-Gregoire/infrastructure)
- [Silvan Mosberger](https://github.com/Infinisil/system)
- [Vincent Ambo's depot](https://github.com/tazjin/depot) - Personal monorepo of my services & tools.
- [Aaron Janse](https://github.com/aaronjanse/dotfiles)
- [Sridhar Ratnakumar](https://github.com/srid/nix-config)
- [homelab](https://github.com/danderson/homelab) - NixOS configurations for home servers. ([Tweet](https://twitter.com/dave_universetf/status/1236634753765269512))
- [Henrik Lissner](https://github.com/hlissner/dotfiles)
- [Edmund Wu](https://github.com/eadwu/nixos-configuration)
- [Roman Gonzalez](https://github.com/roman/nix-dots)
- [Kim Zick](https://github.com/rummik/nixos-config)
- [Eric Bailey](https://github.com/yurrriq/dotfiles)
- [Martin Baillie](https://github.com/martinbaillie/dotfiles)
- [Alex Ermolov](https://github.com/wiedzmin/nixos-config)
- [Bastian Kocher](https://github.com/bkchr/nixos-config)
- [Structured flake-based NixOS configuration by Tony O](https://github.com/bqv/nixrc)
- [chessai](https://github.com/chessai/nixos-configs)
- [Bruno Bigras](https://github.com/bbigras/nix-config)
- [Thomas Honeyman](https://github.com/thomashoneyman/.dotfiles)
- [Jorg Thalheim](https://github.com/Mic92/dotfiles)
- [nixcfg](https://github.com/colemickens/nixcfg) - NixOS and Home-Manager configurations.
- [Julius Bruijn](https://github.com/pimeys/nixos)
- [Michael Lingelbach](https://github.com/mjlbach/nix-dotfiles)
- [Thiago Okada](https://github.com/thiagokokada/nix-configs)
- [Pablo Corral](https://github.com/pinpox/nixos)
- [jkachmar](https://github.com/jkachmar/dotnix)
- [Xe](https://github.com/Xe/nixos-configs)
- [Eric Dallo](https://github.com/ericdallo/dotfiles)
- [Matthew Croughan](https://github.com/MatthewCroughan/nixcfg)
- [fortune](https://github.com/fortuneteller2k/nix-config) - NixOS configuration spawned from madness (home-manager and system).
- [Dov Alperin](https://github.com/DAlperin/dotfiles)
- [May Niklas](https://github.com/MayNiklas/nixos)
- [Victor Freire](https://github.com/ratsclub/dotfiles)
- [Kevin Amado](https://github.com/kamadorueda/machine)
- [Magnus Aasrud](https://github.com/kmaasrud/dotfiles)
- [Bernardo Meurer](https://github.com/lovesegfault/nix-config)
- [Riccardo Mazzarini](https://github.com/noib3/dotfiles)
- [David Farley](https://github.com/dwf/dotfiles)

## Nix configs (macOS)

- [Calum MacRae](https://github.com/cmacrae/config)
- [John Wiegley](https://github.com/jwiegley/nix-config)
- [LnL7](https://github.com/LnL7/dotfiles)
- [Tom's nix-configs](https://github.com/nocoolnametom/nix-configs)
- [Phil Pluckthun](https://github.com/kitten/nix-system)
- [Nix-Darwin-Dotfiles](https://github.com/shaunsingh/nix-darwin-dotfiles)
- [Malo Bourgon](https://github.com/malob/nixpkgs)

## Notes

- [Even if you curate your system, it gathers dust: configuration files left to rot, manually installed packages that didn't get uninstalled properly, orphaned packages difficult to track down... You could argue that it shouldn't happen in the first place, but that actually takes discipline. In NixOS, this is managed for you. Once you do nixos collect-garbage -d, you know that your system is only left with what it needs. Nothing more, nothing less.](https://www.reddit.com/r/NixOS/comments/441ymh/nixos_users_tell_me_what_are_the_cons/czmu9lo/)
- [Many server security best practices are cheap or free by virtue of using NixOS.](https://twitter.com/GabrielG439/status/1408181256160903170)

## Links

- [PhD thesis on nixOS](https://nixos.org/~eelco/pubs/phd-thesis.pdf)
- [Search NixOS options](https://nixos.org/nixos/options.html#)
- [Notes on nixOS package manager](https://yoshuawuyts.gitbooks.io/knowledge/content/bin/nix.html)
- [Why nixOS?](https://www.reddit.com/r/NixOS/comments/8bxdyu/why_nixos/)
- [Not OS](https://github.com/cleverca22/not-os) - Operating system generator, based on NixOS, that, given a config, outputs a small (47 MB), read-only squashfs for a runit-based operating system, with support for iPXE and signed boot.
- [NixOS 💜 Chromebook?](https://sphalerite.org/ghotl/posts/2017-11-10-chromebook.html)
- [NixOS Wiki](https://nixos.wiki/wiki/Main_Page)
- [NixOps](https://github.com/NixOS/nixops) - NixOS-based cloud deployment tool.
- [NixOS Discourse forum](https://discourse.nixos.org/)
- [Getting started with NixOS on Raspberry Pi 3 Model B+](https://github.com/zupo/nix)
- [Collection of NixOS image builders](https://github.com/nix-community/nixos-generators) - Allows to take the same NixOS configuration, and generate outputs for different target formats.
- [HN: Guix An advanced operating system (2019)](https://news.ycombinator.com/item?id=18902823)
- [NixOS on ARM](https://github.com/illegalprime/nixos-on-arm) - WIP to cross compile NixOS to run on ARM targets.
- [Arion](https://github.com/hercules-ci/arion) - Run docker-compose with help from Nix/NixOS.
- [Morph](https://github.com/DBCDK/morph) - Tool for managing existing NixOS hosts.
- [Mobile NixOS](https://github.com/samueldr/mobile-nixos) - Goal is to get a nix-built operating system, preferably NixOS running on mobile devices, e.g. Android phones.
- [Anyone using NixOS as main desktop (2019)](https://www.reddit.com/r/NixOS/comments/eb5nxv/anyone_using_nixos_as_main_destkop/)
- [NixOS: For developers (2020)](https://myme.no/posts/2020-01-26-nixos-for-development.html) ([Lobsters](https://lobste.rs/s/jevfaf/nixos_for_developers))
- [nixos-shell](https://github.com/Mic92/nixos-shell) - Spawns lightweight nixos vms in a shell.
- [Erase your darlings (2020)](https://grahamc.com/blog/erase-your-darlings) ([HN](https://news.ycombinator.com/item?id=22856199)) ([Lobsters](https://lobste.rs/s/2ayklq/erase_your_darlings_immutable))
- [Building a web app with functional programming - NixOS (2020)](https://blog.patchgirl.io/nixos/2020/03/31/nixos.html) ([HN](https://news.ycombinator.com/item?id=22877355))
- [nixos-manager](https://github.com/pmiddend/nixos-manager) - Manage your NixOS graphically.
- [Search NixOS packages and options](https://search.nixos.org/) ([Code](https://github.com/NixOS/nixos-search))
- [My NixOS Desktop Flow (2020)](https://christine.website/blog/nixos-desktop-flow-2020-04-25) ([HN](https://news.ycombinator.com/item?id=22984639)) ([Lobsters](https://lobste.rs/s/yb1oqg/my_nixos_desktop_flow))
- [Is NixOS Reproducible?](https://r13y.com/) ([Code](https://github.com/grahamc/r13y.com))
- [Impermanence](https://github.com/nix-community/impermanence) - Modules to help you handle persistent state on systems with ephemeral root storage.
- [NixOS Weekly Newsletter](https://weekly.nixos.org/) - Stay up to date with events, learning resources, and recent developments in NixOS community. ([Code](https://github.com/NixOS/nixos-weekly))
- [Nix Community Infrastructure](https://github.com/nix-community/infra)
- [NixOS: How it works and how to install it (2020)](https://www.youtube.com/watch?v=oPymb2-IXbg)
- [Nix(OS) Thoughts (2020)](https://blog.qtp2t.club/posts/2020-06-20-nix-nixos-thoughts/) ([Lobsters](https://lobste.rs/s/iy17mo/nix_os_thoughts))
- [Lightweight Linux VMs on NixOS (2020)](https://www.srid.ca/2012301.html)
- [adhoc executable patching on nixos (2020)](https://notes.neeasade.net/adhoc-executable-patching-on-nix.html)
- [Nix Flakes: Managing NixOS systems (2020)](https://www.tweag.io/blog/2020-07-31-nixos-flakes/)
- [NixOS Channels (2020)](https://nixos.online/posts/NixOS_channels/)
- [Building and Importing NixOS AMIs on EC2 (2020)](http://jackkelly.name/blog/archives/2020/08/30/building_and_importing_nixos_amis_on_ec2/)
- [Tailscale is magic; even more so with NixOS (2020)](https://fzakaria.com/2020/09/17/tailscale-is-magic-even-more-so-with-nixos.html)
- [Secure, Declarative Key Management with NixOps, Pass, and nix-plugins (2018)](https://elvishjerricco.github.io/2018/06/24/secure-declarative-key-management.html)
- [nixos-install-scripts](https://github.com/nix-community/nixos-install-scripts) - Collection of one-shot scripts to install NixOS on various server hosters and other hardware.
- [NixOS on prgmr and Failing to Learn Nix (2018)](https://push.cx/2018/nixos) ([Lobsters](https://lobste.rs/s/qpbohs/nixos_on_prgmr_failing_learn_nix_2018))
- [Eight Months of NixOS (2020)](https://catgirl.ai/log/nixos-experience/) ([Lobsters](https://lobste.rs/s/7eq5qv/eight_months_nixos))
- [One Week of NixOS (2020)](https://jae.moe/blog/2020/11/one-week-of-nixos/) ([HN](https://news.ycombinator.com/item?id=25024639)) ([Lobsters](https://lobste.rs/s/b7hjcy/one_week_nixos))
- [Nixops Services on Your Home Network (2020)](https://christine.website/blog/nixops-services-2020-11-09) ([Lobsters](https://lobste.rs/s/kzforn/nixops_services_on_your_home_network))
- [sops-nix](https://github.com/Mic92/sops-nix) - Atomic secret provisioning for NixOS based on sops.
- [NixOS infrastructure configurations](https://github.com/NixOS/nixos-org-configurations)
- [nix-ld](https://github.com/Mic92/nix-ld) - Run unpatched dynamic binaries on NixOS.
- [Nix(OS) Thoughts (2020)](https://blog.knightsofthelambdacalcul.us/posts/2020-06-20-nix-nixos-thoughts/) ([Lobsters](https://lobste.rs/s/m3j4yn/nix_os_thoughts))
- [NixOps AWS Plugin](https://github.com/NixOS/nixops-aws) - Tool for deploying NixOS machines in a network or cloud.
- [nixflk](https://github.com/nrdxp/nixflk) - Highly structured NixOS configuration database.
- [NixOS Pre Installer](https://github.com/alexandergall/nixos-pxe-installer) - Set of modules to perform a fully automated installation of a customized NixOS system.
- [krops](https://github.com/krebs/krops) - Lightweight toolkit to deploy NixOS systems, remotely or locally.
- [TangeriNixOS](https://github.com/Pamplemousse/tangerinixos) - NixOS tailored for pentesting.
- [Methods for building custom NixOS AMIs](https://github.com/nh2/nixos-ami-building)
- [Colmena](https://github.com/zhaofengli/colmena) - Simple, stateless NixOS deployment tool modeled after NixOps and Morph, written in Rust.
- [NixOS in the Cloud, step-by-step (2020)](https://justinas.org/nixos-in-the-cloud-step-by-step-part-1)
- [Mayflower Nix Consulting](https://nixos.mayflower.consulting/)
- [agenix](https://github.com/ryantm/agenix) - age-encrypted secrets for NixOS.
- [nix-autobahn](https://github.com/Lassulus/nix-autobahn) - Allows you to download ELF binaries and use them right away in NixOS.
- [Why isn't NixOS more popular (2021)](https://www.reddit.com/r/NixOS/comments/kpntby/why_isnt_nixos_more_popular/)
- [Server-optimized NixOS](https://github.com/arianvp/server-optimised-nixos) - Distribution inspired by NixOS, ChromeOS, Container Optimised Linux and Container Linux. Opinionated, server-first distribution.
- [HN: NixOS Linux (2021)](https://news.ycombinator.com/item?id=25718098)
- [NixOps backend for Google Cloud](https://github.com/nix-community/nixops-gce) - Tool for deploying NixOS machines in a network or cloud.
- [Nixus](https://github.com/Infinisil/nixus) - Experimental deployment tool for multiple NixOS systems.
- [nixos.org website code](https://github.com/NixOS/nixos-homepage)
- [Encrypted Secrets with NixOS (2021)](https://christine.website/blog/nixos-encrypted-secrets-2021-01-20) ([Lobsters](https://lobste.rs/s/gur8yy/encrypted_secrets_with_nixos))
- [Offloading NixOS builds to a faster machine (2021)](https://sgt.hootr.club/molten-matter/nix-distributed-builds/)
- [Why you should never ever use NixOS (2021)](https://hands-on.cloud/why-you-should-never-ever-use-nixos/) ([Lobsters](https://lobste.rs/s/f6i7g0/why_you_should_never_ever_use_nixos)) ([HN](https://news.ycombinator.com/item?id=25881654))
- [NixOS on Raspberry Pi](https://github.com/lucernae/nixos-pi)
- [Learning nix workshop](https://github.com/spacekookie/nixos-workshops)
- [Using NixOS as a router (2021)](https://francis.begyn.be/blog/nixos-home-router)
- [Immutable Systems Infrastructure, or how to mashup Kubernetes and Nix](https://tevps.net/blog/2021/2/20/immutable-systems-infrastructure-or-how-mashup-kub/) ([Lobsters](https://lobste.rs/s/h8ejms/immutable_systems_infrastructure_how))
- [NixOS Flake Example](https://github.com/colemickens/nixos-flake-example) - Demo NixOS config, with optional flakes support. Along with notes on why flakes is useful and worth adopting.
- [Bitte](https://github.com/input-output-hk/bitte) - Nix Ops for Terraform, Consul, Vault, Nomad.
- [nixos-up](https://github.com/samuela/nixos-up) - Fastest NixOS install there is.
- [Declarative Docker Container Service in NixOS (2020)](https://www.breakds.org/post/declarative-docker-in-nixos/)
- [Using Morph for Deploying to NixOS (2021)](https://christine.website/blog/morph-setup-2021-04-25)
- [Show me what you run (2021)](https://blog.superbaloo.net/posts/show-me-what-you-run/)
- [List of companies using NixOS technologies](https://discourse.nixos.org/t/list-of-companies-using-nixos-technologies/8428)
- [DevOS](https://devos.divnix.com/) - Simple template to use, deploy and manage NixOS systems for personal and productive use. ([Code](https://github.com/divnix/devos)) ([GitHub](https://github.com/divnix))
- [NixOS 21.05 (2021)](https://nixos.org/manual/nixos/stable/release-notes.html#sec-release-21.05) ([HN](https://news.ycombinator.com/item?id=27368361)) ([Lobsters](https://lobste.rs/s/iaxedy/nixos_21_05_released))
- [Nixkite](https://github.com/input-output-hk/nixkite) - Buildkite pipeline generation tool using the NixOS module system.
- [HN: NixOS-unstable’s ISO_minimal.x86_64-Linux is 100% reproducible (2021)](https://news.ycombinator.com/item?id=27573393)
- [MicroVM.nix](https://github.com/astro/microvm.nix) - Nix Flake to build NixOS and run it on one of several Type-2 Hypervisors.
- [Paranoid NixOS Setup (2021)](https://christine.website/blog/paranoid-nixos-2021-07-18) ([Lobsters](https://lobste.rs/s/dn4jss/paranoid_nixos_setup))
- [NixOS Ocean Sprint](https://oceansprint.org/)
- [NixOS on the Framework (2021)](https://grahamc.com/blog/nixos-on-framework)
- [NixOS-Infect](https://github.com/elitak/nixos-infect) - Script to install NixOS on non-NixOS hosts.
- [Application Isolation using NixOS Containers (2021)](https://msucharski.eu/posts/application-isolation-nixos-containers/)
- [Mobile NixOS](https://github.com/NixOS/mobile-nixos) - Superset on top of NixOS Linux, Nixpkgs and Nix, aiming to abstract away the differences between mobile devices. ([Web](https://mobile.nixos.org/))
- [NixOS Beginner's Handbook](https://github.com/kstenerud/nixos-beginners-handbook)
- [Template for developing/testing NixOS modules](https://github.com/ngi-nix/nixos-modules-flake-template)
- [Deploying a NixOS configuration into a QEMU VM (2020)](https://alpmestan.github.io/notes/nixos-qemu.html)
- [NixOS on underpowered devices (2021)](https://eno.space/blog/2021/08/nixos-on-underpowered-devices)
- [nix-netboot-serve](https://github.com/DeterminateSystems/nix-netboot-serve) - Make any NixOS system netbootable with 30s cycle times.
- [Nix-Gui](https://github.com/nix-gui/nix-gui) - Make NixOS usable for non-technical users through a settings / package management GUI. ([HN](https://news.ycombinator.com/item?id=28817477))
- [NixOS Configuration with Flakes (2021)](https://jdisaacs.com/blog/nixos-config/)
- [Google Cloud “GCP” native NixOS images build (2021)](https://mudrii.medium.com/google-cloud-gcp-native-nixos-images-build-16f77a412bb7)
- [NixOS Matrix Chat](https://matrix.to/#/#community:nixos.org)
- [How I started with NixOS (2021)](https://gianarb.it/blog/how-i-started-with-nixos) ([Reddit](https://www.reddit.com/r/NixOS/comments/q77m1y/how_i_started_with_nixos/))
- [NixOS and the Art of OS Configuration (2018)](https://www.rousette.org.uk/archives/nixos-and-the-art-of-os-configuration/) ([HN](https://news.ycombinator.com/item?id=28884609))
- [nix-simple-deploy](https://github.com/misuzu/nix-simple-deploy) - Deploy software or an entire NixOS system configuration to another NixOS system.
- [Flying Circus NixOS Platform](https://github.com/flyingcircusio/fc-nixos)
- [Low-footprint NixOS images](https://github.com/lourkeur/miniguest)
- [nix-alien](https://github.com/thiagokokada/nix-alien) - Run unpatched binaries on Nix/NixOS.
- [extra-container](https://github.com/erikarvstedt/extra-container) - Run declarative NixOS containers without full system rebuilds.
- [nix-autobahn](https://github.com/wucke13/nix-autobahn)
- [homeage](https://github.com/jordanisaacs/homeage) - Module for home-manager that enables runtime decryption of declarative age files.
- [How Nix and NixOS Get So Close to Perfect (2021)](https://christine.website/talks/nixos-pain-2021-11-10) ([Lobsters](https://lobste.rs/s/ff54p1/how_nix_nixos_get_so_close_perfect)) ([HN](https://news.ycombinator.com/item?id=31141377))
- [NixOps is easier than I thought (2021)](https://sgt.hootr.club/molten-matter/nixops-on-the-pi/)
- [Nix System Configuration](https://github.com/kclejeune/system) - Declarative system configurations using nixOS, nix-darwin, and home-manager.
- [bootspec](https://github.com/DeterminateSystems/bootspec) - Research project that aims to improve the bootloader story in NixOS.
- [NixOS: Headless Home Assistant VM (2021)](https://myme.no/posts/2021-11-25-nixos-home-assistant.html) ([Lobsters](https://lobste.rs/s/xi9jcs/nixos_headless_home_assistant_vm))
- [Attempts to get NixOS up on M1 Macs](https://github.com/tpwrules/nixos-m1)
- [NixOS aarch64 images](https://github.com/Mic92/nixos-aarch64-images)
- [M1 dev setup using a NixOS virtual machine (2021)](https://calcagno.blog/m1dev/)
- [nixos-gen-config](https://github.com/nix-community/nixos-gen-config)
- [A second look at NixOS (2022)](https://psibi.in/posts/2022-01-01-nixos.html)
- [deploy](https://github.com/winterqt/deploy) - Yet another NixOS deployment tool.
- [Nixinate](https://github.com/MatthewCroughan/nixinate) - NixOS Deployment Tool. Generates a deployment script for each nixosConfiguration you already have in your flake.
- [NixOS: The Ultimate Dev Environment? (2022)](https://myme.no/posts/2022-01-16-nixos-the-ultimate-dev-environment.html) ([Lobsters](https://lobste.rs/s/pwrni4/nixos_ultimate_dev_environment))
- [The Curse of NixOS (2022)](https://blog.wesleyac.com/posts/the-curse-of-nixos) ([HN](https://news.ycombinator.com/item?id=30057287)) ([Lobsters](https://lobste.rs/s/psfsfo/curse_nixos))
- [How I set up a NixOS router with VPN and split routing (2021)](https://pavluk.org/blog/2021/01/26/nixos_router.html) ([Reddit](https://www.reddit.com/r/NixOS/comments/sdsznj/how_i_set_up_a_nixos_router_with_vpn_and_split/))
- [Declarative container images with Nix](https://github.com/cloudwatt/nix-container-images) - Write container images as NixOS machines.
- [Building a Philosophy Workstation with NixOS: Installing Firefox, VSCodium, and LaTeX (2022)](https://shen.hong.io/nixos-for-philosophy-installing-firefox-latex-vscodium/)
- [nix-deploy](https://github.com/awakesecurity/nix-deploy) - Deploy software or an entire NixOS system configuration to another NixOS system.
- [macOS to NixOS the Purely Functional Linux Distribution by Daniel Britten (2022)](https://www.youtube.com/watch?v=SzFn7UwVws0)
- [Remote, encrypted ZFS storage server with NixOS (2022)](https://mazzo.li/posts/hetzner-zfs.html)
- [Plex on NixOS (2022)](https://arne.me/blog/plex-on-nixos/) ([Lobsters](https://lobste.rs/s/jyoukv/plex_on_nixos))
- [NixNG](https://github.com/MagicRB/NixNG) - GNU/Linux distribution, which may be a considered a late sibling to NixOS.
- [RPATH, or why lld doesn’t work on NixOS (2022)](https://matklad.github.io//2022/03/14/rpath-or-why-lld-doesnt-work-on-nixos.html) ([HN](https://news.ycombinator.com/item?id=30688815))
- [Toy highly-available Kubernetes cluster on NixOS](https://github.com/justinas/nixos-ha-kubernetes)
- [Vulnix](https://github.com/flyingcircusio/vulnix) - Vulnerability (CVE) scanner for Nix/NixOS.
- [ninomicro](https://github.com/rcoder/ninodevm) - NixOS + Nomad + Deno + Microvm.
- [NixOS tutorial: one hour, hands-on](https://github.com/brainrake/nixos-tutorial)
- [Operating systems battle: OpenBSD vs. NixOS (2022)](https://dataswamp.org/~solene/2022-04-18-openbsd-vs-nixos.html) ([HN](https://news.ycombinator.com/item?id=31075570))