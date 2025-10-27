# Fotoshot

Scalable, high performance knowledge graph memory system with semantic retrieval, contextual recall, and temporal awareness. Provides any LLM client that supports the model context protocol (e.g., Claude Desktop, Cursor, Github Copilot) with resilient, adaptive, and persistent long-term ontological memory.

## Core Features

### Entity Management

- **create_entities**

  - Create multiple new entities in the knowledge graph
  - Input: `entities` (array of objects)
    - Each object contains:
      - `name` (string): Entity identifier
      - `entityType` (string): Type classification
      - `observations` (string[]): Associated observations


### Relation Management

- **create_relations**

  - Create multiple new relations between entities with enhanced properties
  - Input: `relations` (array of objects)
    - Each object contains:
      - `from` (string): Source entity name
      - `to` (string): Target entity name
      - `relationType` (string): Relationship type
      - `strength` (number, optional): Relation strength (0.0-1.0)
      - `confidence` (number, optional): Confidence level (0.0-1.0)
      - `metadata` (object, optional): Custom metadata fields

