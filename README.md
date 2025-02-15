# Polymer DeepChem Integration Project

This project focuses on the integration of polymer support within the DeepChem ecosystem. The integration process began with the Google Summer of Code (GSoC) 2024 project and has been extended into a workshop paper. The project includes various PR contributions and an extended pipeline implementation to support polymer featurization and generation.

## Contributions and PRs

### Base Polymer Featurizer and Weighted Directed Graph Classes
- A base polymer featurizer class was created to handle polymer representations within the DeepChem framework.
- A weighted directed graph data class was introduced to represent polymers as graphs.
- The creation of utility functions to generate graph-based featurizers.
- Tests were added to ensure the correctness of these classes.

### Modular Changes and Improvements
- The bulk changes were split into several modular PRs, including base polymer featurizer, weighted directed data classes, and data validator classes.
- Tests and documentation were added across all modules.
- Fixes were implemented for pytest and adaptation to newer XGBoost versions.

### Tutorials and Exploratory Work
- A tutorial was created focusing on the implementation of DeepChem models to predict the crystallization tendency of polymers.
- A separate tutorial was added explaining the weighted directed graph featurization and its real-world implications for polymer research.
- A PSMILES tutorial was developed, explaining their formation and tokenization.
- Tutorials were created for the application of PolyBERT for similarity prediction of polymer molecules.

### Extended Work and Research
- A set of generators were developed to align with DeepChem discriminators for generating valid candidates with desired properties.
- The pipeline for generation was integrated into DeepChem.
- The research results were presented at the AI2ASE workshop at the 39th AAAI Annual Conference and published in a research paper.

### Key PR Contributions

*Note- These following PRs were raised on [DeepChem](https://github.com/deepchem/deepchem) github repository.*

- **#3984**: Base polymer featurizer and weighted directed graph data classes with documentation and tests.
- **#3992**: Utility functions for generating graph-based featurizers.
- **#4016**: Base polymer featurizer with additional unit test cases.
- **#4017**: Weighted directed data classes with added documentation.
- **#4020**: Weighted directed data validator classes with unit test cases.
- **#4021**: Utility functions for weighted directed graph data formation.
- **#4070**: Tutorial for predicting crystallization tendency of polymers.
- **#4088**: Tutorial on weighted-directed graph implementation for polymers.
- **#4097**: Tutorial on PSMILES formation and tokenization.
- **#4105**: Tutorial on using PolyBERT for similarity prediction.
- **#4246**: Integration of LSTM generator for SMILES and PSMILES generation.
- **#4252**: Integration of BRICS sampler for reaction-based generation.
- **#4267**: Conversion mechanism between PSMILES and weighted directed graphs.
- **#4276**: Tutorial for reproducibility of the candidate generation using DeepChem generators.
- **#4289**: Tutorial explaining the conversion between PSMILES and weighted directed graphs.

## Research Paper
- The project resulted in a research paper to be presented at the AI2ASE workshop at the AAAI Annual Conference. The paper can be accessed [here](https://arxiv.org/html/2412.08658v1).

- Demo GitHub Repository: [Polymer Pipelines Demo](https://github.com/TRY-ER/polymer_pipelines.git)

