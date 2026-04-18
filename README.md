# Echo: A Multi-Agent AI System for Patient-Centered Pharmacovigilance

**Blog Post**: https://meghabyte.github.io/blog/research/aiscience-claude-25.html 

This repository contains source code for the implementation of **Echo**, a multi-agent AI system that transforms patient narratives from Reddit into structured drug safety intelligence. Echo leverages four specialized language model agents to discover, validate, and contextualize novel drug-symptom associations from online health communities. Echo was accepted at the Agents4Science 2025 conference (https://openreview.net/pdf?id=4nrWtE6oZ9), which studies the impact of significant language model usage during the research process. Please email megha at cs.stanford.edu with any questions!  

### 📋 System Overview

Echo operates through four specialized agents:
- **Explorer**: Extracts drug-symptom mentions from cancer subreddit discussions
- **Analyzer**: Quantifies associations through temporal, confidence, and community metrics
- **Verifier**: Cross-references against FDA databases to identify novel signals
- **Proposer**: Generates mechanistic hypotheses from biomedical literature

### 📁 Repository Structure

#### Core Implementation
```
src/
├── explorer_agent.py          # Reddit data extraction and drug-symptom identification
├── analyzer_agent.py          # Association scoring (temporal, confidence, community)
├── verifier_agent.py          # FAERS database cross-referencing
├── proposer_agent.py          # Hypothesis generation from biomedical literature
├── echo.py           # Echo interface
```


### Future Directions
- **Multi-language Support**: Expansion to global patient communities
- **Therapeutic Area Extension**: Beyond oncology to cardiovascular, neurological conditions
- **Real-time Deployment**: Continuous monitoring and alert systems
- **AI-Human Collaboration**: Augmented clinical decision-making platforms

## 🔧 System Requirements

- **Python 3.8+** with scientific computing stack
- **PRAW Library** for Reddit API integration
- **FDA API Access** for regulatory database queries
- **Modern Web Browser** for interactive visualization interface

## 📋 Ethics & Data Governance

**Responsible Data Sharing**: All patient-derived datasets will be released contingent upon approval from Reddit and adherence to platform terms of service, ensuring full compliance with user privacy expectations and community guidelines.
