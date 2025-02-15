I am working on a project with DeepChem to integrate polymer support into their ecosystem, it started from the gsoc and extended after that till a workshop paper. below is the gsoc archive "

# GSoC-24-Archive @Deepchem 
By: Debasish Mohanty

# PR Timeline 

The following PRs were made in the given hierarchy as part of the GSoC'24 project in the [DeepChem](https://github.com/deepchem/deepchem) repository.

## Week - 0 (27.05.2024 - 03.06.2024)

  - PR – [#3984](https://github.com/deepchem/deepchem/pull/3984) (Status : Splitted Into 2 PRs Later)
    -  A base polymer featurizer class is created
    -  A weighted directed graph data class is created
    -  Fixed linting and added documentation
    -  Tests were added for the above classes

  - PR – [#3992](https://github.com/deepchem/deepchem/pull/3992) (Status : Will be considered while Complete Pipeline Integration)
    -  An utils file is created to store utility functions for generating graph based featurizer
    -  Fixed linting and added documentation for the same
    -  Tests were added for utility functions

## Week - 1 (03.06.2024 - 10.06.2024)
  - Previous PRs were fixed

## Week - 2 (10.06.2024 - 17.06.2024)
  - Previous PRs were reviewed

## Week - 3 (17.06.2024 - 24.06.2024)  

  - Splitted the bulk PRs raised before into 4 PR with modular changes
    - PR – [#4016](https://github.com/deepchem/deepchem/pull/4016) (Status: Merged on July 3rd) ✅
      - PR for base polymer featurizer with added unit test cases
        
    - PR – [#4017](https://github.com/deepchem/deepchem/pull/4017)  (Status : Merged on July 8th) ✅
      - PR for weighted directed data classes with added documentation
        
    - PR – [#4020](https://github.com/deepchem/deepchem/pull/4020)  (Status : Merged on Oct 14th ) ✅
      -  PR for weighted directed data validator classes with splitted unit-cases

    - PR – [#4021](https://github.com/deepchem/deepchem/pull/4021)  (Status : Will be considered while Complete Pipeline Integration)
       - PR for utils functions for weighted directed graph data formation

    - PR – [#4023](https://github.com/deepchem/deepchem/pull/4023)  (Status : Merged on June 24) ✅
      - PR for fixing pytest in unit-tests by adapting codebase to newer xgboost version

## Week - 4 (24.06.2024 - 01.07.2024)

  - PR - #4016 was rebased and reviewed

## Week - 5 (01.07.2024 - 08.07.2024)

  - PR - #4035 (Status: Split into 2 different tutorials for conversion and featurization)
    - Raised a PR on an exploratory understanding of  weighted directed graph featurization for polymers

## Week - 6 (08.07.2024 - 15.07.2024)
  - PR - #4035 got reviews

## Week - 7 (15.07.2024 - 22.07.2024)
  - PR - #4035 is split into two separate PRs

## Week - 8 (22.07.2024 - 29.07.2024)
  - PR - #4035 Real-world implications and Research Papers were referred

## Week - 9 (29.07.2024 - 05.08.2024)
  - PR - [#4070](https://github.com/deepchem/deepchem/pull/4070) (Status :Merged on July 31st)✅
    - The tutorial focuses on the implementation of deepchem models to predict crystallization tendency of polymers.

- PR - [#4073](https://github.com/deepchem/deepchem/pull/4073) (Status: Deleted later for some merge conflicts)
    - This PR is split from PR #4035 for weighted directed graph explanation.
   
## Week - 10 (05.08.2024 - 12.08.2024)
  - PR - [#4088](https://github.com/deepchem/deepchem/pull/4088) (Status: Merged on Aug 7th)✅
    - The rebased tutorial on Weighted-Directed Graph implementation for polymers.

  - PR - [#4097](https://github.com/deepchem/deepchem/pull/4097) (Status: Merged on Aug 12th)✅
    - The tutorial on PSMILES, their formation, and tokenization.

## Week - 11 (12.08.2024 - 19.08.2024)
  - PR - [#4093](https://github.com/deepchem/deepchem/pull/4093) (Status: Merged on Aug 19th) ✅
    - Fixed image rendering issue in polymer tutorials using github image paths

## Week - 12 (19.08.2024 - 26.08.2024)
  - PR - [#4105](https://github.com/deepchem/deepchem/pull/4015) (Status: Merged on Aug 24th) ✅
    - Tutorial on utilization of PolyBERT for similarity prediction of polymer molecules

  
" and below is the extension work. "


- After setup for integration of polymers with the deepchem tooling, we developed a set of generators that can align with existing deepchem discriminators to generate valid candidates with required properties. The following repo showcases the rough pipeline implemented.

    - Repo - [https://github.com/TRY-ER/polymer_pipelines.git]

- With this pipeline we submitted a research paper for AI2ASE workshop for 39th AAAI Annual conference and got selected for presentation.

- The paper is accesible through ArXiv on this [link](https://arxiv.org/html/2412.08658v1)

- The following PRs are responsible for integration of the pipeline into the DeepChem codebase

    -  PR [#4246](https://github.com/deepchem/deepchem/pull/4246)
        - Integration of LSTM Generator for training and inference of SMILES, PSMILES and weighted directed graph generation purposes.
    
    - PR [#4252](https://github.com/deepchem/deepchem/pull/4252)

        - Integration of BRICS sampler for reaction based generation with SMILES and PSMILES

    - PR [#4267](https://github.com/deepchem/deepchem/pull/4267)
        
        - Integration of conversion mechanism between PSMILES and weighted directed graph string representation implemented as utility.

    - PR [#4276](https://github.com/deepchem/deepchem/pull/4276)
        
        - The tutorial for adoption of deepchem generators for candidates generation. The tutorial is developed to showcase the reproducability of our research paper code.

    - PR [#4289](https://github.com/deepchem/deepchem/pull/4289)

        - The tutorial explaining the conversion mechanism between PSMILES and weighted directed graphs. The process is specifically utilized for implementation in our research paper.
