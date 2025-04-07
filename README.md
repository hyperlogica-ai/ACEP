# AI Conceptual Exchange Protocol (ACEP)

[![License](https://img.shields.io/badge/License-Apache%202.0-blue.svg)](https://opensource.org/licenses/Apache-2.0)

## Overview

The AI Conceptual Exchange Protocol (ACEP) is a specialized communication language designed for efficient, precise, and unambiguous information exchange between artificial intelligence systems. ACEP prioritizes semantic density, computational efficiency, and mathematical precision over human readability, enabling more efficient AI-to-AI communication than is possible with natural language.

## Key features

- **Vector-Based Conceptual Tokens**: Concepts are represented as high-dimensional vectors (typically 10,000+ dimensions) in hyperdimensional computing space rather than as tokens or words
- **Explicit Relationship Markers**: All relationships between concepts include explicit type markers and certainty values
- **State-Based Context Management**: Information is stored in an addressable state system for efficient reference
- **Parallel Information Streams**: Multiple information streams can be processed simultaneously
- **Bounded Reasoning Structures**: Complex reasoning is organized into limited-length syllogisms with controlled uncertainty propagation
- **Embedded Certainty and Metadata**: Computational requirements, certainty values, and processing hints are directly encoded

## Documentation

This repository contains the complete specification for ACEP version 1.2, along with implementation examples, architecture designs, and usage patterns.

### Contents

- `/acep`: Formal specifications for ACEP (version 1.2)

## Use cases

ACEP is particularly valuable for:

- **AI-to-AI Communication**: Enabling efficient information exchange between different AI systems
- **Complex Reasoning**: Representing multi-step logical chains with explicit uncertainty propagation
- **Legal/Business Documents**: Precisely encoding contracts, agreements, and business rules
- **Knowledge Representation**: Storing and retrieving complex knowledge structures
- **Business Process Automation**: Encoding workflows, rules, and decision processes

## Example

Here's a simple example comparing ACEP to natural language:

**English (80+ tokens):**
```
"The weather forecast predicts rain tomorrow. If it rains tomorrow, then the outdoor event will be canceled. If the outdoor event is canceled, attendees will be refunded. Therefore, attendees will likely be refunded."
```

**ACEP (35-40 tokens):**
```
<{concept:rain_forecast, temporal:tomorrow, certainty:0.8}>
<{concept:event_cancellation}> ← <{condition:0.95}> ← <{ref:state[1]}>
<{concept:refund_issuance}> ← <{condition:1.0}> ← <{ref:state[2]}>
<{concept:refund_issuance, certainty:0.76}> // 0.8 × 0.95 × 1.0
```

This example demonstrates how ACEP can represent complex reasoning chains more efficiently while maintaining explicit certainty values and relationships.

## Getting started

### Prerequisites

- Understanding of vector representation in AI systems
- Familiarity with hyperdimensional computing concepts
- Development environment for your chosen implementation language

## Contributing

Contributions are welcome! Please feel free to submit a Pull Request.

1. Fork the repository
2. Create your feature branch (`git checkout -b feature/amazing-feature`)
3. Commit your changes (`git commit -m 'Add some amazing feature'`)
4. Push to the branch (`git push origin feature/amazing-feature`)
5. Open a Pull Request

## License

This project is licensed under the Apache License 2.0 - see the [LICENSE](LICENSE) file for details.

## Citation

If you use ACEP in your research, please cite:

```
@misc{acep2025,
  author = {Chroma Capital Management Pty Ltd},
  title = {AI Conceptual Exchange Protocol (ACEP)},
  year = {2025},
  publisher = {GitHub},
  url = {https://github.com/hyperlogica-ai/acep}
}
```


## Contact

Project URL: [https://github.com/hyperlogica-ai/acep](https://github.com/hyperlogica-ai/acep)
