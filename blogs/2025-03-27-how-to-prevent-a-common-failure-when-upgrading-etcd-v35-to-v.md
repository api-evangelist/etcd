---
title: "How to Prevent a Common Failure when Upgrading etcd v3.5 to v3.6"
url: "https://etcd.io/blog/2025/upgrade_from_3.5_to_3.6_issue/"
date: "Thu, 27 Mar 2025 00:00:00 +0000"
author: ""
feed_url: "https://etcd.io/blog/index.xml"
---
<div class="alert alert-primary"><div class="h4 alert-heading">Update (October 21, 2025)</div>
<p>We have identified and fixed two additional upgrade issues. Please see our
new blog posts
<a href="https://etcd.io/blog/2025/upgrade_from_3.5_to_3.6_issue_followup">Follow Up - Preventing Upgrade Failures from etcd v3.5 to v3.6</a> and <a href="https://etcd.io/blog/2025/zombie_members_upgrade">Avoiding Zombie Cluster Members When Upgrading</a>
for details.</p>
</div>
<p>There is a common issue <a href="https://github.com/etcd-io/etcd/issues/19557" rel="noopener" target="_blank">19557</a> in the etcd v3.5 to v3.6 upgrade that may cause the upgrade
process to fail. You can find detailed information and related discussions in the issue.</p>
<h2 id="tl-dr">TL; DR</h2>
<p>Users are required to first upgrade to etcd v3.5.20 (or a higher patch version) before upgrading
to etcd v3.6.0. Failure to do so may result in an unsuccessful upgrade.</p>
