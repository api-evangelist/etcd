---
title: "Avoiding Zombie Cluster Members When Upgrading to etcd v3.6"
url: "https://etcd.io/blog/2025/zombie_members_upgrade/"
date: "Wed, 17 Dec 2025 00:00:00 +0000"
author: ""
feed_url: "https://etcd.io/blog/index.xml"
---
<p><strong>Summary: SIG-etcd has patched another potential issue blocking upgrades from v3.5 to v3.6. If you are upgrading, make sure to update to <a href="https://github.com/etcd-io/etcd/releases/tag/v3.5.26" rel="noopener" target="_blank">v3.5.26</a> or later first.</strong></p>
<h2 id="issue-summary">Issue Summary</h2>
<p>Recently, the etcd community addressed an issue that may appear when users <a href="https://etcd.io/docs/v3.6/upgrades/upgrade_3_6/" rel="noopener" target="_blank">upgrade from v3.5 to v3.6</a>. This bug can cause the cluster to report &ldquo;zombie members&rdquo;, which are etcd nodes that were removed from the database cluster some time ago, and are re-appearing and joining database consensus. The etcd cluster is then inoperable until these zombie members are removed.</p>
