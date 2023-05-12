---
title: "PBC Yokozuna Index Delete"
description: ""
project: "riak_kv"
project_version: 3.0.10
menu:
  riak_kv-3.0.10:
    name: "Yokozuna Index Delete"
    identifier: "pbc_yz_index_delete"
    weight: 122
    parent: "apis_pbc"
toc: true
aliases:
  - /riak/3.0.10/dev/references/protocol-buffers/yz-index-delete
  - /riak/kv/3.0.10/dev/references/protocol-buffers/yz-index-delete
---

Delete a search index.

## Request

The `name` parameter is the name of the index to delete, as a binary.

```protobuf
message RpbYokozunaIndexDeleteReq {
    required bytes name  =  1;
}
```

## Response

Returns a [RpbDelResp]({{<baseurl>}}riak/kv/3.0.10/developing/api/protocol-buffers/#message-codes) code with no data on success.





