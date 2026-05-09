---
title: "May 1 Security Release Patches RBAC Bypass in Transactions"
url: "https://etcd.io/blog/2026/may-patch-release/"
date: "2026-05-04"
author: ""
feed_url: "https://etcd.io/blog/index.xml"
---
SIG-etcd released updates v3.6.11, v3.5.30, and v3.4.44 today. These patch releases fix a vulnerability that allows an authenticated user to bypass RBAC authorization checks when reading data via PrevKv or attaching leases inside Put requests nested in etcd transactions. In addition, v3.6.11 and v3.5.30 contain a bug fix for an issue that prevented adding a new member when one member was down, even though quorum was still satisfied. This vulnerability does not affect etcd as a part of the Kubernetes Control Plane.
