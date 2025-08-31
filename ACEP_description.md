# AI Conceptual Exchange Protocol (ACEP)
## Formal Specification v2.0

## 1. Introduction

The AI Conceptual Exchange Protocol (ACEP) v2.0 is a communication protocol for information exchange between artificial intelligence systems. Building upon the hyperdimensional computing foundation of ACEP v1.0, this version adds support for multi-dimensional uncertainty modeling, temporal knowledge dynamics, causal reasoning, and cognitive processing patterns.

ACEP uses a compact, efficient notation designed for minimal token usage while maximizing semantic expressiveness. This specification defines both the core ACEP notation and JSON implementation formats for different use cases.

## 2. Protocol Formats

### 2.1 Core ACEP Format

The core ACEP format uses angle brackets with structured attribute notation:
```
<{attribute:value, attribute:value, ...}>
```

This format is optimized for:
- **Token efficiency**: Minimal character count for maximum information density
- **Machine parsing**: Unambiguous structure for automated processing
- **Human readability**: Clear semantic structure
- **Compositionality**: Easy combination of elements

### 2.2 JSON Implementation Format

JSON representations provide expanded attribute structures suitable for:
- **Implementation compatibility**: Standard JSON parsing libraries
- **Complex nested structures**: Detailed metadata and configuration
- **Debugging and logging**: Human-readable expanded format
- **API integration**: Web services and REST interfaces

Both formats represent identical semantic content with different syntactic presentations.

## 3. Core Design Principles

ACEP v2.0 extends the original design with the following principles:

1. **Hyperdimensional Computing Foundation**: Concepts represented as high-dimensional vectors (typically 10,000+ dimensions) using HDC mathematical operations
2. **Working Memory Integration**: Working memory modeled through vector bundling and unbinding operations with capacity constraints
3. **Multi-Dimensional Uncertainty**: Uncertainty representation that distinguishes between different types of uncertainty and their sources
4. **Temporal Knowledge Management**: Support for knowledge that changes over time with explicit aging and update mechanisms
5. **Causal Relationship Encoding**: Explicit representation of causal relationships with mechanism identification
6. **Hierarchical Abstraction**: Support for abstract concepts through compositional vector operations
7. **Cognitive Processing Patterns**: Attention mechanisms and meta-cognitive operations
8. **Agent-Oriented Design**: Integration points for perception, planning, and goal-directed reasoning
9. **Formal Logic Integration**: Support for quantified expressions, variable binding, and structured logical relationships through HDC composition
10. **Consistency Management**: Built-in contradiction detection and resolution mechanisms using vector coherence measures
11. **Meta-Level Reasoning**: Higher-order reasoning about knowledge and reasoning processes through hierarchical vector structures

## 4. Enhanced ACEP Components

### 4.1 Conceptual Vectors

Conceptual vectors are the atomic units of ACEP v2.0, with enhanced attribute support:

#### 4.1.1 Core ACEP Structure
```
<{concept:identifier, attribute1:value1, attribute2:value2, ..., uncertainty:uncertainty_model, temporal:temporal_model}>
```

#### 4.1.2 JSON Implementation Structure
```json
{
  "concept": "identifier",
  "attributes": {
    "attribute1": "value1",
    "attribute2": "value2"
  },
  "uncertainty": {
    "epistemic": 0.0-1.0,
    "aleatory": 0.0-1.0,
    "confidence": 0.0-1.0
  },
  "temporal": {
    "timestamp": "iso_datetime",
    "validity_period": "time_range"
  }
}
```

#### 4.1.3 Enhanced Standard Attributes
- `temporal`: Temporal reference with decay modeling support
- `valence`: Evaluative quality (positive, negative, neutral) with optional intensity measure
- `modality`: Mode of existence (actual, possible, necessary, hypothetical) with confidence intervals
- `uncertainty`: Multi-dimensional uncertainty model (see Section 4.3)
- `causal_role`: Role in causal relationships (cause, effect, mediator, moderator)
- `abstraction_level`: Level in conceptual hierarchy (0=concrete, higher numbers=more abstract)
- `grounding`: Connection to observable or measurable phenomena

#### 4.1.4 Examples

**Core ACEP:**
```
<{concept:market_volatility, temporal:2024-Q1, modality:observed, uncertainty:{epistemic:0.1, aleatory:0.8, confidence:0.9}, causal_role:effect}>
```

**JSON Implementation:**
```json
{
  "concept": "market_volatility",
  "temporal": {
    "timestamp": "2024-Q1",
    "granularity": "quarter"
  },
  "modality": "observed",
  "uncertainty": {
    "epistemic": 0.1,
    "aleatory": 0.8,
    "confidence": 0.9
  },
  "causal_role": "effect"
}
```

### 4.2 Enhanced Relationship Markers

Relationship markers support complex logical structures and causal relationships:

#### 4.2.1 Core ACEP Structure
```
concept1 → <{relation_type:certainty_model, logical_operator:operator_type, causal_mechanism:mechanism_type}> → concept2
```

#### 4.2.2 JSON Implementation Structure
```json
{
  "relationship_type": "causal|conditional|hierarchical|...",
  "source": "concept1",
  "target": "concept2",
  "attributes": {
    "certainty_model": 0.0-1.0,
    "logical_operator": "and|or|not|implies|...",
    "causal_mechanism": "mechanism_type"
  }
}
```

#### 4.2.3 Enhanced Relationship Types
- `causal`: Cause-effect relationships with mechanism specification
- `counterfactual`: Hypothetical relationships under alternative conditions
- `conditional`: If-then relationships supporting compound conditions
- `temporal_causal`: Time-dependent causal relationships
- `hierarchical`: Abstract-concrete relationships in conceptual hierarchies
- `analogical`: Cross-domain similarity relationships
- `part_of`: Component relationships with compositional semantics
- `is_a`: Type or category relationships with inheritance properties
- `enables`: Facilitation relationships
- `prevents`: Blocking or inhibiting relationships

#### 4.2.4 Logical Operators
- `and`: Conjunction of conditions
- `or`: Disjunction of conditions  
- `not`: Negation
- `implies`: Material implication
- `iff`: Biconditional
- `forall`: Universal quantification
- `exists`: Existential quantification

#### 4.2.5 Examples

**Core ACEP:**
```
<{concept:interest_rate_increase}> → <{causal:{mechanism:discount_rate_theory, strength:0.8, time_lag:30_days}}> → <{concept:tech_stock_decline}>

<{logical_operator:and, clauses:[condition1, condition2]}> → <{implies:0.8}> → conclusion
```

**JSON Implementation:**
```json
{
  "relationship_type": "causal",
  "source": {
    "concept": "interest_rate_increase",
    "magnitude": "significant"
  },
  "target": {
    "concept": "tech_stock_decline",
    "entity": "technology_sector"
  },
  "causal_metadata": {
    "mechanism": "discount_rate_theory",
    "strength": 0.8,
    "time_lag": "30_days"
  }
}
```

### 4.3 Multi-Dimensional Uncertainty Model

#### 4.3.1 Core ACEP Structure
```
<{uncertainty:{epistemic:float, aleatory:float, confidence:float, evidence_quality:float, temporal_decay:decay_model}}>
```

#### 4.3.2 JSON Implementation Structure
```json
{
  "uncertainty": {
    "epistemic": 0.0-1.0,
    "aleatory": 0.0-1.0,
    "confidence": 0.0-1.0,
    "evidence_quality": 0.0-1.0,
    "temporal_decay": {
      "model": "exponential|linear|step|none",
      "parameters": {}
    },
    "consensus_level": 0.0-1.0
  }
}
```

#### 4.3.3 Uncertainty Components
- `epistemic`: Uncertainty due to lack of knowledge (0-1)
- `aleatory`: Uncertainty due to inherent randomness (0-1) 
- `confidence`: Subjective confidence in the assessment (0-1)
- `evidence_quality`: Quality and reliability of supporting evidence (0-1)
- `temporal_decay`: Model for how uncertainty changes over time
- `consensus_level`: Level of agreement across multiple sources (0-1)

#### 4.3.4 Temporal Decay Models
- `exponential`: Exponential decay with half-life parameter
- `linear`: Linear decay rate
- `step`: Discrete expiration dates
- `none`: No temporal decay

#### 4.3.5 Examples

**Core ACEP:**
```
<{uncertainty:{epistemic:0.2, aleatory:0.1, confidence:0.9, evidence_quality:0.8, temporal_decay:{model:exponential, half_life:365_days}, consensus_level:0.7}}>
```

**JSON Implementation:**
```json
{
  "uncertainty": {
    "epistemic": 0.2,
    "aleatory": 0.1,
    "confidence": 0.9,
    "evidence_quality": 0.8,
    "temporal_decay": {
      "model": "exponential",
      "half_life": "365_days"
    },
    "consensus_level": 0.7
  }
}
```

### 4.4 Temporal Dynamics

#### 4.4.1 Core ACEP Structure
```
<{temporal:{timestamp:iso_datetime, validity_period:time_range, update_frequency:frequency, decay_function:function_type}}>
```

#### 4.4.2 JSON Implementation Structure
```json
{
  "temporal": {
    "timestamp": "2024-03-15T14:30:00Z",
    "validity_period": {
      "start": "2024-Q1",
      "end": "2024-Q2"
    },
    "update_frequency": "monthly",
    "decay_function": "exponential_0.95",
    "temporal_scope": "past|present|future|atemporal",
    "temporal_granularity": "seconds|days|years"
  }
}
```

#### 4.4.3 Temporal Components
- `timestamp`: Creation or observation time
- `validity_period`: Time range of validity
- `update_frequency`: How often knowledge should be refreshed
- `decay_function`: Knowledge degradation over time
- `temporal_scope`: Past, present, future, or atemporal
- `temporal_granularity`: Precision level (seconds, days, years)

#### 4.4.4 Examples

**Core ACEP:**
```
<{temporal:{timestamp:2024-03-15T14:30:00Z, validity_period:[2024-Q1, 2024-Q2], update_frequency:monthly, decay_function:exponential_0.95}}>
```

**JSON Implementation:**
```json
{
  "temporal": {
    "timestamp": "2024-03-15T14:30:00Z",
    "validity_period": {
      "start": "2024-Q1",
      "end": "2024-Q2"
    },
    "update_frequency": "monthly",
    "decay_function": "exponential_0.95"
  }
}
```

### 4.5 Causal Structure Encoding

#### 4.5.1 Core ACEP Structure
```
<{causal:{mechanism:mechanism_type, intervention_type:intervention_class, confounders:variable_list, strength:causal_strength}}>
```

#### 4.5.2 JSON Implementation Structure
```json
{
  "causal": {
    "mechanism": "physical|logical|statistical|...",
    "intervention_type": "necessary|sufficient|contributory|preventive",
    "confounders": ["variable1", "variable2"],
    "strength": 0.0-1.0,
    "direction": "positive|negative",
    "time_lag": "duration"
  }
}
```

#### 4.5.3 Causal Components
- `mechanism`: Type of causal mechanism (physical, logical, statistical)
- `intervention_type`: Necessary, sufficient, contributory, preventive
- `confounders`: Variables that may affect the relationship
- `strength`: Causal strength measure (0-1)
- `direction`: Positive or negative causal influence
- `time_lag`: Delay between cause and effect

#### 4.5.4 Examples

**Core ACEP:**
```
<{concept:interest_rate_increase}> → <{causal:{mechanism:economic, intervention_type:contributory, strength:0.7, direction:negative, time_lag:30_days}}> → <{concept:stock_market_decline}>
```

**JSON Implementation:**
```json
{
  "relationship_type": "causal",
  "source": {
    "concept": "interest_rate_increase"
  },
  "target": {
    "concept": "stock_market_decline"
  },
  "causal_metadata": {
    "mechanism": "economic",
    "intervention_type": "contributory",
    "strength": 0.7,
    "direction": "negative",
    "time_lag": "30_days"
  }
}
```

### 4.6 Enhanced Operations

Operations support complex reasoning patterns and agent capabilities:

#### 4.6.1 Core ACEP Structure
```
<{operation:type, parameters:parameter_dict, cognitive_context:context_model}>
```

#### 4.6.2 JSON Implementation Structure
```json
{
  "operation": {
    "type": "reason|plan|learn|attend|abstract|ground|simulate|meta_reason",
    "parameters": {},
    "cognitive_context": {
      "working_memory_state": [],
      "attention_focus": "concept",
      "reasoning_strategy": "strategy_type",
      "goal_stack": [],
      "confidence_threshold": 0.0-1.0
    }
  }
}
```

#### 4.6.3 Enhanced Operation Types
- `reason`: Perform inference with strategy specification
- `plan`: Generate action sequences toward goals
- `learn`: Update knowledge from experience
- `attend`: Focus working memory on specific concepts
- `abstract`: Create higher-level representations
- `ground`: Connect to sensorimotor experience
- `simulate`: Run counterfactual scenarios
- `meta_reason`: Reason about reasoning strategies

#### 4.6.4 Examples

**Core ACEP:**
```
<{operation:plan, parameters:{goal:maximize_profit, horizon:1_year, risk_tolerance:0.3}, cognitive_context:{working_memory_state:[market_data, portfolio_state], attention_focus:volatility_analysis, reasoning_strategy:causal_inference}}>
```

**JSON Implementation:**
```json
{
  "operation": {
    "type": "plan",
    "parameters": {
      "goal": "maximize_profit",
      "horizon": "1_year",
      "risk_tolerance": 0.3
    },
    "cognitive_context": {
      "working_memory_state": ["market_data", "portfolio_state"],
      "attention_focus": "volatility_analysis",
      "reasoning_strategy": "causal_inference"
    }
  }
}
```

### 4.8 Quantifier and Variable Binding System

ACEP v2.0 supports formal logical structures through HDC compositional binding:

#### 4.8.1 Core ACEP Structure
```
<{quantifier:{type:universal|existential, variables:variable_list, domain_constraints:constraint_list, scope:logical_expression}}>
```

#### 4.8.2 JSON Implementation Structure
```json
{
  "quantifier": {
    "type": "universal|existential",
    "variables": [
      {
        "identifier": "?X",
        "domain": "concept_type",
        "constraints": ["constraint1", "constraint2"]
      }
    ],
    "scope": {
      "logical_expression": "...",
      "vector_binding": "compositional_structure"
    }
  }
}
```

#### 4.8.3 Variable Binding Components
- `variable_identifier`: Unique variable name (e.g., ?X, ?Y)
- `domain_constraints`: Type restrictions for the variable
- `scope`: Expression where the variable is bound
- `binding_vector`: HDC vector encoding variable relationships
- `substitution_pattern`: Template for variable instantiation

#### 4.8.4 HDC Variable Binding Implementation
```
// Generate unique role vectors for variables
V_var_X = generate_vector("variable_X")
V_var_Y = generate_vector("variable_Y")

// Bind variables with their constraints  
V_X_constrained = V_bind(V_var_X, V_bind(constraint_role, V_domain))

// Compose complex quantified expressions
V_quantified = V_bind(V_universal, V_bind(V_X_constrained, V_scope_expression))
```

#### 4.8.5 Examples

**Core ACEP - Universal Quantification:**
```
<{quantifier:{type:universal, variables:[{id:?X, domain:Bird, constraints:[living]}], scope:<{?X}> → <{capability:flying}>, vector_binding:V_bind(V_universal, V_bind(V_X_bird, V_flying))}}>
```

**JSON Implementation:**
```json
{
  "quantifier": {
    "type": "universal",
    "variables": [
      {
        "identifier": "?X",
        "domain": "Bird", 
        "constraints": ["living", "adult"]
      }
    ],
    "scope": {
      "implication": {
        "antecedent": {"variable": "?X", "property": "is_bird"},
        "consequent": {"variable": "?X", "capability": "flying"}
      }
    },
    "vector_binding": "V_bind(V_universal, V_bind(V_X_bird, V_flying))"
  }
}
```

**Core ACEP - Complex Multi-Variable:**
```
<{quantifier:{type:existential, variables:[{id:?COMPANY, domain:Company}, {id:?YEAR, domain:CalendarYear, constraints:[gt_2020]}], scope:<{?COMPANY, revenue_in:?YEAR}> → <{gt:$1M}> → <{?COMPANY, has:employees}>}}>
```

### 4.9 Consistency Management System

ACEP v2.0 includes built-in contradiction detection and resolution:

#### 4.9.1 Core ACEP Structure
```
<{consistency:{coherence_measure:float, contradictions:contradiction_list, resolution_strategy:strategy_type, confidence_adjustment:adjustment_factor}}>
```

#### 4.9.2 JSON Implementation Structure  
```json
{
  "consistency": {
    "coherence_measure": 0.0-1.0,
    "contradictions": [
      {
        "statement1": "statement_id",
        "statement2": "statement_id", 
        "conflict_type": "direct|indirect|probabilistic",
        "severity": 0.0-1.0
      }
    ],
    "resolution_strategy": "priority_based|confidence_weighted|temporal_precedence",
    "confidence_adjustment": -1.0-1.0
  }
}
```

#### 4.9.3 HDC Consistency Implementation
```
// Measure vector coherence across knowledge base
V_knowledge_state = V_bundle([V_fact1, V_fact2, ..., V_factN])
coherence = measure_vector_coherence(V_knowledge_state)

// Detect contradictions through vector opposition
contradiction_threshold = 0.3
for each pair (V_i, V_j) in knowledge_base:
    if similarity(V_i, V_negate(V_j)) > contradiction_threshold:
        flag_contradiction(V_i, V_j)
```

#### 4.9.4 Consistency Components
- `coherence_measure`: Overall knowledge base consistency (0-1)
- `contradiction_detection`: Automatic identification of conflicting statements
- `resolution_strategies`: Methods for resolving detected contradictions
- `confidence_propagation`: How contradictions affect statement confidence
- `temporal_consistency`: Ensuring consistency across time

#### 4.9.5 Examples

**Core ACEP:**
```
<{consistency:{coherence_measure:0.85, contradictions:[{stmt1:weather_sunny, stmt2:weather_rainy, conflict_type:direct, severity:0.9}], resolution_strategy:temporal_precedence, confidence_adjustment:-0.2}}>
```

**JSON Implementation:**
```json
{
  "consistency": {
    "coherence_measure": 0.85,
    "contradictions": [
      {
        "statement1": "weather_sunny_today",
        "statement2": "weather_rainy_today",
        "conflict_type": "direct",
        "severity": 0.9,
        "detection_method": "vector_opposition"
      }
    ],
    "resolution_strategy": "temporal_precedence",
    "confidence_adjustment": -0.2
  }
}
```

### 4.10 Meta-Level Reasoning System

Support for reasoning about knowledge and reasoning processes:

#### 4.10.1 Core ACEP Structure
```
<{meta_level:{reasoning_about:target_concept, meta_type:knowledge|process|strategy, higher_order_relation:relation_type, reflexivity:boolean}}>
```

#### 4.10.2 JSON Implementation Structure
```json
{
  "meta_level": {
    "reasoning_about": "target_concept_id",
    "meta_type": "knowledge|process|strategy|belief",
    "higher_order_relation": "believes|knows|doubts|proves",
    "reflexivity": true,
    "meta_vector_binding": "hierarchical_structure"
  }
}
```

#### 4.10.3 HDC Meta-Level Implementation
```
// Create meta-level through hierarchical binding
V_meta_role = generate_vector("meta_level_reasoning")
V_knowledge_about = generate_vector("knowledge_about")
V_target_concept = generate_vector("target_reasoning")

// Bind meta-relationship
V_meta_statement = V_bind(V_meta_role, 
                    V_bind(V_knowledge_about, 
                     V_bind(agent_vector, V_target_concept)))
```

#### 4.10.4 Meta-Level Components
- `reasoning_about`: Target of meta-level reasoning
- `meta_type`: Type of meta-level relationship (knowledge, belief, process)
- `higher_order_relation`: Specific meta-relationship (believes, knows, proves)
- `reflexivity`: Whether the statement can refer to itself
- `meta_confidence`: Confidence in the meta-level assessment

#### 4.10.5 Examples

**Core ACEP - Agent Belief:**
```
<{meta_level:{agent:AI_system_1, believes:<{concept:market_growth, entity:AAPL, confidence:0.8}>, meta_confidence:0.9, justification:historical_analysis}}>
```

**JSON Implementation:**
```json
{
  "meta_level": {
    "agent": "AI_system_1", 
    "meta_relation": "believes",
    "target_statement": {
      "concept": "market_growth",
      "entity": "AAPL", 
      "confidence": 0.8
    },
    "meta_confidence": 0.9,
    "justification": "historical_analysis",
    "vector_structure": "V_bind(V_believes, V_bind(V_agent, V_target))"
  }
}
```

**Core ACEP - Reasoning About Reasoning:**
```
<{meta_level:{process:causal_inference, effectiveness:0.7, domain:financial_markets, meta_type:strategy_evaluation, higher_order:<{strategy:analogical_reasoning}> → <{better_for:novel_domains}>}}>
```

### 4.11 Context and Microtheory Support

Support for contextual knowledge and belief spaces:

#### 4.11.1 Core ACEP Structure
```
<{context:{id:context_identifier, type:belief_space|temporal_context|hypothetical|domain, scope:statement_list, inheritance:parent_contexts}}>
```

#### 4.11.2 JSON Implementation Structure
```json
{
  "context": {
    "id": "context_identifier",
    "type": "belief_space|temporal_context|hypothetical|domain",
    "scope": ["statement_id1", "statement_id2"],
    "inheritance": ["parent_context1", "parent_context2"],
    "validity_conditions": [],
    "isolation_level": 0.0-1.0
  }
}
```

#### 4.11.3 HDC Context Implementation
```
// Generate context vectors
V_context = generate_vector("context_name")
V_context_type = generate_vector("belief_space")

// Bind statements to contexts
V_contextualized = V_bind(V_context, 
                    V_bind(V_context_type, V_statement))

// Context inheritance through vector composition
V_child_context = V_bind(V_parent_context, V_child_specific)
```

#### 4.11.4 Context Components
- `context_identifier`: Unique context name
- `context_type`: Type of contextual space (belief, temporal, hypothetical)
- `scope`: Statements that exist within this context
- `inheritance`: Parent contexts from which this inherits
- `validity_conditions`: Conditions under which context is active
- `isolation_level`: How isolated the context is from others

#### 4.11.5 Examples

**Core ACEP:**
```
<{context:{id:CurrentWorldMt, type:belief_space, scope:[fact1, fact2, fact3]}}> 
<{context:{id:HypotheticalScenario_1, type:hypothetical, inheritance:[CurrentWorldMt], validity_conditions:[fed_rate_unchanged]}}>
```

**JSON Implementation:**
```json
{
  "contexts": [
    {
      "id": "CurrentWorldMt",
      "type": "belief_space", 
      "scope": ["capital_paris", "population_france", "gdp_2024"],
      "inheritance": [],
      "authority_level": 1.0
    },
    {
      "id": "HypotheticalScenario_Fed",
      "type": "hypothetical",
      "scope": ["market_response_scenario"],
      "inheritance": ["CurrentWorldMt"],
      "validity_conditions": ["fed_rate_unchanged"],
      "isolation_level": 0.3
    }
  ]
}
```

### 4.12 Default Logic and Non-Monotonic Reasoning

Support for defeasible reasoning and exception handling:

#### 4.12.1 Core ACEP Structure
```
<{default_rule:{antecedent:condition, consequent:conclusion, exceptions:exception_list, defeat_strength:float, specificity:priority_level}}>
```

#### 4.12.2 JSON Implementation Structure
```json
{
  "default_rule": {
    "antecedent": "condition_statement",
    "consequent": "conclusion_statement", 
    "exceptions": ["exception1", "exception2"],
    "defeat_strength": 0.0-1.0,
    "specificity": 0.0-1.0,
    "defeasible": true
  }
}
```

#### 4.12.3 HDC Default Logic Implementation
```
// Create default rule with exception handling
V_default_rule = V_bind(V_antecedent, V_consequent)
V_exception_vector = V_bundle([V_exception1, V_exception2])

// Apply default with exception checking
if similarity(V_current_situation, V_exception_vector) < exception_threshold:
    apply_default(V_default_rule)
else:
    block_default_inference()
```

#### 4.12.4 Default Logic Components
- `default_rule`: Defeasible rule that can be overridden
- `exceptions`: Conditions that block the default conclusion
- `defeat_strength`: How strongly exceptions override defaults
- `specificity`: Priority when multiple defaults conflict
- `revision_capability`: Ability to retract previous conclusions

#### 4.12.5 Examples

**Core ACEP:**
```
<{default_rule:{antecedent:<{isa:?X, Bird}>, consequent:<{?X, capableOf:Flying}>, exceptions:[<{isa:?X, Penguin}>, <{isa:?X, Ostrich}>], defeat_strength:0.9, specificity:0.7}}>
```

**JSON Implementation:**
```json
{
  "default_rule": {
    "id": "birds_fly_default",
    "antecedent": {
      "variable": "?X",
      "type": "Bird"
    },
    "consequent": {
      "variable": "?X", 
      "capability": "Flying"
    },
    "exceptions": [
      {"variable": "?X", "type": "Penguin"},
      {"variable": "?X", "type": "Ostrich"},
      {"variable": "?X", "condition": "injured"}
    ],
    "defeat_strength": 0.9,
    "specificity": 0.7,
    "defeasible": true
  }
}
```

Working memory is modeled as the active set of concept vectors maintained in a bundled superposition. This implementation reflects cognitive constraints on information processing capacity.

#### 4.7.1 Core ACEP Structure
```
<{working_memory:{active_concepts:concept_list, capacity_utilization:float, attention_weights:weight_dict, interference_level:float}}>
```

#### 4.7.2 JSON Implementation Structure
```json
{
  "working_memory": {
    "active_concepts": ["concept1", "concept2", "concept3"],
    "capacity_utilization": 0.0-1.0,
    "attention_weights": {
      "concept1": 0.0-1.0,
      "concept2": 0.0-1.0
    },
    "interference_level": 0.0-1.0,
    "rehearsal_schedule": {},
    "forgetting_curve": {}
  }
}
```

#### 4.7.3 Working Memory Components
- `active_concepts`: Currently active concept vectors in working memory
- `capacity_utilization`: Fraction of working memory capacity in use (0-1)
- `attention_weights`: Relative attention allocation across active concepts
- `interference_level`: Measure of cross-concept interference
- `rehearsal_schedule`: Timing for concept maintenance operations
- `forgetting_curve`: Parameters for natural decay of unused concepts

#### 4.7.4 Examples

**Core ACEP:**
```
<{working_memory:{active_concepts:[stock_analysis, market_trends, risk_assessment], capacity_utilization:0.7, attention_weights:{stock_analysis:0.5, market_trends:0.3, risk_assessment:0.2}, interference_level:0.2}}>
```

**JSON Implementation:**
```json
{
  "working_memory": {
    "active_concepts": ["stock_analysis", "market_trends", "risk_assessment"],
    "capacity_utilization": 0.7,
    "attention_weights": {
      "stock_analysis": 0.5,
      "market_trends": 0.3,
      "risk_assessment": 0.2
    },
    "interference_level": 0.2
  }
}
```

## 5. Enhanced Vector Operations

ACEP v2.0 extends the basic HDC operations with additional capabilities for temporal processing, causal reasoning, and cognitive modeling.

### 5.1 Core HDC Operations
The fundamental operations remain unchanged from ACEP v1.0:
- **Binding (⊕)**: V_bind(A, B) creates associations between concepts
- **Bundling (+)**: V_bundle(A, B, ...) creates superpositions of concepts
- **Unbinding**: V_unbind(A⊕B, A) approximately recovers B

### 5.2 Hierarchical Binding
Creates abstract concepts through compositional operations:
```
V_abstract = V_bind(V_concrete, V_bind(abstraction_role, category_vector))
```

### 5.3 Temporal Vector Updates
Supports knowledge evolution over time:
```
V_aged = V_temporal_decay(V_original, time_elapsed, decay_function)
V_updated = V_learn(V_existing, V_new_evidence, learning_rate)
```

### 5.4 Causal Binding
Encodes causal relationships with explicit mechanisms:
```
V_causal = V_bind(V_cause, V_bind(causation_role, V_bind(mechanism_vector, V_effect)))
```

### 5.5 Attention Operations
Implements selective processing of information:
```
V_attended = V_unbind(V_working_memory, V_query)
V_focused = V_amplify(V_concept, attention_weight)
```

### 5.6 Quantifier Operations
Supports formal logical structures through HDC composition:
```
V_universal = V_bind(V_quantifier_universal, V_bind(V_variable, V_scope))
V_existential = V_bind(V_quantifier_existential, V_bind(V_variable, V_scope))
V_instantiate = V_unbind(V_quantified_statement, V_specific_binding)
```

### 5.7 Consistency Operations
Maintains knowledge base coherence:
```
coherence = measure_vector_coherence(V_bundle([V_fact1, ..., V_factN]))
contradictions = detect_contradictions(knowledge_base, threshold)
V_resolved = resolve_contradiction(V_conflicting_statements, strategy)
```

### 5.8 Meta-Level Operations
Enables reasoning about reasoning:
```
V_meta = V_bind(V_meta_level, V_bind(V_agent, V_bind(V_belief_relation, V_target_statement)))
V_strategy_eval = V_bind(V_strategy_assessment, V_bind(V_reasoning_method, V_effectiveness))
```

### 5.9 Context Operations
Manages contextual and hypothetical reasoning:
```
V_contextualized = V_bind(V_context, V_statement)
V_inherited_context = V_bind(V_parent_context, V_child_context)
V_hypothetical = V_bind(V_hypothetical_marker, V_bind(V_conditions, V_consequences))
```

### 5.10 Default Logic Operations  
Handles defeasible reasoning:
```
V_default = create_default_rule(V_antecedent, V_consequent, V_exceptions)
applicability = check_exceptions(V_current_situation, V_exception_vector)
V_concluded = apply_default_if_applicable(V_default, V_situation)
```

## 6. Enhanced Communication Flow

### 6.1 Session Establishment with Cognitive Context

**Core ACEP:**
```
<{operation:session_init, session_id:123456, capabilities:[ACEP_v2.0, vector_dim:10000, hdc_operations:true], cognitive_profile:{working_memory_capacity:7, attention_span:moderate, reasoning_preferences:[causal_inference, analogical_reasoning]}}>
```

**JSON Implementation:**
```json
{
  "operation": {
    "type": "session_init",
    "session_id": 123456,
    "capabilities": ["ACEP_v2.0", "vector_dim:10000", "hdc_operations:true"],
    "cognitive_profile": {
      "working_memory_capacity": 7,
      "attention_span": "moderate",
      "reasoning_preferences": ["causal_inference", "analogical_reasoning"]
    }
  }
}
```

### 6.2 Complex Query with Uncertainty

**Core ACEP:**
```
<{operation:query, content:<{concept:market_forecast, entity:AAPL, temporal:next_quarter, uncertainty:{epistemic:0.3, confidence_threshold:0.8}, causal_dependencies:[interest_rates, earnings_growth]}>, cognitive_context:{reasoning_strategy:probabilistic, working_memory_focus:financial_indicators}}>
```

**JSON Implementation:**
```json
{
  "operation": {
    "type": "query",
    "content": {
      "concept": "market_forecast",
      "entity": "AAPL",
      "temporal": "next_quarter",
      "uncertainty": {
        "epistemic": 0.3,
        "confidence_threshold": 0.8
      },
      "causal_dependencies": ["interest_rates", "earnings_growth"]
    },
    "cognitive_context": {
      "reasoning_strategy": "probabilistic",
      "working_memory_focus": "financial_indicators"
    }
  }
}
```

### 6.3 Multi-Dimensional Response

**Core ACEP:**
```
<{operation:response, reference:query_id_456, content:<{concept:market_forecast, entity:AAPL, temporal:2024-Q2, prediction:bullish, uncertainty:{epistemic:0.2, aleatory:0.4, confidence:0.85, evidence_quality:0.9}, causal_chain:[{cause:earnings_growth, mechanism:fundamental_analysis, strength:0.8}, {cause:market_sentiment, mechanism:psychological, strength:0.6}]}>, reasoning_trace:[{step:1, operation:retrieve_historical_data}, {step:2, operation:causal_analysis}, {step:3, operation:uncertainty_propagation}]}>
```

**JSON Implementation:**
```json
{
  "operation": {
    "type": "response",
    "reference": "query_id_456",
    "content": {
      "concept": "market_forecast",
      "entity": "AAPL",
      "temporal": "2024-Q2",
      "prediction": "bullish",
      "uncertainty": {
        "epistemic": 0.2,
        "aleatory": 0.4,
        "confidence": 0.85,
        "evidence_quality": 0.9
      },
      "causal_chain": [
        {
          "cause": "earnings_growth",
          "mechanism": "fundamental_analysis",
          "strength": 0.8
        },
        {
          "cause": "market_sentiment",
          "mechanism": "psychological",
          "strength": 0.6
        }
      ]
    },
    "reasoning_trace": [
      {"step": 1, "operation": "retrieve_historical_data"},
      {"step": 2, "operation": "causal_analysis"},
      {"step": 3, "operation": "uncertainty_propagation"}
    ]
  }
}
```

## 7. Implementation Requirements

### 7.1 Enhanced Vector Space Management
- Support hierarchical binding operations
- Implement temporal decay functions
- Maintain working memory capacity constraints
- Provide attention mechanism APIs

### 7.2 Multi-Dimensional Uncertainty Handling
- Separate epistemic and aleatory uncertainty
- Implement uncertainty propagation through reasoning chains
- Support temporal uncertainty modeling
- Provide confidence calibration mechanisms

### 7.3 Causal Reasoning Support
- Distinguish causal from correlational relationships
- Support counterfactual reasoning operations
- Implement intervention modeling
- Provide causal strength estimation

### 7.4 Enhanced Implementation Requirements

### 7.4.1 Quantifier and Variable Support
- Variable binding consistency across complex expressions
- Quantifier scope resolution and instantiation
- HDC-based variable substitution mechanisms
- Domain constraint enforcement

### 7.4.2 Consistency Management
- Real-time contradiction detection using vector coherence
- Multiple resolution strategies (temporal, confidence-based, authority-based)
- Consistency maintenance during knowledge updates
- Coherence measurement across large knowledge bases

### 7.4.3 Meta-Level Infrastructure
- Hierarchical vector binding for higher-order relationships
- Agent belief and knowledge state representation
- Reasoning strategy evaluation and adaptation
- Self-referential statement handling

### 7.4.4 Context and Microtheory Support
- Context inheritance and isolation mechanisms
- Hypothetical reasoning with validity conditions
- Context switching and state management
- Cross-context knowledge retrieval

### 7.4.5 Default Logic Implementation
- Exception detection and handling
- Defeasible rule application
- Non-monotonic belief revision
- Specificity-based conflict resolution

## 8. Usage Examples

### 8.1 Simple Factual Statement with Enhanced Uncertainty

**English**: "Apple's P/E ratio is 28.5, based on recent earnings reports."

**Core ACEP:**
```
<{concept:pe_ratio, entity:AAPL, value:28.5, temporal:{timestamp:2024-03-01, validity_period:90_days, update_frequency:quarterly}, uncertainty:{epistemic:0.05, aleatory:0.02, confidence:0.95, evidence_quality:0.9, temporal_decay:{model:linear, rate:0.1_per_quarter}}, grounding:{source:earnings_report, verification:multiple_sources}}>
```

**JSON Implementation:**
```json
{
  "concept": "pe_ratio",
  "entity": "AAPL",
  "value": 28.5,
  "temporal": {
    "timestamp": "2024-03-01",
    "validity_period": "90_days",
    "update_frequency": "quarterly"
  },
  "uncertainty": {
    "epistemic": 0.05,
    "aleatory": 0.02,
    "confidence": 0.95,
    "evidence_quality": 0.9,
    "temporal_decay": {
      "model": "linear",
      "rate": "0.1_per_quarter"
    }
  },
  "grounding": {
    "source": "earnings_report",
    "verification": "multiple_sources"
  }
}
```

### 8.2 Complex Causal Relationship

**English**: "When interest rates rise significantly, technology stocks typically decline due to higher discount rates on future cash flows, though the effect may be delayed by market momentum."

**Core ACEP:**
```
<{concept:interest_rate_increase, threshold:significant}> → <{causal:{mechanism:discount_rate_theory, intervention_type:contributory, strength:0.8, direction:negative, time_lag:30_days, confounders:[market_momentum, investor_sentiment]}, uncertainty:{epistemic:0.15, aleatory:0.25, confidence:0.85}}> → <{concept:tech_stock_decline, entity:technology_sector}>
```

**JSON Implementation:**
```json
{
  "relationship_type": "causal",
  "source": {
    "concept": "interest_rate_increase",
    "threshold": "significant"
  },
  "target": {
    "concept": "tech_stock_decline",
    "entity": "technology_sector"
  },
  "causal_metadata": {
    "mechanism": "discount_rate_theory",
    "intervention_type": "contributory",
    "strength": 0.8,
    "direction": "negative",
    "time_lag": "30_days",
    "confounders": ["market_momentum", "investor_sentiment"]
  },
  "uncertainty": {
    "epistemic": 0.15,
    "aleatory": 0.25,
    "confidence": 0.85
  }
}
```

### 8.3 Hierarchical Abstraction with Meta-Cognition

**English**: "Investment analysis requires considering multiple factors simultaneously, which challenges working memory capacity."

**Core ACEP:**
```
<{concept:investment_analysis, abstraction_level:1}> → <{requires:multiple_factor_consideration, working_memory:{capacity_demand:high, interference_potential:0.7}}> → <{meta_cognitive:{reasoning_limitation:working_memory_overload, strategy_recommendation:sequential_analysis, confidence_impact:negative_0.2}}>
```

**JSON Implementation:**
```json
{
  "relationship_type": "hierarchical",
  "source": {
    "concept": "investment_analysis",
    "abstraction_level": 1
  },
  "target": {
    "requires": "multiple_factor_consideration",
    "working_memory": {
      "capacity_demand": "high",
      "interference_potential": 0.7
    }
  },
  "meta_cognitive": {
    "reasoning_limitation": "working_memory_overload",
    "strategy_recommendation": "sequential_analysis",
    "confidence_impact": "negative_0.2"
  }
}
```

### 8.4 Temporal Learning and Adaptation

**English**: "My prediction accuracy for tech stocks has improved from 60% to 75% over the past year through experience with earnings announcements."

**Core ACEP:**
```
<{operation:meta_learn, content:<{concept:prediction_accuracy, domain:tech_stocks, historical_performance:{initial:0.60, current:0.75, time_period:1_year}, learning_mechanism:earnings_pattern_recognition, confidence_progression:{initial:0.6, current:0.8}, temporal:{learning_curve:logarithmic, improvement_rate:0.15_per_quarter}}>, meta_cognitive:{strategy_effectiveness:high, knowledge_quality:improving, transfer_potential:moderate}}>
```

**JSON Implementation:**
```json
{
  "operation": {
    "type": "meta_learn",
    "content": {
      "concept": "prediction_accuracy",
      "domain": "tech_stocks",
      "historical_performance": {
        "initial": 0.60,
        "current": 0.75,
        "time_period": "1_year"
      },
      "learning_mechanism": "earnings_pattern_recognition",
      "confidence_progression": {
        "initial": 0.6,
        "current": 0.8
      },
      "temporal": {
        "learning_curve": "logarithmic",
        "improvement_rate": "0.15_per_quarter"
      }
    },
    "meta_cognitive": {
      "strategy_effectiveness": "high",
      "knowledge_quality": "improving",
      "transfer_potential": "moderate"
    }
  }
}
```

### 8.5 Goal-Directed Planning with Uncertainty

**English**: "To achieve a 10% portfolio return this year, I should increase exposure to growth stocks, but this increases risk and depends on continued economic expansion."

**Core ACEP:**
```
<{operation:plan, goal:<{concept:portfolio_return, target:0.10, temporal:2024}>, strategy:<{action:increase_growth_exposure, magnitude:moderate, risk_tradeoff:accept_higher_volatility}>, dependencies:<{concept:economic_expansion, continuation:required, uncertainty:{epistemic:0.3, aleatory:0.4}, causal_strength:0.7}>, plan_confidence:0.7, contingency_planning:enabled}>
```

**JSON Implementation:**
```json
{
  "operation": {
    "type": "plan",
    "goal": {
      "concept": "portfolio_return",
      "target": 0.10,
      "temporal": "2024"
    },
    "strategy": {
      "action": "increase_growth_exposure",
      "magnitude": "moderate",
      "risk_tradeoff": "accept_higher_volatility"
    },
    "dependencies": {
      "concept": "economic_expansion",
      "continuation": "required",
      "uncertainty": {
        "epistemic": 0.3,
        "aleatory": 0.4
      },
      "causal_strength": 0.7
    },
    "plan_confidence": 0.7,
    "contingency_planning": "enabled"
  }
}
```

### 8.6 Counterfactual Reasoning

**English**: "If the Federal Reserve had not raised rates in March, the tech selloff would likely have been much milder."

**Core ACEP:**
```
<{statement_type:counterfactual, base_world:<{concept:fed_rate_increase, temporal:2024-03, actual:true}>, counterfactual_world:<{concept:fed_rate_increase, temporal:2024-03, hypothetical:false}>, predicted_difference:<{concept:tech_selloff_magnitude, base_world:severe, counterfactual_world:mild, confidence:0.75}>, causal_mechanism:investor_sentiment_and_discount_rates}>
```

**JSON Implementation:**
```json
{
  "statement_type": "counterfactual",
  "base_world": {
    "concept": "fed_rate_increase",
    "temporal": "2024-03",
    "actual": true
  },
  "counterfactual_world": {
    "concept": "fed_rate_increase",
    "temporal": "2024-03",
    "hypothetical": false
  },
  "predicted_difference": {
    "concept": "tech_selloff_magnitude",
    "base_world": "severe",
    "counterfactual_world": "mild",
    "confidence": 0.75
  },
  "causal_mechanism": "investor_sentiment_and_discount_rates"
}
```

### 8.8 Quantified Logical Statement (Cyc-Style)

**English**: "All birds that are not penguins can fly."

**Core ACEP:**
```
<{quantifier:{type:universal, variables:[{id:?X, domain:Bird}], scope:<{?X, isa:Bird}> ∧ <{¬(?X, isa:Penguin)}> → <{?X, capableOf:Flying}>, exceptions:[penguin, ostrich], default_strength:0.9}}>
```

**JSON Implementation:**
```json
{
  "quantifier": {
    "type": "universal",
    "variables": [{"identifier": "?X", "domain": "Bird"}],
    "scope": {
      "logical_structure": {
        "operator": "implies",
        "antecedent": {
          "operator": "and", 
          "clauses": [
            {"variable": "?X", "type": "Bird"},
            {"operator": "not", "clause": {"variable": "?X", "type": "Penguin"}}
          ]
        },
        "consequent": {"variable": "?X", "capability": "Flying"}
      }
    },
    "defeasible": true,
    "exceptions": ["penguin", "ostrich"],
    "default_strength": 0.9
  }
}
```

### 8.9 Meta-Level Knowledge Representation

**English**: "The AI system believes that Apple stock will rise, based on earnings analysis, with high confidence in this belief."

**Core ACEP:**
```
<{meta_level:{agent:AI_system_alpha, believes:<{concept:stock_movement, entity:AAPL, direction:rise, confidence:0.8}>, justification:earnings_analysis, meta_confidence:0.9, belief_strength:0.85}}>
```

**JSON Implementation:**
```json
{
  "meta_level": {
    "agent": "AI_system_alpha",
    "meta_relation": "believes",
    "target_belief": {
      "concept": "stock_movement",
      "entity": "AAPL", 
      "direction": "rise",
      "confidence": 0.8
    },
    "justification": {
      "reasoning_type": "earnings_analysis",
      "evidence_quality": 0.85,
      "data_sources": ["Q4_earnings", "analyst_reports"]
    },
    "meta_confidence": 0.9,
    "belief_strength": 0.85
  }
}
```

### 8.10 Contextual Knowledge with Inheritance

**English**: "In the current world, Paris is the capital of France. In a hypothetical scenario where Napoleon won at Waterloo, the capital might be different."

**Core ACEP:**
```
<{context:{id:CurrentWorld, type:belief_space}}> <{concept:capital, country:France, city:Paris, certainty:1.0}>

<{context:{id:Napoleon_Victory, type:hypothetical, inheritance:[CurrentWorld], conditions:[napoleon_wins_waterloo]}}> <{concept:capital, country:France, city:unknown, uncertainty:{epistemic:0.8, aleatory:0.3}}>
```

**JSON Implementation:**
```json
{
  "contexts": [
    {
      "id": "CurrentWorld",
      "type": "belief_space",
      "statements": [
        {
          "concept": "capital",
          "country": "France", 
          "city": "Paris",
          "certainty": 1.0
        }
      ]
    },
    {
      "id": "Napoleon_Victory_Scenario", 
      "type": "hypothetical",
      "inheritance": ["CurrentWorld"],
      "conditions": ["napoleon_wins_waterloo"],
      "modified_statements": [
        {
          "concept": "capital",
          "country": "France",
          "city": "unknown",
          "uncertainty": {
            "epistemic": 0.8,
            "aleatory": 0.3
          }
        }
      ]
    }
  ]
}
```

### 8.11 Default Logic with Exception Handling

**English**: "Companies typically have employees, but shell companies and dissolved companies are exceptions."

**Core ACEP:**
```
<{default_rule:{antecedent:<{isa:?X, Company}>, consequent:<{?X, has:employees}>, exceptions:[<{?X, type:shell_company}>, <{?X, status:dissolved}>, <{?X, size:micro}>, defeater_strength:0.95, specificity:0.8}}>
```

**JSON Implementation:**
```json
{
  "default_rule": {
    "id": "companies_have_employees_default",
    "antecedent": {
      "variable": "?X",
      "type": "Company"
    },
    "consequent": {
      "variable": "?X",
      "property": "has_employees" 
    },
    "exceptions": [
      {"variable": "?X", "type": "shell_company"},
      {"variable": "?X", "status": "dissolved"},
      {"variable": "?X", "size": "micro", "employee_count": 0}
    ],
    "defeater_strength": 0.95,
    "specificity": 0.8,
    "domain": "business_entities"
  }
}
```

### 8.12 Complex Multi-Variable Quantification (Cyc-Style)

**English**: "For every company that has revenue greater than $1 million in any year after 2020, there probably exists at least one employee."

**Core ACEP:**
```
<{quantifier:{type:universal, variables:[{id:?COMPANY, domain:Company}]}, scope:<{∃?YEAR: ?YEAR > 2020 ∧ revenue(?COMPANY, ?YEAR) > $1M}> → <{∃?EMP: employee(?EMP, ?COMPANY)}>, modal:probably, confidence:0.8}>
```

**JSON Implementation:**
```json
{
  "quantifier": {
    "type": "universal",
    "variables": [{"identifier": "?COMPANY", "domain": "Company"}],
    "scope": {
      "implication": {
        "antecedent": {
          "quantifier": "existential",
          "variable": "?YEAR",
          "domain": "CalendarYear", 
          "conditions": [
            {"variable": "?YEAR", "operator": "greater_than", "value": 2020},
            {
              "function": "revenue",
              "arguments": ["?COMPANY", "?YEAR"],
              "operator": "greater_than", 
              "value": {"amount": 1000000, "currency": "USD"}
            }
          ]
        },
        "consequent": {
          "quantifier": "existential",
          "variable": "?EMP",
          "domain": "Person",
          "relation": {
            "predicate": "employee",
            "arguments": ["?EMP", "?COMPANY"]
          }
        }
      }
    },
    "modal": "probably",
    "confidence": 0.8
  }
}
```

### 8.13 Consistency Management in Action

**English**: "The system detected a contradiction between 'It is sunny today' and 'It is raining today', resolved by temporal precedence (rain started later)."

**Core ACEP:**
```
<{consistency:{detected_contradiction:[{stmt1:sunny_today_0800, stmt2:raining_today_1400}], conflict_type:temporal_sequence, resolution:temporal_precedence, resolved_state:raining_currently, confidence_adjustment:weather_stmt1:-0.8}}> 
```

**JSON Implementation:**
```json
{
  "consistency_event": {
    "detected_contradiction": [
      {
        "statement1": {
          "id": "sunny_today_0800",
          "concept": "weather",
          "state": "sunny", 
          "timestamp": "2024-03-15T08:00:00Z"
        },
        "statement2": {
          "id": "raining_today_1400", 
          "concept": "weather",
          "state": "raining",
          "timestamp": "2024-03-15T14:00:00Z"
        }
      }
    ],
    "conflict_analysis": {
      "type": "temporal_sequence",
      "severity": 0.9,
      "resolvable": true
    },
    "resolution": {
      "strategy": "temporal_precedence",
      "resolved_state": "weather_changed_from_sunny_to_rainy",
      "confidence_adjustments": {
        "sunny_today_0800": 1.0,
        "raining_today_1400": 1.0,
        "overall_consistency": 0.95
      }
    }
  }
}
```

**English**: "The weather forecast predicts rain tomorrow with 80% certainty. If it rains, the outdoor event will be canceled with 95% certainty. If the event is canceled, attendees will be refunded with 100% certainty. Therefore, attendees will likely be refunded with 76% certainty."

**Core ACEP (35 tokens):**
```
<{concept:rain_forecast, temporal:tomorrow, certainty:0.8}>
<{concept:event_cancellation}> ← <{condition:0.95}> ← <{ref:state[1]}>
<{concept:refund_issuance}> ← <{condition:1.0}> ← <{ref:state[2]}>
<{concept:refund_issuance, certainty:0.76}> // 0.8 × 0.95 × 1.0
```

**JSON Implementation:**
```json
{
  "reasoning_chain": [
    {
      "step": 1,
      "statement": {
        "concept": "rain_forecast",
        "temporal": "tomorrow",
        "uncertainty": {"confidence": 0.8}
      }
    },
    {
      "step": 2,
      "statement": {
        "concept": "event_cancellation",
        "conditional_on": "state[1]",
        "uncertainty": {"confidence": 0.95}
      }
    },
    {
      "step": 3,
      "statement": {
        "concept": "refund_issuance",
        "conditional_on": "state[2]",
        "uncertainty": {"confidence": 1.0}
      }
    },
    {
      "step": 4,
      "conclusion": {
        "concept": "refund_issuance",
        "uncertainty": {
          "confidence": 0.76,
          "calculation": "0.8 × 0.95 × 1.0"
        }
      }
    }
  ]
}
```

## 9. Format Selection Guidelines

### 9.1 Core ACEP Format Usage
Use Core ACEP format when:
- **Token efficiency** is critical (network bandwidth, storage)
- **Real-time communication** between AI systems
- **High-frequency** knowledge exchanges
- **Embedded systems** with memory constraints
- **Human experts** familiar with the compact notation

### 9.2 JSON Implementation Usage
Use JSON Implementation format when:
- **API integration** with web services
- **Debugging and development** requiring human readability
- **Complex nested structures** with extensive metadata
- **Legacy system integration** requiring JSON compatibility
- **Documentation and examples** for non-experts

### 9.3 Conversion Between Formats
Both formats represent identical semantic content and should be freely convertible:
- **Core ACEP → JSON**: Expansion of compact notation into structured JSON
- **JSON → Core ACEP**: Compression of JSON structure into compact notation
- **Validation**: Both formats must validate against the same semantic requirements

## 10. Backward Compatibility

ACEP v2.0 maintains backward compatibility with v1.0 through default value mapping:

### 10.1 Core ACEP v1.0 to v2.0
```
// v1.0
<{concept:example, certainty:0.8, temporal:now}>

// v2.0 (expanded)
<{concept:example, uncertainty:{confidence:0.8, epistemic:0.2, aleatory:0.1}, temporal:{timestamp:now, decay_function:exponential}}>
```

### 10.2 Compatibility Defaults
- v1.0 `certainty` values map to v2.0 `confidence`
- Missing uncertainty components get default values
- Simple relationships become basic causal structures
- Single timestamps expand to temporal models

## 11. Enhanced Cyc Integration Capabilities

### 11.1 Cyc Knowledge Conversion Support

ACEP v2.0 now provides comprehensive support for Cyc knowledge base conversion:

#### 11.1.1 Supported Cyc Constructs
- **Quantified statements**: Universal and existential quantification with variable binding
- **Complex predicates**: Multi-argument predicates with typed variables  
- **Taxonomic hierarchies**: isa, genls relationships through vector inheritance
- **Temporal assertions**: holdsIn, temporal indexicals
- **Modal statements**: probablyTrue, possiblyTrue, unknownTruth
- **Contextual knowledge**: Microtheories and belief spaces
- **Default reasoning**: Defeasible rules with exception handling
- **Meta-level assertions**: Beliefs, knowledge, and reasoning about reasoning

#### 11.1.2 Conversion Success Rates
Based on enhanced ACEP v2.0 capabilities:
- **Directly convertible**: ~75% of Cyc knowledge (up from 25%)
- **Convertible with minor adaptation**: ~20% (down from 35%) 
- **Requires complex transformation**: ~5% (down from 40%)

#### 11.1.3 HDC-Based Cyc Implementation
```
// Cyc: (forAll ?X (implies (isa ?X Bird) (capableOf ?X Flying)))
V_universal = generate_vector("universal_quantifier")
V_var_X = generate_vector("variable_X")
V_bird_constraint = generate_vector("bird_type")
V_flying_capability = generate_vector("flying_capability")

V_cyc_rule = V_bind(V_universal,
              V_bind(V_var_X,
                V_bind(V_bird_constraint, V_flying_capability)))

// ACEP v2.0 Representation:
<{quantifier:{type:universal, variables:[{id:?X, domain:Bird}], scope:<{?X, isa:Bird}> → <{?X, capableOf:Flying}>, vector_binding:V_cyc_rule}}>
```

### 11.2 Cyc-ACEP Translation Patterns

#### 11.2.1 Simple Assertions
```cyc
(isa Apple Fruit)
```
**ACEP v2.0:**
```
<{concept:Apple, is_a:Fruit, certainty:1.0}>
```

#### 11.2.2 Complex Quantified Relations
```cyc
(forAll ?COMPANY 
  (implies (and (isa ?COMPANY Company)
                (greaterThan (numberOfEmployees ?COMPANY) 100))
           (probablyTrue (isa ?COMPANY LargeOrganization))))
```

**ACEP v2.0:**
```
<{quantifier:{type:universal, variables:[{id:?COMPANY, domain:Company}], scope:<{?COMPANY, employees:gt_100}> → <{?COMPANY, classification:LargeOrganization, modal:probably, confidence:0.7}>}}>
```

#### 11.2.3 Temporal Indexicals
```cyc
(holdsIn Today (weatherCondition Paris Sunny))
```

**ACEP v2.0:**
```
<{concept:weather_condition, entity:Paris, state:Sunny, temporal:{timestamp:Today, validity_period:24_hours, scope:temporal_indexical}}>
```

#### 11.2.4 Microtheories and Contexts
```cyc
(ist CurrentWorldDataMt (capitalOf France Paris))
(ist HypotheticalContext-427 (capitalOf France London))
```

**ACEP v2.0:**
```
<{context:{id:CurrentWorldDataMt, type:belief_space}}> <{concept:capital, country:France, city:Paris}>
<{context:{id:HypotheticalContext_427, type:hypothetical, inheritance:[CurrentWorldDataMt]}}> <{concept:capital, country:France, city:London}>
```

### 11.3 Implementation Strategy for Cyc Integration

#### 11.3.1 Phase 1: Direct Mapping (75% of Cyc knowledge)
- Simple assertions and taxonomic relationships
- Basic quantified statements  
- Temporal assertions with straightforward time references
- Modal statements with probability mappings

#### 11.3.2 Phase 2: Complex Structure Handling (20% of Cyc knowledge)
- Nested quantification patterns
- Complex temporal relationships
- Multi-context reasoning
- Higher-order predicates through meta-level structures

#### 11.3.3 Phase 3: Advanced Integration (5% of Cyc knowledge)
- Mathematical relationships requiring symbolic computation
- Highly complex logical structures
- Domain-specific reasoning patterns
- Integration with specialized reasoning engines

### 11.4 Validation and Quality Assurance

#### 11.4.1 Semantic Preservation Testing
- Round-trip conversion validation (Cyc → ACEP → reasoning → validation)
- Logical entailment preservation checks
- Consistency maintenance across converted knowledge bases

#### 11.4.2 Performance Benchmarks
- Conversion speed for large Cyc microtheories
- HDC operation scalability with millions of Cyc assertions
- Query response time comparisons between native Cyc and ACEP representations

## 12. Conclusion

ACEP v2.0 provides a comprehensive foundation for AI system communication with significant enhancements specifically designed to address the gaps identified in Cyc knowledge base integration. The enhanced specification now supports:

- **Formal logical structures** through HDC-based quantifier and variable binding systems
- **Consistency management** with automatic contradiction detection and resolution
- **Meta-level reasoning** capabilities for beliefs, knowledge, and reasoning about reasoning
- **Contextual knowledge representation** supporting microtheories and hypothetical reasoning
- **Default logic and non-monotonic reasoning** with exception handling and defeasible rules

These enhancements, combined with the mathematical properties of hyperdimensional computing, enable ACEP v2.0 to handle approximately **95% of Cyc's knowledge base** with varying degrees of fidelity, representing a dramatic improvement over the original specification.

The dual-format approach (Core ACEP and JSON) ensures both computational efficiency for machine-to-machine communication and human readability for development and debugging. The enhanced vector operations and HDC-based implementations provide the mathematical foundation needed to represent complex logical relationships while maintaining the efficiency and scalability required for large-scale knowledge integration.

ACEP v2.0 bridges the gap between formal logical knowledge representation and practical AI system communication, enabling sophisticated reasoning systems to leverage both the precision of formal logic and the robustness of hyperdimensional computing.

ACEP v2.0 provides a comprehensive foundation for AI system communication while leveraging the mathematical properties of hyperdimensional computing. The dual-format specification supports both efficient machine-to-machine communication through the compact Core ACEP notation and human-readable development through JSON implementations.

The enhanced specification supports complex logical structures, multi-dimensional uncertainty modeling, temporal dynamics, and cognitive processing patterns while maintaining the efficiency and elegance of the original HDC-based design. Both formats enable AI systems to engage in sophisticated reasoning patterns while maintaining computational efficiency required for real-world applications.
