# Graph Report - hexagonal_architecture_graph  (2026-09-08)

## Corpus Check
- Corpus is ~0 words - fits in a single context window. You may not need a graph.

## Summary
- 21 nodes · 23 edges · 4 communities (3 shown, 1 thin omitted)
- Extraction: 83% EXTRACTED · 17% INFERRED · 0% AMBIGUOUS · INFERRED: 4 edges (avg confidence: 0.8)
- Token cost: 0 input · 0 output

## Community Hubs (Navigation)
- Ports, Adapters, and Testing
- Layered Architecture Approaches
- Configurable Interaction Patterns
- UML Component Interfaces

## God Nodes (most connected - your core abstractions)
1. `Ports & Adapters` - 12 edges
2. `Hexagonal Architecture Explained` - 6 edges
3. `Configurable Receiver` - 5 edges
4. `Hexagonal Architecture` - 2 edges
5. `Strategy Pattern` - 2 edges
6. `UML Component` - 2 edges
7. `Clean Architecture` - 2 edges
8. `Onion Architecture` - 2 edges
9. `Inside and Outside Layers` - 1 edges
10. `Primary and Secondary Actors` - 1 edges

## Surprising Connections (you probably didn't know these)
- `Ports & Adapters` --semantically_similar_to--> `Hexagonal Architecture`  [INFERRED] [semantically similar]
  hexagonal_book.pdf → hexagonal_book.pdf  _Bridges community 1 → community 0_
- `Ports & Adapters` --implements--> `Configurable Receiver`  [EXTRACTED]
  hexagonal_book.pdf → hexagonal_book.pdf  _Bridges community 0 → community 2_
- `Ports & Adapters` --conceptually_related_to--> `UML Component`  [EXTRACTED]
  hexagonal_book.pdf → hexagonal_book.pdf  _Bridges community 0 → community 3_

## Hyperedges (group relationships)
- **Hexagonal Architecture Boundary Mechanisms** — hexagonal_book_ports, hexagonal_book_adapters, hexagonal_book_provided_required_interfaces, hexagonal_book_test_doubles [INFERRED 0.85]
- **Configurable Receiver Collaboration** — hexagonal_book_configurator, hexagonal_book_configurable_receiver, hexagonal_book_sender_owned_interface [EXTRACTED 1.00]

## Communities (4 total, 1 thin omitted)

### Community 0 - "Ports, Adapters, and Testing"
Cohesion: 0.25
Nodes (8): Adapter Pattern, Adapters, Inside and Outside Layers, Ports, Ports & Adapters, Primary and Secondary Actors, Test Doubles, Tests and Mocks First

### Community 1 - "Layered Architecture Approaches"
Cohesion: 0.40
Nodes (6): Anti-Corruption Layer, Clean Architecture, CQRS Architecture, Hexagonal Architecture, Hexagonal Architecture Explained, Onion Architecture

### Community 2 - "Configurable Interaction Patterns"
Cohesion: 0.40
Nodes (5): Configurable Receiver, Configurator, Observer Pattern, Sender-Owned Interface, Strategy Pattern

## Knowledge Gaps
- **10 isolated node(s):** `Primary and Secondary Actors`, `Ports`, `Adapters`, `Test Doubles`, `Configurator` (+5 more)
  These have ≤1 connection - possible missing edges or undocumented components.
- **1 thin communities (<3 nodes) omitted from report** — run `graphify query` to explore isolated nodes.

## Suggested Questions
_Questions this graph is uniquely positioned to answer:_

- **Why does `Ports & Adapters` connect `Ports, Adapters, and Testing` to `Layered Architecture Approaches`, `Configurable Interaction Patterns`, `UML Component Interfaces`?**
  _High betweenness centrality (0.863) - this node is a cross-community bridge._
- **Why does `Hexagonal Architecture Explained` connect `Layered Architecture Approaches` to `Ports, Adapters, and Testing`?**
  _High betweenness centrality (0.363) - this node is a cross-community bridge._
- **Why does `Configurable Receiver` connect `Configurable Interaction Patterns` to `Ports, Adapters, and Testing`?**
  _High betweenness centrality (0.284) - this node is a cross-community bridge._
- **Are the 2 inferred relationships involving `Configurable Receiver` (e.g. with `Observer Pattern` and `Strategy Pattern`) actually correct?**
  _`Configurable Receiver` has 2 INFERRED edges - model-reasoned connections that need verification._
- **What connects `Primary and Secondary Actors`, `Ports`, `Adapters` to the rest of the system?**
  _10 weakly-connected nodes found - possible documentation gaps or missing edges._