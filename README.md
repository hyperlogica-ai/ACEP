# AI Conceptual Exchange Protocol (ACEP)

<div align="center">

**A communication protocol for AI systems based on hyperdimensional computing**

[![Protocol Version](https://img.shields.io/badge/ACEP-v2.0-green.svg)](ACEP_description.md)
[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](LICENSE)

</div>

---

## Overview

The AI Conceptual Exchange Protocol (ACEP) is a communication protocol for information exchange between artificial intelligence systems. Based on hyperdimensional computing principles, ACEP v2.0 extends the original specification with multi-dimensional uncertainty modeling, temporal knowledge dynamics, and causal reasoning capabilities.

ACEP represents concepts as high-dimensional vectors (typically 10,000+ dimensions) and uses vector operations to encode relationships and perform reasoning operations. The protocol uses a compact notation with angle brackets and structured attribute lists.

## Protocol Components

### Core Elements
- **Hyperdimensional Computing Foundation**: Vector-based concept representation
- **Multi-Dimensional Uncertainty**: Distinction between different uncertainty types
- **Temporal Knowledge Management**: Support for knowledge that changes over time
- **Causal Relationship Encoding**: Representation of causal mechanisms
- **Working Memory Integration**: Modeling of cognitive processing constraints

### New in v2.0
- **Compound Logical Operators**: Support for AND, OR, NOT operations
- **Causal Mechanism Types**: Classification of causal relationships
- **Attention Operations**: Selective information processing
- **Goal-Directed Processing**: Target-oriented reasoning support
- **Enhanced Uncertainty Model**: Separate epistemic and aleatory components

## Quick Start

### Basic Concept Representation
```
<{concept:market_volatility, temporal:2024-Q1, modality:observed, uncertainty:{epistemic:0.1, aleatory:0.8, confidence:0.9}, causal_role:effect}>
```

### Causal Relationship Example
```
<{concept:interest_rate_increase, magnitude:significant}> → <{causal:{mechanism:discount_rate_theory, intervention_type:contributory, strength:0.8, direction:negative, time_lag:30_days, confounders:[market_momentum, investor_sentiment]}, uncertainty:{epistemic:0.15, aleatory:0.25, confidence:0.85}}> → <{concept:tech_stock_decline, entity:technology_sector}>
```

### Working Memory Representation
```
<{working_memory:{active_concepts:[market_analysis, risk_assessment, portfolio_optimization], capacity_utilization:0.7, attention_weights:{market_analysis:0.5, risk_assessment:0.3, portfolio_optimization:0.2}, interference_level:0.2}}>
```

## Structure

### 1. Conceptual Vectors
- High-dimensional vector representations of concepts
- Attributes for uncertainty, temporal, and causal information
- Support for abstraction levels

### 2. Relationship Markers
- Relationship types with uncertainty values
- Logical operators for compound conditions
- Causal relationships with mechanism types

### 3. Multi-Dimensional Uncertainty
- **Epistemic**: Uncertainty from incomplete knowledge
- **Aleatory**: Inherent randomness
- **Confidence**: Assessment confidence level
- **Evidence Quality**: Source reliability measure
- **Temporal Decay**: Time-dependent uncertainty changes

### 4. Temporal Dynamics
- Knowledge aging and decay functions
- Update frequency specifications
- Validity period tracking

### 5. Working Memory Operations
- Capacity constraints modeling
- Attention allocation
- Information interference patterns

## Vector Operations

ACEP v2.0 uses standard HDC operations:

### Basic Operations
- **Binding (⊕)**: Create associations between concepts
- **Bundling (+)**: Combine multiple concepts
- **Unbinding**: Retrieve associated concepts

### Extended Operations
- **Hierarchical Binding**: Create abstract concepts
- **Temporal Updates**: Apply aging to knowledge vectors
- **Causal Binding**: Encode causal relationships
- **Attention Operations**: Selective activation

## Implementation Requirements

### Vector Space Management
- Support for high-dimensional vectors (10,000+ dimensions recommended)
- Vector similarity computation
- Binding and unbinding operations
- Temporal vector updates

### Uncertainty Handling
- Multi-dimensional uncertainty representation
- Uncertainty propagation through reasoning
- Temporal uncertainty modeling

### Causal Reasoning
- Causal relationship representation
- Intervention modeling
- Counterfactual reasoning support

### Working Memory
- Capacity constraint implementation
- Attention mechanisms
- Information interference modeling

## Migration from ACEP v1.0

ACEP v2.0 maintains backward compatibility with v1.0:

### Backward Compatibility
ACEP v2.0 maintains backward compatibility with v1.0 through default value mapping:
- v1.0 certainty values map to v2.0 confidence
- Simple relationships become basic causal structures
- Single timestamps expand to temporal models

## Reference Implementation

### Hyperlogica
Current reference implementation of ACEP v2.0:
- **Language**: Python 3.8+
- **Features**: ACEP v2.0 support with FAISS vector storage

## Application Areas

ACEP v2.0 can be applied in domains requiring:
- Uncertainty quantification and reasoning
- Temporal knowledge management
- Causal relationship modeling
- Multi-step inference chains
- Knowledge integration across sources

## Testing and Validation

Implementation testing should verify:
- ACEP v2.0 structure compliance
- Vector operation correctness
- Uncertainty propagation accuracy
- Temporal consistency

## Documentation

- **[Protocol Specification](ACEP_description.md)** - Complete ACEP v2.0 specification with examples

## Contributing

Contributions to the ACEP specification are welcome:

1. **Protocol Proposals**: Submit proposals for protocol extensions
2. **Implementation Feedback**: Report specification issues
3. **Usage Examples**: Provide real-world usage examples
4. **Testing Tools**: Contribute validation utilities

## License

This protocol specification is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.
