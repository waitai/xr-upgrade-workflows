# xr-upgrade-workflows
A set of CWM workflows for upgrading a single OS image of IOS-XR (LNT Flavor) devices.  The CWM workflows interact with NSO via the IOS-XR NETCONF NED to perform the pre-check, image upgrade and post-check.  The workflows are defined in [CNCF's Serverless Workflow DSL Specification](https://github.com/serverlessworkflow/specification/blob/0.9.x/specification.md).

More documentation to come.

## Table of contents

- [Introduction](#introduction)
- [Prerequisites](#prerequisites)

## Introduction

Cisco's Crosswork Workflow Manager (CWM) enables customers to build their own automation workflows, with capabilities to integrate to existing Operations Support Systems (OSS) and Business Support Systems (BSS) within their environment. These integrations are achieved through the use of adapters.

Together with Cisco's Network Service Orchestrator (NSO), CWM allows ease of automating change management for your network.  It also enables the automation of Router OS upgrade for your network devices.

The xr-upgrade-workflow project demonstrates how a set of child workflows that were developed with assistance from GitHub Copilot can be stitched together into a parent workflow (invoke-xr-upgrade) for orchestrating the end-to-end IOS-XR OS image upgrade process including pre-check, upgrade (distribute, activiate, commit), and post-check.

## Prerequisites
- [**CWM** 1.2 installed using OVA](https://www.cisco.com/c/en/us/td/docs/net_mgmt/cisco_workflow/AdministratorGuide1-2/b_administrator-guide11/m_install-cwm-using-ova_1-1.html)
  - NSO adapter
- **NSO** install
