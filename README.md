# Obsidian PKM
# Active Matter Physics Vault Structure

## Research Core Structure

### 1. Active Matter MOC
```markdown
# Active Matter Physics MOC

## Theoretical Frameworks
- [[Langevin Equation]]
- [[Stokes Equation]]
- [[Active Brownian Motion]]
- [[Run and Tumble Dynamics]]

## Bacterial Suspensions
- [[Bacterial Swimming Mechanisms]]
- [[Collective Behavior]]
- [[Confinement Effects]]
- [[Activity Parameters]]

## Passive Particles
- [[Brownian Motion]]
- [[Passive Tracer Dynamics]]
- [[Mean Square Displacement Analysis]]
- [[Diffusion in Active Baths]]

## Experimental Methods
- [[Microscopy Techniques]]
- [[Particle Tracking]]
- [[Image Analysis Protocols]]
- [[Data Processing Workflows]]

## Mathematical Tools
- [[Statistical Analysis]]
- [[Correlation Functions]]
- [[Numerical Methods]]
- [[MATLAB Analysis Scripts]]
```

### 2. Thesis Framework
```markdown
thesis/
├── chapters/
│   ├── ch1-introduction/
│   │   ├── active_matter_overview.md
│   │   ├── bacterial_suspensions.md
│   │   └── research_objectives.md
│   ├── ch2-theoretical_framework/
│   │   ├── langevin_dynamics.md
│   │   ├── active_brownian_motion.md
│   │   └── confinement_effects.md
│   ├── ch3-experimental_methods/
│   │   ├── setup.md
│   │   ├── protocols.md
│   │   └── data_collection.md
│   └── ch4-results/
│       ├── msd_analysis.md
│       ├── activity_parameters.md
│       └── discussion.md
├── experiments/
│   ├── raw_data/
│   ├── processed_data/
│   └── analysis_scripts/
└── presentations/
    ├── group_meetings/
    ├── conferences/
    └── defense/
```

## Templates

### 1. Experiment Log Template
```markdown
# Experiment: {{title}}
Date: {{date}}

## Setup Parameters
- Bacterial strain: 
- Concentration:
- Confinement geometry:
- Temperature:
- Medium composition:

## Measurements
- [ ] Microscopy settings
- [ ] Frame rate
- [ ] Duration
- [ ] Number of particles tracked

## Data Collection
- Raw data location: 
- Backup status:
- Initial observations:

## Analysis Tasks
- [ ] Particle tracking
- [ ] MSD calculation
- [ ] Activity parameter extraction
- [ ] Statistical analysis

## Results
### Raw Measurements
- Particle trajectories:
- Bacterial density:
- Flow characteristics:

### Processed Data
- MSD curves:
- Diffusion coefficients:
- Activity parameters:

## Notes
- Observations:
- Challenges:
- Follow-up questions:

## Next Steps
- [ ] Additional measurements needed
- [ ] Analysis refinements
- [ ] Theory connections
```

### 2. Analysis Protocol Template
```markdown
# Analysis Protocol: {{title}}

## Data Prerequisites
- [ ] Raw trajectory data
- [ ] Calibration files
- [ ] Control measurements

## MATLAB Analysis Steps
```matlab
% Key code snippets and parameters
```

## Quality Checks
- [ ] Trajectory validation
- [ ] Statistical significance
- [ ] Error analysis

## Expected Outputs
- [ ] MSD curves
- [ ] Diffusion coefficients
- [ ] Activity parameters

## Visualization
- [ ] Required plots
- [ ] Key figures
- [ ] Error bars
```

## Daily Note Integration

### Daily Research Log Template
```markdown
# {{date}} Research Log

## Progress
### Experiments
- [ ] Running experiments
- [ ] Data collection
- [ ] Analysis progress

### Theory
- [ ] Model development
- [ ] Calculations
- [ ] Literature review

### Writing
- [ ] Thesis sections
- [ ] Paper drafts
- [ ] Presentation prep

## Insights
- New ideas:
- Connections found:
- Questions raised:

## Tasks
- [ ] Priority tasks
- [ ] Follow-ups
- [ ] Collaborations

## References
- Papers read:
- Relevant notes:
- Resources needed:
```

## Dataview Queries

### Experiment Tracking
```dataview
TABLE 
    date as "Date",
    bacterial_strain as "Strain",
    concentration as "Concentration",
    status as "Status"
FROM "experiments"
SORT date DESC
```

### Analysis Progress
```dataview
TABLE
    file.ctime as "Created",
    analysis_type as "Analysis",
    status as "Status",
    results as "Key Findings"
FROM "thesis/experiments"
WHERE contains(tags, "#analysis")
SORT file.ctime DESC
```

## Enhanced Git Integration

### .gitignore Additions
```gitignore
# Large experimental data
*.tif
*.avi
*.mat

# MATLAB temporary files
*.asv
*.m~

# Analysis outputs
/thesis/experiments/raw_data/
/thesis/experiments/processed_data/
```

## Knowledge Graph Structure

### Tag System
- #experiment/bacterial
- #analysis/msd
- #theory/langevin
- #method/tracking
- #result/significant
- #status/active
- #status/analysis
- #status/writing

### Priority Links
1. Experimental results ↔ Theoretical predictions
2. Analysis methods ↔ Data interpretation
3. Literature findings ↔ Your results
4. Methods ↔ Protocols

## Maintenance Workflow

### Daily
- Process experimental data
- Update analysis logs
- Link new insights to existing notes

### Weekly
- Review experiment progress
- Update thesis sections
- Backup data and analysis
- Git commits

### Monthly
- Comprehensive results review
- Update theoretical models
- Refine analysis methods
- Knowledge graph cleanup
---
# Complete Guide to Using Obsidian for Academic Research

## Part 1: Getting Started

### Setting Up Your First Note
1. **Creating Notes**
   - Press `Ctrl/Cmd + N` for a new note
   - Use meaningful titles
   - Start with a header (`# Title`)
   - Add metadata at the top if needed:
     ```markdown
     ---
     tags: physics, active-matter
     date: 2024-11-15
     status: in-progress
     ---
     ```

2. **Basic Markdown Syntax**
   ```markdown
   # Header 1
   ## Header 2
   
   *italic* or _italic_
   **bold** or __bold__
   
   - Bullet point
   - Another point
     - Sub-point
   
   1. Numbered list
   2. Second item
   
   > Quote or important note
   
   `inline code`
   
   ```python
   # code block
   def function():
       pass
   ```
   ```

3. **Essential Keyboard Shortcuts**
   - `Ctrl/Cmd + P`: Command palette
   - `Ctrl/Cmd + O`: Quick switcher
   - `Ctrl/Cmd + E`: Toggle edit/preview
   - `Ctrl/Cmd + Click`: Open link in new pane

### Creating Links and Connections
1. **Internal Links**
   - Use `[[]]` for internal links
   - Examples:
     - Basic link: `[[Note Title]]`
     - With alias: `[[Note Title|Display Text]]`
     - Header link: `[[Note Title#Section]]`

2. **Backlinks**
   - View in right sidebar
   - Shows all notes linking to current note
   - Great for discovering connections

3. **Tags**
   - Use `#tag-name`
   - Hierarchical tags: `#physics/quantum`
   - View all tags in tag pane

## Part 2: Organization Techniques

### Folder Structure
```markdown
vault/
├── 00-inbox/           # Temporary storage for new notes
├── 01-daily/           # Daily notes
├── 02-literature/      # Paper notes and references
├── 03-projects/        # Active research projects
├── 04-permanent/       # Processed, permanent notes
└── templates/          # Note templates
```

### Using Maps of Content (MOCs)
1. **Create Hub Notes**
   ```markdown
   # Physics Concepts MOC
   
   ## Quantum Mechanics
   - [[QM Fundamentals]]
   - [[Wave Functions]]
   - [[Operators]]
   
   ## Statistical Mechanics
   - [[Entropy]]
   - [[Partition Functions]]
   ```

2. **Link MOCs Together**
   ```markdown
   # Research MOC
   
   ## Theory
   - [[Physics Concepts MOC]]
   - [[Mathematics MOC]]
   
   ## Practice
   - [[Experiments MOC]]
   - [[Analysis Methods MOC]]
   ```

### Daily Notes Workflow
1. **Set Up Daily Notes**
   - Enable Core Plugin
   - Create template:
     ```markdown
     # {{date}}
     
     ## Tasks
     - [ ] 
     
     ## Notes
     
     ## Ideas
     
     ## Links
     ```

2. **Link to Projects**
   - Reference ongoing work
   - Create quick capture notes
   - Link to relevant literature

## Part 3: Advanced Features

### Using Templates
1. **Create Template**
   ```markdown
   # {{title}}
   Created: {{date}}
   
   ## Overview
   
   ## Key Points
   
   ## Questions
   
   ## References
   ```

2. **Template Hotkeys**
   - Set up template hotkeys
   - Use in different contexts

### Essential Plugins
1. **Core Plugins**
   - File explorer
   - Search
   - Quick switcher
   - Graph view
   - Outgoing links
   - Tags pane

2. **Community Plugins**
   - Dataview (for queries)
   - Calendar
   - Citations
   - LaTeX Suite
   - Excalidraw

### Using Dataview
1. **Basic Queries**
   ```dataview
   TABLE file.ctime as Created,
         status as Status
   FROM "projects"
   WHERE status = "active"
   ```

2. **Task Tracking**
   ```dataview
   TASK
   FROM "daily"
   WHERE !completed
   GROUP BY file.link
   ```

## Part 4: Practical Workflows

### Literature Note Workflow
1. **Create Literature Note**
   ```markdown
   # {{paper-title}}
   
   ## Citation
   - Authors:
   - Year:
   - Journal:
   - DOI:
   
   ## Summary
   
   ## Key Points
   
   ## Methodology
   
   ## Results
   
   ## Relevance to Research
   
   ## Notes & Questions
   ```

2. **Link to Research**
   - Connect to projects
   - Add to literature MOC
   - Tag appropriately

### Research Project Workflow
1. **Project Setup**
   ```markdown
   # Project: {{title}}
   
   ## Objective
   
   ## Methods
   
   ## Progress
   - [ ] Phase 1
   - [ ] Phase 2
   
   ## Notes
   
   ## Resources
   ```

2. **Regular Updates**
   - Link daily notes
   - Track progress
   - Document decisions

## Part 5: Best Practices

### File Naming
1. **Conventions**
   - Use descriptive names
   - Include dates for temporal notes
   - Use prefixes for categories
     - `lit-` for literature
     - `proj-` for projects
     - `exp-` for experiments

2. **Examples**
   ```
   lit-smith2024-active-matter.md
   proj-bacterial-dynamics.md
   exp-2024-11-particle-tracking.md
   ```

### Linking Strategy
1. **When to Link**
   - Connect related concepts
   - Link evidence to claims
   - Connect methods to results

2. **How to Link**
   - Use descriptive aliases
   - Link specific sections
   - Create bidirectional links

### Maintenance
1. **Daily**
   - Process inbox
   - Update daily note
   - Link new content

2. **Weekly**
   - Review unlinked mentions
   - Update MOCs
   - Check broken links

3. **Monthly**
   - Clean up tags
   - Update templates
   - Archive completed projects

### Backup Strategy
1. **Local Backup**
   - Use Git for version control
   - Regular system backups
   - Export important notes

2. **Cloud Backup**
   - Sync to cloud service
   - Version history
   - Multiple devices

## Part 6: Troubleshooting

### Common Issues
1. **Broken Links**
   - Check unlinked mentions
   - Update renamed files
   - Fix broken references

2. **Performance**
   - Regular vault cleanup
   - Optimize large files
   - Manage plugin load

3. **Search Problems**
   - Update search index
   - Check file locations
   - Verify syntax