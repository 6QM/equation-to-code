# Equation to Code

**Problem awareness → history → first principles → equations → experiments → working code → proof of work.**

Equation to Code is a public problem lab for understanding important ideas in mathematics, physics, engineering, and computation. Each project begins with a question worth asking, reconstructs the context and reasoning behind it, and moves toward models, numerical experiments, or software that can be inspected and run.

This is not a CFD-only repository. Fluid mechanics and heat transfer are natural starting points, but the method also applies to differential equations, numerical analysis, linear algebra, control, optimization, scientific computing, and other technical subjects.

## Why this repository exists

Technical learning is often split across biographies, textbooks, handwritten derivations, notebooks, and code. That fragmentation makes it difficult to see how an idea developed—or to verify that it has truly been understood.

This repository keeps the chain of reasoning intact:

1. **Ask a precise question.** What are we trying to understand, and why does it matter?
2. **Recover the context.** Which practical or intellectual problem made the idea necessary?
3. **Rebuild from first principles.** State assumptions and derive the essential relationships.
4. **Turn relationships into models.** Identify equations, closures, boundary conditions, and approximations.
5. **Test the model.** Use small numerical experiments, limiting cases, and reference solutions.
6. **Build something runnable.** Produce clear code, a solver, a visualization, or another inspectable artifact.
7. **Record what remains uncertain.** Separate evidence, interpretation, and open questions.

Not every investigation must reach code. The goal is an honest, traceable progression from curiosity to a result that another person can examine.

## Proof of work

The repository itself is a growing record of work, not a stream of claims about learning. Here, **proof of work** means the inspectable evidence left behind by an investigation:

- a question framed precisely enough to be challenged;
- source notes that show where factual and historical claims came from;
- derivations whose assumptions and intermediate steps are visible;
- notebooks or code that another person can run;
- tests, limiting cases, convergence studies, or benchmark comparisons;
- selected results with inputs, units, and reproduction instructions;
- a record of errors, revisions, and remaining uncertainty.

The standard is not that every project contains every artifact. The standard is that its conclusion is supported by appropriate evidence. In this sense, **problem awareness is the starting point, equation to code is the method, and proof of work is the output**.

## Repository map

| Area | Purpose |
| --- | --- |
| [`questions/`](questions/) | Complete investigations organized around specific questions rather than academic departments. |
| [`people-and-ideas/`](people-and-ideas/) | The historical development of ideas, emphasizing problems, assumptions, disagreements, and conceptual advances. |
| [`equation-to-code/`](equation-to-code/) | Focused implementations that map mathematical models and numerical schemes into tested code. |
| [`builds/`](builds/) | Larger artifacts: solvers, tools, interactive demonstrations, and integrated projects. |
| [`maps/`](maps/) | Concept maps, timelines, dependency maps, and reading paths across investigations. |
| [`references/`](references/) | Curated bibliographies, source notes, datasets, and conventions used across the repository. |

## What a strong investigation contains

A substantial question should make its evidence and reasoning easy to audit. A typical project may include:

```text
questions/why-does-finite-volume-conserve/
├── README.md              # question, answer, assumptions, and narrative
├── derivation.md          # equations and derivation details
├── experiment.ipynb      # executable exploration
├── src/                  # reusable implementation
├── tests/                # analytical, benchmark, or regression checks
├── results/              # selected tables and figures
└── references.md         # sources tied to specific claims
```

Use only the pieces the question requires. A concise, verified investigation is better than an elaborate but unfinished package.

## Working principles

- **Questions before categories.** Organize work around what needs to be understood.
- **Context before symbolism.** Explain why a model exists before manipulating its equations.
- **Assumptions in the open.** State what is idealized, omitted, or uncertain.
- **Derivation connected to implementation.** Make it possible to trace a term in an equation to its role in code.
- **Verification over impressive output.** Prefer limiting cases, conservation checks, manufactured solutions, and benchmark comparisons.
- **Reproducibility by default.** Record inputs, units, dependencies, and commands needed to reproduce a result.
- **Sources close to claims.** Distinguish primary sources, later interpretation, and personal synthesis.

## Possible starting questions

- How did the Navier–Stokes equations emerge, and which assumptions entered at each stage?
- Why does the finite-volume method conserve fluxes locally and globally?
- What makes a numerical scheme stable, and what does “stable” fail to guarantee?
- How does SIMPLE couple pressure and velocity when pressure has no standalone transport equation?
- Why are some partial differential equations easier to solve than others?

## Status

The repository begins as a scaffold. Investigations will be added incrementally, and its structure may evolve as the work reveals better ways to connect history, theory, experiments, and code.

## License

Code and original written material in this repository are available under the [MIT License](LICENSE). Third-party sources, quotations, datasets, and images retain their respective rights and should be credited where used.
