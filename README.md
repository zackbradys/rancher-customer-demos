---
title: Rancher Demos Apps with Fleet
author: Zack Brady - Field Engineer
contact: zack.brady@rancherfederal.com
---

# Rancher Demo Applications with Rancher Fleet

### Table of Contents
* [About Me](#about-me)
* [Configuration](#configuration)
* [Extras](#extras)

## About Me

A little bit Zack Brady, his history, and what he's done in the industry. 
- DOD/IC Contractor
- U.S. Military Veteran
- Open-Source Contributor
- Built and Exited a Digital Firm
- Active Volunteer Firefighter/EMT

## Configuration

```bash
kubectl apply -f https://raw.githubusercontent.com/zackbradys/rancher-customer-demos/main/fleet.yaml
```

## Extras

Currently there is a bug within Fleet ([rancher/fleet#759](https://github.com/rancher/fleet/issues/759)). Please use this fix:

```bash
kubectl patch ClusterGroup -n fleet-local default --type=json -p='[{"op": "remove", "path": "/spec/selector/matchLabels/name"}]'
```
