# A grammar-driven and decoupled abstract syntax tree for Xtext

The thesis itself: [PDF](thesis.pdf).

The corresponding implementation is in this branch: https://github.com/mischnic/xtext-core/tree/nmischkulnig/cst-ast.


Abstract:
> Xtext is a framework for implementing editors and compilers for domain-specific languages. It works similar to traditional grammar-based parser generators but also automatically generates a class model from the parser rules in the grammar. However, this model is not very customizable if the intended abstract syntax tree differs from the concrete syntax. This becomes an even bigger concern if the grammar has to be refactored to resolve parsing ambiguities or left recursion. Traditionally the AST and mapping code would be specified separately from the grammar leading to duplicated code that is hard to maintain. Instead, we present a way to declare the structure of the AST directly inside the concrete syntax grammar. To keep the grammar readable, the attributes are specified in relation to the model inferred by Xtext. This allows for the automatic generation of mapping code and also leveraging the Xtext class model information for a majority of the AST nodes while still supporting custom AST classes with additional attributes and mapping code performing arbitrary computations including mapping a node to a list of nodes.
