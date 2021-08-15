---
id: yz7BaxKE7IssV5Go
title: Module
desc: ''
updated: 1629041014644
created: 1627924831114
---

## Summary
- status: WIP

This describes the [module schema](module.schema.yml) in more detail. Modules are anything that encapsulate logic with software. They cover everything enmerated in `module.schema`. 

The module schema is meant to be used as part of other schemas. For example, in the template vault, it is used in both `pkg.schema` and `service.schema`. This is because both packages (eg. React, NextJS, etc) and services (eg. AWS S3, Github, Stripe, etc) share the same underlying structure (eg. quickstart, concepts, architecture, lifecycles, etc)


## Nodes

### architecture
- alias: arch

This goes over the general architecture.

This should include:
- [ ] mermaid diagram of major lifecylce events (eg. startup, shutdown, main feature) and components
- [ ] paragraph about major lifecycle events and components

An archietcture node can have children if it exceeds 800 words. At that point, every lifecycle/component can be a direct child 

### concepts
- example: [[Concepts|dendron.concepts]]

Any terms or concepts we should understand

### dev

This goes into specifics of the development process

#### quickstart

This goes into how to get started developing this module

- Sections:
  - Pre-Req: what is needed before you start
  - Steps: How to setup the project for development

### faq

Any commonly asked questions can be put here

### ops
- example: [[Ops|pkg.dendron-plugin.ops]]

How do we diagnose problems with this module.

### qa

How do we maintain quality assurance on this module

#### test

How do we functionally test that everything is correct

#### performance

How do we test that the performance is sufficient?

### quickstart
- example: [[Quickstart|pkg.dendron-plugin.quickstart]]

How do we get started with the module as a user

### topic
- namespace: true

This is for any major component of the module and might be a module itself.


