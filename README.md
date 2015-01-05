Ansible Elasticsearch
==============

Install and configure elasticsearch on Debian server.

Installation
------------

git submodule add git@github.com/boostmyshoporganization/ansible-elasticsearch roles/elasticsearch

```yaml
roles:
    - elasticsearch
```

Configuration
-------------

```yaml
elasticsearch:
  version: 1.3
  cluster:
    name: elasticsearch
  node:
    name: main
  index:
    number_of_shards: 3
    number_of_replicas: 1
  heap_size: 1g
```