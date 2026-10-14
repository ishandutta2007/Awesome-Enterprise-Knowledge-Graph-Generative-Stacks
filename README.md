# Awesome-Enterprise-Knowledge-Graph-Generative-Stacks

## Top Enterprise Knowledge Graph Generative Stacks Ecosystem



**Curated List of SaaS Products & Open-Source GitHub Projects**  

*Focused on Graph Databases, Semantic Layers & Change-Aware Data Evolution*  

**Last updated: October 2026**



This repository tracks notable **SaaS platforms** and **open-source projects** for **Enterprise Knowledge Graph Generative Stacks**. These tools enable organizations to model, store, and query highly connected data—tracking relational changes dynamically and grounding generative AI in structured, verifiable context.



**Examples** include Neo4j, Diffbot, data.world, Stardog, Ontotext GraphDB, Cambridge Semantics, Amazon Neptune, TigerGraph, PuppyGraph, and Katana Graph (the category leaders).



**Open-source emphasis**: This section is heavily expanded with every major active project for self-hosting, change-data-capture pipelines, and open graph+vector retrieval—ideal for data engineers, AI platform teams, and developers seeking transparent, vendor-independent knowledge graph infrastructure.



Contributions welcome! Open a PR to add/update entries. Keep descriptions factual and link to official sites.



## Table of Contents

- [SaaS/Hosted Platforms](#saas-hosted-platforms)

- [Open-Source GitHub Projects](#open-source-github-projects)

- [How to Contribute](#how-to-contribute)

- [Disclaimer](#disclaimer)



## SaaS/Hosted Platforms



- **[Neo4j (AuraDB)](https://neo4j.com/)**  

  The industry-standard graph database with Cypher query language and the largest ecosystem in the category. **AuraDB Free/Professional ($65/GB/mo)/Business Critical/Virtual Dedicated**; self-managed Community (GPL v3) or commercial Enterprise . Features vector index support for GraphRAG, Graph Data Science library with 50+ algorithms, and Bloom visualization. **Query language familiarity is the deciding factor**—teams that have shipped in Cypher rarely switch .



- **[Amazon Neptune](https://aws.amazon.com/neptune/)**  

  Fully managed AWS graph database supporting **Gremlin, SPARQL, and openCypher**. Strong at AWS scale with consumption-based pricing (instance-hours or serverless capacity units). **Neptune Analytics** adds graph analytics without database provisioning. Best for AWS-committed teams wanting a managed option .



- **[TigerGraph](https://www.tigergraph.com/)**  

  Distributed native graph database built for **deep multi-hop traversal** and massively parallel processing. **GSQL** query language with majority openCypher support; GSQL for advanced analytics . Savanna managed from **$45/GB/mo**; self-managed Community free to 300GB single-server . **Hybrid graph + vector search** for GraphRAG. Vendor-reported 40-337x advantage is 2-hop path queries only—unaudited, verify yourself . Best for fraud, AML, cybersecurity, and supply chain workloads .



- **[Stardog](https://www.stardog.com/)**  

  Enterprise knowledge graph platform with **SPARQL 1.1** and strong federated RDF capabilities. **Stardog Free**: renewable 1-year licence, commercial use, no HA/caching/backups/LDAP; Enterprise contact sales . Features federated virtual graphs and reasoning. Best for regulated or ontology-heavy organizations .



- **[Ontotext GraphDB](https://www.ontotext.com/)**  

  Semantic graph database with **SPARQL 1.1** and basic GraphQL in all editions; extended GraphQL is a paid add-on . **Free edition** (licence must be requested): 2 concurrent queries, 5 repositories, on-prem only. Strong for reasoning-heavy workloads and ontology management. Part of Graphwise .



- **[PuppyGraph](https://www.puppygraph.com/)**  

  Zero-ETL graph query engine that **maps data in warehouses and lakehouses into a graph model** and queries existing sources directly. No data migration required. Different category from conventional graph databases—best for teams that want graph analytics on data already in Snowflake, Databricks, or BigQuery .



- **[Diffbot](https://www.diffbot.com/)**  

  Knowledge graph from web-scale data. Features automated entity extraction, relationship mapping, and Knowledge Graph API. Part of emerging vendor category in the knowledge graph market .



- **[data.world](https://data.world/)**  

  Enterprise data catalog with knowledge graph capabilities. Features data discovery, lineage, and governance.



- **[Cambridge Semantics (AnzoGraph)](https://www.cambridgesemantics.com/)**  

  Enterprise knowledge graph platform with parallel processing. AnzoGraph is a native parallel processing graph database for large-scale analytics .



- **[Katana Graph](https://katanagraph.com/)**  

  High-performance graph analytics and AI platform. Features parallel graph processing for large-scale workloads.



## Open-Source GitHub Projects



- **[FalkorDB](https://github.com/FalkorDB/FalkorDB)**  

  **Apache 2.0 licensed graph database with 95%+ Cypher compatibility**—the leading Neo4j Community Edition alternative for license-sensitive projects . Fork of RedisGraph with active community. **In-memory architecture** provides excellent performance for code graphs and traversal-heavy workloads. Single Docker container deployment—lighter than Neo4j . Migration from Neo4j Community: 10-14 days core, 2-3 weeks total. Some advanced Cypher features (APOC equivalents) need adjustment. **The most practical open-source Neo4j replacement available** .



- **[Memgraph](https://github.com/memgraph/memgraph)**  

  **In-memory graph database with 100% Cypher compatibility** and extensive graph algorithm library (50+ algorithms). **BSL licensed**—not fully permissive, but source-available with free community edition . Native streaming support (Kafka, etc.) for real-time graph updates. Recommended alongside Neo4j and TigerGraph for performance and algorithm richness . Best for domains requiring analytics with sufficient RAM.



- **[NebulaGraph](https://github.com/vesoft-inc/nebula)**  

  **Open-source distributed native graph database** built for horizontally scaled deployments. Shared-nothing architecture with distributed storage and partitioning . **nGQL** query language designed to be compatible with openCypher concepts, but syntax and behavioral differences exist. **Enterprise scaling capabilities stand out** alongside TigerGraph . Greater migration and operational lift than closely Cypher-compatible alternatives . Best for engineering organizations prioritizing open-source distributed infrastructure.



- **[Apache AGE](https://github.com/apache/age)**  

  **PostgreSQL extension adding graph database capabilities** (Apache 2.0). OpenCypher support. Medium migration effort from Neo4j . **Best for teams already on PostgreSQL** wanting graph capabilities without a separate database. Single system for relational and graph queries.



- **[ArangoDB](https://github.com/arangodb/arangodb)**  

  **Multi-model database** combining graph, document, and search (Apache 2.0). **AQL** query language—not Cypher compatible, large migration effort . Native graph traversal and document storage. Best for teams needing multiple data models in one system .



- **[TerminusDB](https://github.com/terminusdb/terminusdb)**  

  Open-source **document graph database** with in-memory architecture and powerful versioning. Recommended alongside Memgraph for in-memory GDBs requiring powerful resources . Features time-travel queries and revision history.



- **[JanusGraph](https://github.com/JanusGraph/janusgraph)**  

  **Scalable open-source graph database** with pluggable storage backends (Apache Cassandra, HBase, BerkeleyDB). Best for teams needing horizontal scaling with existing storage infrastructure .



- **[Dgraph](https://github.com/dgraph-io/dgraph)**  

  **Distributed graph database** with GraphQL API (Apache 2.0). Very large migration effort from Neo4j due to GraphQL query language . Native GraphQL for applications already using GraphQL. Horizontal scaling with RAFT consensus .



- **[OverGraph](https://pypi.org/project/overgraph/)**  

  **Embedded graph database with dense/sparse/hybrid vector search** across Rust, Node.js, and Python . **GQL/Cypher-style query language** for reads, writes, schema DDL, and property-index DDL. Features **graph-scoped vector search** ("find 10 most similar nodes within 3 hops of node X"), temporal edges with validity windows and decay scoring, and atomic graph patches. **The most vector-native embedded graph database available**—zero overhead when vectors unused .



- **[trikedb](https://pypi.org/project/trikedb/)**  

  **YAML-file knowledge graph with SPARQL, vector search, and MCP server** . **One self-contained file**—no server, no build step. Features **change events as objects** (`AFFECTED_BY` edges pointing at dated event strings give your graph a memory), **`prov` edge attribute** for fact provenance, **ontology guardrails** preventing typo predicates, **OWL reasoning** with materialized inferred facts, and **SHACL validation** . **MCP server with OAuth 2.1** for Claude/ChatGPT integration—the graph stays a file, identity stays with your IdP . **The most agent-native open-source knowledge graph tool available.**



- **[Flexible GraphRAG](https://pypi.org/project/flexible-graphrag-mcp/)**  

  **Open-source GraphRAG platform with MCP server and OAuth2 bearer security** . Ingests from **14 data sources** (filesystem, CMIS, Alfresco, web, Wikipedia, YouTube, S3, GCS, Azure Blob, OneDrive, SharePoint, Box, Google Drive). Features hybrid search, AI-generated answers from documents, async processing status, and per-ingest `skip_graph` for vector-only fast paths. **Neo4j backend with configurable LLM/embedding providers**. HTTP mode for MCP Inspector debugging .



- **[Leangraph](https://www.npmjs.com/package/leangraph)**  

  **Lightweight embedded graph database with Cypher support** . Node.js/TypeScript with full Cypher clause coverage (CREATE, MATCH, MERGE, UNWIND, variable-length paths, CASE/WHEN). Typed TypeScript results, parameterized queries for injection safety, and in-memory test mode. **The simplest way to add Cypher graph capabilities to a Node.js application** .



- **[Ontograph](https://pypi.org/project/ontograph/)**  

  **LLM-powered knowledge graph engine with ontological entity resolution** . Features **orbit proximity scoring** (entities you interact with frequently score higher for resolution), **phonetic + spelling + semantic + orbit composite matching**, **self-improving feedback loop** tracking resolution accuracy, and **schema-constrained LLM extraction**. Local SQLite storage with `db.ingest()`, `db.search()`, and `db.ask()` . **The most sophisticated open-source entity resolution for knowledge graphs.**



- **[Apache Jena](https://github.com/apache/jena)**  

  **RDF framework and semantic web toolkit** (Apache 2.0). Features RDF parsing, SPARQL querying, OWL reasoning, and TDB storage . **The standard open-source Java toolkit for RDF and semantic web applications.**



- **[RDFLib](https://github.com/RDFLib/rdflib)**  

  **Python library for RDF graphs and SPARQL queries** . The foundational Python RDF library for semantic web applications.



- **[OntoDB](https://pypi.org/project/ontograph/)**  

  See Ontograph above.



### Additional Strong Open-Source Options



- **[docling-graph](https://github.com/topics/knowledge-graph)** — PDF/document → KG with LLM backend (Python) .

- **[llm-graph-builder](https://github.com/neo4j-labs/llm-graph-builder)** — Neo4j official tool for unstructured → graph .

- **[Docs2KG](https://github.com/topics/knowledge-graph)** — Human-LLM collaborative graph from diverse docs (Python) .

- **[knowledge_graph](https://github.com/topics/knowledge-graph)** — Text → graph for RAG & QnA (Python) .

- **[knowledge-graph-construction](https://github.com/topics/knowledge-graph)** — SPO triplet extraction + entity standardization (Python) .

- **[Mem0](https://github.com/mem0ai/mem0)** — Persistent memory with graph storage for LLM applications .

- **[LangChain](https://github.com/langchain-ai/langchain)** / **[LlamaIndex](https://github.com/run-llama/llama_index)** — Graph construction chains, RAG, and entity extraction .

- **[Apache Spark GraphX](https://github.com/apache/spark)** / **[Apache Flink Gelly](https://github.com/apache/flink)** — Distributed graph computation .

- **[NetworkX](https://github.com/networkx/networkx)** / **[igraph](https://github.com/igraph/igraph)** / **[Graph-Tool](https://git.skewed.de/count0/graph-tool)** — Python graph algorithms and analysis .

- **[Cytoscape.js](https://github.com/cytoscape/cytoscape.js)** / **[Sigma.js](https://github.com/jacomyal/sigma.js)** — Interactive web graph visualization .

- Community **n8n** workflows for change-data-capture event routing and GraphRAG pipeline automation.



**Frameworks for building custom systems**: Combine **FalkorDB** for license-permissive Cypher graph storage with **OverGraph** for vector-native retrieval, **trikedb** for YAML-file knowledge graphs with SPARQL and MCP, **Flexible GraphRAG** for multi-source ingestion, and **Ontograph** for entity resolution—creating a fully self-hosted, enterprise-grade knowledge graph generative stack.



## How to Contribute



1. Fork the repo.

2. Add/edit entries in `README.md` (follow existing format).

3. Include: name, link, 1–2 sentence description, and whether it's SaaS or open-source.

4. Submit PR with a short explanation.



Star the repo if you find it useful!



## Disclaimer



- This is a **community-curated** list — not exhaustive and not an endorsement.

- Knowledge graph platforms handling enterprise data must comply with data protection regulations (GDPR, CCPA, etc.) and maintain appropriate access controls.

- **License matters for graph databases.** Neo4j Community Edition is **GPLv3**—copyleft implications conflict with permissive licensing goals . FalkorDB (Apache 2.0) and Apache AGE (Apache 2.0) are fully permissive alternatives . Memgraph is BSL—not fully permissive . **Check the LICENSE file before embedding in a commercial product.**

- **Query language familiarity decides close calls.** Teams that have shipped in Cypher rarely switch—retraining on SPARQL is a cost most buyers underweight . FalkorDB (95%+ Cypher) and Memgraph (100% Cypher) minimize migration friction. NebulaGraph (nGQL) and ArangoDB (AQL) require more adaptation .

- **Change-data-capture (CDC) is essential for live knowledge graphs.** AllegroGraph demonstrates the pattern: Kafka/Debezium streams relational changes, batch-processed overnight, with history preserved for traceability . trikedb's `AFFECTED_BY` edges with dated event strings give graphs a memory—"why did this number change in April?" becomes a query .

- **Graph + vector convergence is the 2026 norm.** Most production GraphRAG systems run hybrid retrieval—vector for semantic similarity, graph for multi-hop reasoning . OverGraph's graph-scoped vector search ("10 most similar within 3 hops") and TigerGraph's hybrid graph+vector are examples .

- Self-hosted open-source solutions require proper security hardening, query optimization, and ongoing maintenance. Knowledge graphs are strategic assets—access controls and audit trails are essential.



---



**Made for data engineers, AI platform teams, and developers building transparent knowledge graph infrastructure.**  

Let's make Enterprise Knowledge Graph Generative Stacks more open, data-driven, and change-aware.
