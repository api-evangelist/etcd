---
title: "Announcing etcd v3.6.0"
url: "https://etcd.io/blog/2025/announcing-etcd-3.6/"
date: "Thu, 15 May 2025 00:00:00 +0000"
author: ""
feed_url: "https://etcd.io/blog/index.xml"
---
<h2 id="table-of-contents">Table of Contents</h2>
<ul>
<li><strong><a href="#introduction">Introduction</a></strong></li>
<li><strong><a href="#security">Security</a></strong></li>
<li><strong><a href="#features">Features</a></strong>
<ul>
<li><a href="#migration-to-v3store">Migration to v3store</a></li>
<li><a href="#downgrade">Downgrade</a></li>
<li><a href="#feature-gates">Feature Gates</a></li>
<li><a href="#livezreadyz-checks">Livez/readyz checks</a></li>
<li><a href="#v3discovery">v3discovery</a></li>
</ul>
</li>
<li><strong><a href="#performance">Performance</a></strong>
<ul>
<li><a href="#memory">Memory</a></li>
<li><a href="#throughput">Throughput</a></li>
</ul>
</li>
<li><strong><a href="#breaking-changes">Breaking changes</a></strong>
<ul>
<li><a href="#old-binaries-are-incompatible-with-new-schema-versions">Old Binaries Are Incompatible with New Schema Versions</a></li>
<li><a href="#peer-endpoints-no-longer-serve-client-requests">Peer Endpoints No Longer Serve Client Requests</a></li>
<li><a href="#clear-boundary-between-etcdctl-and-etcdutl">Clear boundary between etcdctl and etcdutl</a></li>
</ul>
</li>
<li><strong><a href="#testing">Testing</a></strong></li>
<li><strong><a href="#critical-bug-fixes">Critical bug fixes</a></strong></li>
<li><strong><a href="#upgrade-issue">Upgrade issue</a></strong></li>
<li><strong><a href="#platforms">Platforms</a></strong></li>
<li><strong><a href="#dependencies">Dependencies</a></strong>
<ul>
<li><a href="#dependency-bumping-guide">Dependency Bumping Guide</a></li>
<li><a href="#core-dependency-updates">Core Dependency Updates</a></li>
<li><a href="#grpc-gatewayv2">grpc-gateway@v2</a></li>
<li><a href="#grpc-ecosystemgo-grpc-middlewareprovidersprometheus">grpc-ecosystem/go-grpc-middleware/providers/prometheus</a></li>
</ul>
</li>
<li><strong><a href="#community">Community</a></strong>
<ul>
<li><a href="#etcd-becomes-a-kubernetes-sig">etcd Becomes a Kubernetes SIG</a></li>
<li><a href="#new-contributors-maintainers-and-reviewers">New Contributors, Maintainers, and Reviewers</a></li>
<li><a href="#new-release-team">New Release Team</a></li>
<li><a href="#introducing-the-etcd-operator-working-group">Introducing the etcd Operator Working Group</a></li>
</ul>
</li>
<li><strong><a href="#extended-support-for-v34">Extended Support for v3.4</a></strong></li>
<li><strong><a href="#future-development">Future Development</a></strong></li>
</ul>
<h2 id="introduction">Introduction</h2>
<p>Today, we are releasing <a href="https://github.com/etcd-io/etcd/releases/tag/v3.6.0" rel="noopener" target="_blank">etcd v3.6.0</a>, the first minor release since etcd v3.5.0 on June 15, 2021. This release
introduces several new features, makes significant progress on long-standing efforts like downgrade support and
migration to v3store, and addresses numerous critical &amp; major issues. It also includes major optimizations in
memory usage, improving efficiency and performance.</p>
