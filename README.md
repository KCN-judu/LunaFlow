# LunaFlow Project Plan & Introduction
LunaFlow - A Scientific Computing Ecosystem Built for MoonBit.
**This repository doesn't contain any LunaFlow source code.**
**It is only for project introduction and repository navigation.**
## Introduction
### Background

As the MoonBit language evolves, building a complete scientific computing ecosystem is crucial for research computing, engineering applications, and even machine learning. The goal of LunaFlow is to provide an efficient, flexible, and extensible scientific computing framework that supports numerical computation, symbolic computation, and probability statistics, thereby strengthening the mathematical capabilities of the MoonBit ecosystem.

### Objectives

LunaFlow's development is structured into three phases, gradually establishing a comprehensive ecosystem from fundamental mathematical operations to advanced scientific computing applications.

### **Phase Plan**

#### **Phase 1: Core Dependency Development**

The first phase focuses on building essential mathematical libraries that serve as the foundation for subsequent modules:

1. **math library**: Implements fundamental mathematical functions, including numerical operations, elementary functions, and special functions.
2. **utils library**: Provides general mathematical utilities such as numerical format conversion and auxiliary functions for vector/matrix operations.
3. **linear-algebra library**: Built upon the math and utils libraries, this module supports matrix operations, linear algebra fundamentals, matrix decomposition, inversion, eigenvalue computation, etc.
4. **calculus-numerical library**: Develops numerical calculus functionalities, including numerical integration, differentiation, and interpolation.

#### **Phase 2: Symbolic Computation & Probability Statistics**

The second phase extends beyond numerical computation into symbolic mathematics and statistical analysis:

1. **calculus-symbolic library**: Supports symbolic differentiation, integration, expression parsing, simplification, and equation solving.
2. **probability-statistics library**: Provides functionalities for probability distributions, statistical analysis, and stochastic processes, supporting data science and machine learning applications.

#### **Phase 3: Domain-Specific Scientific Applications**

Building on the numerical and symbolic computation capabilities from **Phase 1** and **Phase 2**, the third phase will focus on developing applied scientific computing solutions across various domains:

1. **Physics Simulations**: Implement computational tools for classical mechanics, electromagnetism, quantum mechanics, and other physical models, leveraging numerical solvers and symbolic computation.
2. **Financial Mathematics**: Develop models for risk analysis, option pricing, stochastic processes, and quantitative finance applications.
3. **Mathematical Modeling**: Apply LunaFlow’s capabilities to solve real-world mathematical problems, including differential equations, optimization, and algebraic systems.
4. **Other Scientific and Engineering Applications**: Expand LunaFlow’s use cases to fields such as control systems, bioinformatics, and machine learning, integrating with external datasets and computational frameworks where needed.

### **Current Progress & Next Steps**

#### **Current Progress**

LunaFlow is currently in **Phase 1**, focusing on building core dependencies. Initially, the **utils, math, and linear-algebra** libraries were developed alongside **calculus-numerical**. However, this structure has proven inefficient, leading to a decision to **separate these foundational dependencies into independent modules** for better modularity and maintainability.

- **linear-algebra**: Originally integrated with calculus-numerical, now being extracted as a standalone module.
- **utils**: Developed in parallel with calculus-numerical, also being separated into its own module.
- **math**: Under evaluation for potential replacement with an existing library to avoid redundant development.

#### **Next Steps**

1. **Complete the separation of utils and linear-algebra** into independent modules, ensuring clear interfaces and reducing coupling.
2. **Finalize the evaluation of math dependencies** and decide whether to adopt an external library or develop a customized solution.
3. **Refactor calculus-numerical** to integrate with the newly structured modules, maintaining efficiency and modularity.
4. **Implement and validate numerical calculus functions**, ensuring correctness through comprehensive testing.

This restructuring will create a **robust foundation for Phase 2**, enabling efficient development of symbolic calculus and probability/statistics functionalities.