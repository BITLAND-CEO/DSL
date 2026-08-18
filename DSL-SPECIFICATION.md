# DSL — Digital Sign Language
## Specification v1.0

**Status:** Community Draft / Version 1.0  
**Project:** Digital Sign Language (DSL)

### 1. Purpose

Digital Sign Language (DSL) is an open, extensible system for adding standardized digital signals to content.

DSL is intended to communicate the **intended role, attention, or action associated with a message** without replacing the natural language used in that message.

DSL is designed for humans and, where implemented, machine-readable systems.

### 2. Design Principles

1. **Simple** — signals should be easy to understand and use.
2. **Universal** — the signaling layer should work across natural languages.
3. **Explicit** — a signal must have a defined meaning.
4. **Extensible** — new signals can be proposed without breaking existing meanings.
5. **Machine-readable** — syntax should be parseable by software.
6. **Open** — development, proposals, discussion, and decisions should be transparent.
7. **Non-authoritative** — a DSL signal does not prove truth, identity, authority, urgency, or endorsement.

### 3. Core Syntax

The minimum human-readable form is:

`#DSL #SIGNAL`

Examples:

`#DSL #IDEA`  
`#DSL #HELP`  
`#DSL #WARNING`  
`#DSL #REQUEST`  
`#DSL #QUESTION`

The controlled vocabulary is defined by this specification and future approved revisions.

### 4. Core Signals v1.0

| Signal | Meaning |
|---|---|
| `IDEA` | An idea or concept submitted for consideration |
| `HELP` | A request for assistance |
| `WARNING` | A warning or alert |
| `REQUEST` | A request directed toward a person, group, organization, or system |
| `QUESTION` | A question for which attention or response is sought |
| `PROPOSAL` | A proposed action, change, or solution |
| `ATTENTION` | A request that content receive attention |
| `INFORMATION` | Important information intended primarily for communication |

A signal may be used only according to its defined meaning.

### 5. Optional Target

A future-compatible target form is:

`#DSL #TARGET:<identifier> #SIGNAL`

Example:

`#DSL #TARGET:ExampleOrg #REQUEST`

Target identifiers do not establish affiliation, authorization, identity, or endorsement.

### 6. Optional Metadata

Implementations may attach machine-readable metadata such as:

- specification version
- date/time
- language
- target
- signal
- source
- status

Metadata must not change the defined meaning of a core signal.

### 7. Machine Representation

A compatible implementation may represent a DSL signal as structured data.

Example:

```json
{
  "dsl": "1.0",
  "signal": "REQUEST",
  "target": "ExampleOrg"
}
```

JSON is an implementation example, not a requirement for ordinary users.

### 8. Truth and Verification

DSL identifies the sender's declared signal or intention. It does not verify the factual accuracy of the associated content.

Platforms must not treat the presence of a DSL signal as automatic verification.

### 9. Safety

Implementations should protect against:

- spam
- impersonation
- harassment
- false urgency
- manipulation
- automated abuse
- misleading targeting

No DSL signal automatically grants visibility, priority, authority, or access.

### 10. Compatibility

Existing v1.0 core signals should not be silently redefined.

Breaking semantic changes require a new major version.

### 11. Versioning

- **Major:** breaking semantic or syntax change
- **Minor:** backward-compatible new functionality or signal
- **Patch:** editorial, documentation, or non-semantic correction

Current version: **1.0**

### 12. Open Development

Anyone may propose additions, corrections, or changes through the project's proposal process.

See:

- `GOVERNANCE.md`
- `CONTRIBUTING.md`
- `PROPOSALS/README.md`

### 13. Status

DSL v1.0 is an open community specification and is not claimed to be an internationally adopted standard.
