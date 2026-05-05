---
title: "Follow Up - Preventing Upgrade Failures from etcd v3.5 to v3.6"
url: "https://etcd.io/blog/2025/upgrade_from_3.5_to_3.6_issue_followup/"
date: "Tue, 21 Oct 2025 00:00:00 +0000"
author: ""
feed_url: "https://etcd.io/blog/index.xml"
---
<p>We have identified and fixed an additional scenario that may cause upgrade failures when
moving from etcd v3.5 to v3.6. This post contains details, the fix, and additional workarounds.
Please refer to issue <a href="https://github.com/etcd-io/etcd/issues/20793" rel="noopener" target="_blank">20793</a> to get detailed technical information.</p>
<h2 id="issue">Issue</h2>
<p>In a previous post — <a href="https://etcd.io/blog/2025/upgrade_from_3.5_to_3.6_issue/" rel="noopener" target="_blank">How to Prevent a Common Failure when Upgrading etcd v3.5 to v3.6</a> — we
described an upgrade issue affecting etcd versions in v3.5.1-v3.5.19. That issue was addressed in
v3.5.20. However, a follow-up investigation revealed that the original fix did not cover all scenarios.</p>
