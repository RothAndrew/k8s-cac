# Docker Desktop -- Rancher

Deploy Rancher on Docker Desktop in one step!

Roughly follows [this guide](https://rancher.com/blog/2018/2018-05-18-how-to-run-rancher-2-0-on-your-desktop/) (updated for 2020) by deploying nginx-ingress and cert-manager, then Rancher.

## Instructions

1. Clone this repo
1. `cd` into this directory
1. `helmfile apply`
1. Rancher is available at [https://rancher.localhost](https://rancher.localhost). Not sure why, but it didn't work for me on Firefox. Chrome worked fine.

## Other Notes

- Don't forget to increase CPU and Memory. You'll quickly run out, especially if you start deploying other apps from Rancher like Prometheus/Grafana, Istio, EFK, etc.
- The Kubernetes page in Docker Desktop preferences has a "reset cluster" button you can use to blow the cluster away and start fresh if you want to.