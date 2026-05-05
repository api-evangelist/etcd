---
title: "Announcing etcd-operator v0.2.0"
url: "https://etcd.io/blog/2026/announcing-etcd-operator-v0.2.0/"
date: "Fri, 20 Mar 2026 00:00:00 +0000"
author: ""
feed_url: "https://etcd.io/blog/index.xml"
---
<h2 id="introduction">Introduction</h2>
<p>Today, we are excited to announce the release of <a href="https://github.com/etcd-io/etcd-operator/releases/tag/v0.2.0" rel="noopener" target="_blank">etcd-operator v0.2.0</a>! This release brings important
new features and improvements that enhance security, reliability, and operability for managing etcd clusters.</p>
<h2 id="new-features">New Features</h2>
<h3 id="certificate-management">Certificate Management</h3>
<p>Version 0.2.0 introduces built-in certificate management to secure all TLS communication:</p>
<ul>
<li>Between etcd members (inter-member communication)</li>
<li>Between clients and etcd members</li>
</ul>
<p>TLS is only configured when explicitly enabled by the user. Once enabled, etcd-operator automatically
provisions and manages certificates based on the selected provider.</p>
