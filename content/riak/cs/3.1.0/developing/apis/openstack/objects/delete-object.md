---
title_supertext: "APIs > OpenStack > Objects"
title: "Delete an Object"
description: ""
menu:
  riak_cs-3.1.0:
    name: "Delete"
    identifier: "develop_apis_openstack_objects_delete"
    weight: 103
    parent: "develop_apis_openstack_objects"
project: "riak_cs"
project_version: "3.1.0"
aliases:
  - /riakcs/3.1.0/references/apis/storage/openstack/RiakCS-OpenStack-Delete-Object
  - /riak/cs/3.1.0/references/apis/storage/openstack/RiakCS-OpenStack-Delete-Object
  - /riakcs/3.1.0/references/apis/storage/openstack/delete-object
  - /riak/cs/3.1.0/references/apis/storage/openstack/delete-object
---

Removes the specified object, if it exists.

## Requests

### Request Syntax

```http
DELETE /<api version>/<account>/<container>/<object> HTTP/1.1
Host: data.basho.com
X-Auth-Token: auth_token
```

## Responses

This operation does not return a response.

## Examples

### Sample Request

The following request deletes the object `basho-process.jpg` from the container `basho-docs`.

```http
DELETE /v1.0/deadbeef/basho-docs/basho-process.jpg HTTP/1.1
Host: data.basho.com
Date: Fri, 01 Jun  2012 12:00:00 GMT
X-Auth-Token: aaaaaaaa-aaaa-aaaa-aaaa-aaaaaaaaaaaa
```

### Sample Response

```http
HTTP/1.1 204 No Content
Date: Wed, 06 Jun 2012 20:47:15 GMT
Connection: close
Server: RiakCS
```
