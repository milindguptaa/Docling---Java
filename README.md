# Docling-Java

**RCOS Project — Spring 2026**

## Overview

Docling-Java is a project aimed at building a **local Java API** for Docling, a document-processing framework used in AI pipelines. Docling converts unstructured documents into structured, usable data. 

Currently, Docling exists only as a Python library. Other languages must access it indirectly through tools like *Docling-serve*, which exposes it as a REST API over HTTP and runs in Docker. 

This approach works but introduces extra overhead and complexity.

---

## Project Goal

The objective of this project is to create a **local GraalVM-based Java implementation** that allows Java applications to directly interact with the Docling Python library within the same process. 

By using GraalVM’s polyglot support, the system will:

* Remove HTTP communication overhead
* Simplify deployment
* Improve performance
* Provide a cleaner developer experience 

---

## Why This Matters

Existing methods of accessing Docling from Java rely on external communication layers. These add latency, increase system complexity, and make integration harder. 

Docling-Java aims to provide:

* Direct integration
* Faster execution
* More maintainable architecture

---

## Technical Approach

The project explores GraalVM’s ability to run multiple languages in a single process. This allows Java code to call Python libraries directly without network calls. 

Key technical focus areas:

* GraalVM polyglot interoperability
* Embedding Python runtime inside Java
* API design for Java developers
* Performance benchmarking

---
