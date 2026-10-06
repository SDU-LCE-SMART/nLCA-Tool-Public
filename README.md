# nLCA Tool

**Research software for Nutritional Life Cycle Assessment**

**Version 1.1**

Developed by the **SMART Research Team, Center for Life Cycle Engineering, University of Southern Denmark (SDU)**.

---

## Overview

**nLCA Tool** is research software developed to support methodological implementation, comparison, and sensitivity analysis in **nutritional Life Cycle Assessment (nLCA)**.

Nutritional Life Cycle Assessment extends conventional environmental Life Cycle Assessment by incorporating nutritional characteristics into the assessment of foods and food-related systems. nLCA Tool provides a structured computational environment for investigating how alternative approaches to nutritional characterization affect nutritional indices and nutrition-adjusted environmental results.

Version 1.1 focuses particularly on methodological choices related to:

- nutrient-density assessment;
- protein quantity and protein-quality characterization;
- amino acid composition and digestibility;
- DIAAS-related protein-quality assessment;
- nutrient bioavailability;
- nutrient capping;
- alternative nutrient aggregation approaches;
- methodological sensitivity analysis; and
- integration of nutritional indices with environmental Life Cycle Assessment results.

The software is intended primarily for **research and methodological development** in nutritional Life Cycle Assessment, sustainable food-system assessment, and related fields.

---

## Conceptual framework

The overall structure of nLCA Tool Version 1.1 is illustrated below.

![Conceptual overview of nLCA Tool Version 1.1](figures/nlca_tool_v1.1_overview.png)

**Figure 1. Conceptual workflow of nLCA Tool Version 1.1.**  
The software links nutritional and environmental input data with alternative nutritional characterization approaches. Methodological assumptions concerning protein quality, nutrient bioavailability, capping, aggregation, and related calculation choices can be evaluated systematically before nutritional results are integrated with environmental indicators.

---

## Scientific workflow

The general workflow implemented in Version 1.1 can be represented as:

**Input data -> Nutritional characterization -> Protein-quality characterization -> Bioavailability adjustment -> Capping and aggregation -> Nutritional index -> Environmental integration -> Sensitivity analysis and reporting**

This modular structure is intended to make methodological assumptions explicit and allow researchers to investigate their influence on nLCA results.

---

## Nutritional characterization

The tool supports nutrient-density based nutritional characterization in which selected qualifying and limiting nutrients can be evaluated relative to appropriate reference values.

Researchers can investigate alternative methodological assumptions rather than relying on a single fixed nutritional scoring approach.

Methodological dimensions that can be evaluated include:

- nutrient selection;
- nutrient reference values;
- treatment of qualifying and limiting nutrients;
- nutrient capping;
- sum and mean aggregation;
- weighted aggregation;
- nutrient bioavailability adjustment; and
- protein-quality characterization.

---

## Protein-quality characterization

Version 1.1 implements a **six-level protein-quality framework, Levels 0 to 5**.

Depending on the selected level and the available data, protein assessment can incorporate information related to:

- protein quantity;
- amino acid composition;
- amino acid reference patterns;
- limiting indispensable amino acids;
- protein or amino acid digestibility;
- amino acid scores; and
- DIAAS-related protein-quality characterization.

The multi-level structure allows researchers to investigate how increasing levels of protein-quality characterization influence nutritional and nutrition-adjusted environmental results.

### Example: comparison across protein-quality levels

![Cross-level comparison](figures/cross_level_comparison.png)

**Figure 2. Cross-level comparison of nutritional indices across protein-quality Levels 0 to 5.**  
The figure compares unadjusted and bioavailability-adjusted nutritional indices across the six protein-quality characterization levels for a selected calculation method. This output allows the effect of increasing protein-quality characterization detail to be evaluated while retaining the same assessment object and calculation context.

---

## Nutrient bioavailability

Version 1.1 allows nutrient bioavailability to be incorporated into nutritional characterization when appropriate data or researcher-defined assumptions are available.

Results can therefore be compared between:

- **unadjusted nutritional characterization**; and
- **bioavailability-adjusted nutritional characterization**.

This enables researchers to quantify how assumptions concerning nutrient availability influence the resulting nutritional index.

### Example: bioavailability across calculation variants

![Nutritional index across calculation variants](figures/nutritional_index_variants.png)

**Figure 3. Nutritional index across four calculation variants, comparing unadjusted and bioavailability-adjusted results.**  
The figure compares Cap + Sum, No cap + Sum, Cap + Mean, and No cap + Mean. For each calculation variant, unadjusted and bioavailability-adjusted nutritional indices are presented. The output demonstrates how bioavailability assumptions interact with capping and aggregation choices.

---

## Capping, aggregation, and weighting

A central methodological question in nutrient-density assessment concerns how individual nutrient contributions are treated and subsequently combined.

Version 1.1 supports methodological variants involving:

- capping versus no capping;
- sum versus mean aggregation; and
- weighted aggregation approaches.

These variants can be evaluated using the same assessment object and input dataset.

### Example: calculation-method sensitivity at Level 5

![Calculation method comparison](figures/calculation_method_comparison.png)

**Figure 4. Nutritional index across calculation methods at protein-quality Level 5 using bioavailability-adjusted values.**  
The figure compares eight methodological variants combining capping or no capping with sum, mean, and weighted aggregation approaches. Protein-quality level and bioavailability treatment are held constant. The dashed line at 100% provides a reference point for interpretation. The output therefore isolates the sensitivity of the nutritional index to the selected calculation method.

---

## Methodological sensitivity analysis

A central purpose of nLCA Tool is to facilitate transparent investigation of **methodological sensitivity**.

Comparisons can be conducted across dimensions such as:

- protein-quality level;
- nutrient capping;
- aggregation method;
- weighting approach;
- nutrient bioavailability; and
- combinations of methodological assumptions.

Version 1.1 therefore supports comparison of alternative methodological treatments for the **same defined assessment object**.

---

## Integration with environmental Life Cycle Assessment

Environmental Life Cycle Assessment results can be integrated with the nutritional index calculated by the tool.

This enables environmental impacts to be expressed relative to nutritional performance and allows researchers to investigate how nutritional characterization affects interpretation of environmental performance.

The tool preserves both the underlying environmental result and the nutritional characterization so that the effect of nutritional adjustment remains transparent.

### Example: nutrition-adjusted climate-change result

![Climate change across calculation methods](figures/climate_change_methods.png)

**Figure 5. Climate-change impact per nutritional-index point across alternative nutritional calculation methods.**  
The figure demonstrates how alternative nutritional calculation methods propagate into nutrition-adjusted environmental results. Because the underlying environmental impact for the assessment object is held constant, differences among the bars arise from differences in the calculated nutritional index.

---

## Comparison and visualization

Version 1.1 provides graphical outputs to support interpretation of methodological sensitivity.

Implemented comparisons include:

- nutritional indices across calculation variants;
- unadjusted versus bioavailability-adjusted results;
- comparison across protein-quality Levels 0 to 5;
- comparison of capping, aggregation, and weighting approaches; and
- environmental impacts expressed relative to alternative nutritional-index calculations.

These outputs are designed to make the consequences of methodological choices visible and support transparent reporting of nLCA studies.

---

## Current scope of Version 1.1

Version 1.1 performs methodological assessment for an **individual assessment object at a time**.

The current release is primarily intended for detailed nutritional characterization and methodological sensitivity analysis of a defined assessment object rather than simultaneous comparative assessment of multiple independent ingredients, foods, dishes, meals, or diets.

The tool can compare alternative **protein-quality levels, bioavailability assumptions, capping approaches, aggregation approaches, weighting approaches, and resulting nutrition-adjusted environmental indicators** for the same assessment object.

---

## Planned development

Future development is intended to extend the software toward a structured classification and comparison framework across multiple food-system assessment levels.

The planned framework includes:

1. **Ingredients**
2. **Foods and food products**
3. **Dishes and recipes**
4. **Meals**
5. **Diets and dietary scenarios**

A hierarchical classification framework for these assessment levels is planned for Version 2 and is **not part of the implemented functionality of Version 1.1**.

---

## Research applications

Potential applications of nLCA Tool include:

- methodological research in nutritional Life Cycle Assessment;
- investigation of protein-quality treatment in nLCA;
- evaluation of nutrient bioavailability assumptions;
- sensitivity analysis of nutrient-density models;
- investigation of capping, aggregation, and weighting approaches;
- assessment of nutrition-adjusted environmental indicators;
- sustainable food and alternative-protein research; and
- transparent comparison of alternative nLCA methodological choices.

The software is designed as a research environment rather than as a nutritional recommendation, dietary guidance, or consumer health assessment tool.

---

## Software access

The detailed source code of nLCA Tool Version 1.1 is maintained in a **controlled-access private repository** and is not currently distributed publicly.

This public repository provides scientific documentation, citation information, selected software-generated figures, version information, and information about the research software.

Access to the research software or source code may be considered for research collaboration subject to the conditions established by the developers and affiliated institution.

---

## Citation

If you use nLCA Tool in research, please cite the archived software record:

> **Khoshnevisan, B. (2026). nLCA Tool (Version 1.1). Center for Life Cycle Engineering, University of Southern Denmark. Zenodo.**

The DOI will be added following publication of the Version 1.1 Zenodo record.

Citation metadata are also provided in [`CITATION.cff`](CITATION.cff).

---

## Development

**SMART Research Team**  
**Center for Life Cycle Engineering**  
**University of Southern Denmark (SDU)**  
Denmark

Research team website: https://sdu-lce-smart.github.io/

---

## Contact

**Benyamin Khoshnevisan**  
Associate Professor  
Center for Life Cycle Engineering  
University of Southern Denmark  
Email: bekh@igt.sdu.dk

ORCID: https://orcid.org/0000-0003-0236-5970

---

## Version

Current documented research release:

**nLCA Tool Version 1.1**

Future versions may extend the scientific framework, calculation options, classification system, comparative capabilities, and user interface.

---

## Copyright and reuse

The nLCA Tool source code is not currently released under an open-source software license.

The existence of this public documentation repository does not imply public release of the source code and does not grant permission to copy, modify, redistribute, sublicense, or commercially exploit source code that has not been publicly released.

Copyright ownership and software reuse remain subject to applicable institutional intellectual-property policies of the University of Southern Denmark.

---

## Disclaimer

nLCA Tool is research software.

The developers and affiliated institutions make no warranty regarding the completeness, accuracy, or suitability of results for a particular purpose. Users are responsible for evaluating the appropriateness of input data, reference values, methodological choices, assumptions, and resulting interpretations.

Results generated using nLCA Tool should be interpreted in the context of the methodological assumptions and data used in each individual study.

The software is intended for research purposes and does not provide medical, clinical, dietary, or nutritional advice.

