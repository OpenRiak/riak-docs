---
title: "HTTP Search Index Info"
description: ""
project: "riak_kv"
project_version: 2.9.8
menu:
  riak_kv-2.9.8:
    name: "Search Index Info"
    identifier: "http_search_index_info"
    weight: 114
    parent: "apis_http"
toc: true
aliases:
  - /riak/2.9.8/dev/references/http/search-index-info
  - /riak/kv/2.9.8/dev/references/http/search-index-info
---

Retrieves information about all currently available [Search indexes]({{<baseurl>}}riak/kv/2.9.8/developing/usage/search) in JSON format.

## Request

```
GET /search/index
```

## Response

If there are no currently available Search indexes, a `200 OK` will be
returned but with an empty list as the response value.

Below is the example output if there is one Search index, called
`test_index`, currently available:

```json
[
  {
    "n_val": 3,
    "name": "test_index",
    "schema": "_yz_default"
  }
]
```

#### Normal Response Codes

* `200 OK`

#### Typical Error Codes

* `404 Object Not Found`
  - /riak/latest/developing/api/http/search-index-info/
  - /riak/kv/latest/developing/api/http/search-index-info/
  - /riakkv/latest/developing/api/http/search-index-info/
---
Typically returned if Riak Search is not
    currently enabled on the node
* `503 Service Unavailable`
  - /riak/latest/developing/api/http/search-index-info/
  - /riak/kv/latest/developing/api/http/search-index-info/
  - /riakkv/latest/developing/api/http/search-index-info/
---
The request timed out internally




