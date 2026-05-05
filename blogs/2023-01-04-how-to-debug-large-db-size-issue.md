---
title: "How to debug large db size issue?"
url: "https://etcd.io/blog/2023/how_to_debug_large_db_size_issue/"
date: "Wed, 04 Jan 2023 00:00:00 +0000"
author: ""
feed_url: "https://etcd.io/blog/index.xml"
---
<h1 id="background">Background</h1>
<p>Users can configure the quota of the backend db size using flag <code>--quota-backend-bytes</code>. It&rsquo;s the max number of bytes
the etcd db file may consume, namely the ${etcd-data-dir}/member/snap/db file. Its default value is 2GB, and the
suggested max value is 8GB.</p>
<p>2GB is usually sufficient for most use cases. If you run out of the db quota, you will see error message <code>etcdserver: mvcc: database space exceeded</code>
when trying to write more data, and see alarm &ldquo;NOSPACE&rdquo; (see example below) when checking the endpoint status or health state. It would be better to figure out whether it&rsquo;s expected. It&rsquo;s exactly the reason why I provide this guide.</p>
