# Extraction Plan for Level Generation Classes

## Overview
This document outlines the plan for extracting the level generation classes from the `shattered-pixel-dungeon` repository to be integrated into the `spd-level-previsualisation` repository. The extraction will focus on modularization for improved maintainability and clarity.

## Objectives
- Identify and isolate the relevant level generation classes from the `shattered-pixel-dungeon` repository.
- Ensure compatibility with the current architecture in `spd-level-previsualisation`.
- Document dependencies and interfaces.

## Steps for Extraction

### 1. Identify Relevant Classes
- Examine the `shattered-pixel-dungeon` codebase to identify level generation classes, such as:
  - `LevelGenerator`
  - `Room`
  - `Corridor`

### 2. Dependency Analysis
- List all external dependencies used by the identified classes.
- Assess if these dependencies are already included in `spd-level-previsualisation`.

### 3. Modularity Refactoring
- Modify the identified classes for modularity if necessary. This includes:
  - Removing hard dependencies.
  - Creating interfaces if multiple implementations are needed.

### 4. Transfer Code
- Move the refined class definitions into `spd-level-previsualisation` directory structure, under `level_generation/`.

### 5. Integrate and Test
- Integrate the classes into the main functionality of `spd-level-previsualisation`.
- Create unit tests to ensure the integrity of the extracted classes.

### 6. Documentation
- Update the documentation of `spd-level-previsualisation` to include details about the new level generation classes, their usage, and integration points.

## Timeline
- **Week 1**: Code extraction and initial modularization.
- **Week 2**: Testing and documentation update.
- **Week 3**: Review and finalize the integration.

## Expected Outcomes
- Cleanly extracted and functional level generation classes ready for usage in `spd-level-previsualisation`.
- Comprehensive documentation for future reference and onboarding.

## Conclusion
This extraction plan serves as a guideline to ensure a systematic approach to integrating level generation classes from `shattered-pixel-dungeon` into `spd-level-previsualisation`. Proper execution will enhance the functionality and maintainability of the project.