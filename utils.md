---
layout: default
title: Utils
nav_order: 8
---

# Utils
{: .no_toc }

## Table of contents
{: .no_toc .text-delta }

1. TOC
{:toc}

---

## Parent from key
Get parent collection path from `key`

```python
parent_collection = utils.get_parent(key)
```

## Parent doc from key
Get parent document path from `key`

```python
parent_doc = utils.get_parent_doc(key)
```

## Id from key
Get `id` from `key`

```python
id = utils.get_id(key)
```

## Key from id and model
Get `key` from `id` and `model`

Simply concatenates `model.collection_name` and `id` so cannot derive the full `key` for models used in subcollections.

```python
key = utils.generateKeyFromId(model, key)
```