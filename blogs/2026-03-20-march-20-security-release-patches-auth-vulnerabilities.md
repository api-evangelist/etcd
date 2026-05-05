---
title: "March 20 Security Release Patches Auth Vulnerabilities"
url: "https://etcd.io/blog/2026/mar20-patch-release/"
date: "Fri, 20 Mar 2026 00:00:00 +0000"
author: ""
feed_url: "https://etcd.io/blog/index.xml"
---
<p>SIG-etcd released updates <a href="https://github.com/etcd-io/etcd/releases/tag/v3.6.9" rel="noopener" target="_blank">3.6.9</a>, <a href="https://github.com/etcd-io/etcd/releases/tag/v3.5.28" rel="noopener" target="_blank">3.5.28</a>, and <a href="https://github.com/etcd-io/etcd/releases/tag/v3.4.42" rel="noopener" target="_blank">3.4.42</a> today. These patch releases fix several vulnerabilities which allow unauthorized users to bypass authentication or authorization controls that are part of etcd Auth using the gRPC API.</p>
<p>These vulnerabilities do not affect etcd as a part of the Kubernetes Control Plane. They only affect etcd clusters in other contexts, specifically ones with Auth enabled where it is required for access control in untrusted or partially trusted networks or with untrused users.</p>
