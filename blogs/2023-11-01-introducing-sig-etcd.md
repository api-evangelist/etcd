---
title: "Introducing sig-etcd"
url: "https://etcd.io/blog/2023/introducing-sig-etcd/"
date: "Wed, 01 Nov 2023 00:00:00 +0000"
author: ""
feed_url: "https://etcd.io/blog/index.xml"
---
<p>Special Interest Groups (SIGs) are a fundamental part of the Kubernetes project, with a substantial share of the community activity happening within them. When the need arises, <a href="https://github.com/kubernetes/community/blob/master/sig-wg-lifecycle.md" rel="noopener" target="_blank">new SIGs can be created</a>, and that was precisely what happened recently.</p>
<p><a href="https://github.com/kubernetes/community/blob/master/sig-etcd/README.md" rel="noopener" target="_blank">SIG etcd</a> is the most recent addition to the list of Kubernetes SIGs. In this article we will get to know it a bit better, understand its origins, scope, and plans.</p>
<h2 id="the-critical-role-of-etcd">The critical role of etcd</h2>
<p>If we look inside the control plane of a Kubernetes cluster, we will find <a href="https://kubernetes.io/docs/concepts/overview/components/#etcd" rel="noopener" target="_blank">etcd</a>, a consistent and highly-available key value store used as Kubernetes&rsquo; backing store for all cluster data -- this description alone highlights the critical role that etcd plays, and the importance of it within the Kubernetes ecosystem.</p>
