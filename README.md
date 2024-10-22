# Geoecology Research Group - Repository Guide

## Repository Structure

```
geoecology-halle/
├── research-projects/               # Active research projects
│   ├── environmental-monitoring/    # Environmental data collection and analysis
│   │   ├── field-protocols/        # Standard operating procedures for field work
│   │   ├── data-collection/        # Raw data and collection scripts
│   │   └── analysis/              # Analysis scripts and results
│   │
│   ├── biogeochemical-cycling/     # Biogeochemical research
│   │   ├── soil-analysis/         # Soil sampling and analysis protocols
│   │   ├── lab-protocols/         # Laboratory procedures
│   │   └── data/                  # Datasets and analysis
│   │
│   └── land-use-change/           # Land use impact studies
│       ├── satellite-data/        # Remote sensing data processing
│       ├── ground-truth/          # Field validation data
│       └── models/                # Predictive models and analysis
│
├── teaching-materials/             # Educational resources
│   ├── courses/                   # Course-specific materials
│   │   ├── intro-geoecology/     # Introduction to Geoecology
│   │   ├── field-methods/        # Field Methods in Geoecology
│   │   └── data-analysis/        # Environmental Data Analysis
│   │
│   └── workshops/                 # Workshop materials
│       ├── r-tutorials/          # R programming tutorials
│       └── qgis-basics/         # QGIS training materials
│
├── data-tools/                    # Analysis and visualization tools
│   ├── data-processors/          # Data processing scripts
│   ├── visualization-tools/      # Plotting and visualization
│   └── field-apps/              # Mobile data collection apps
│
├── publications/                  # Publication-related materials
│   ├── manuscripts/              # Paper drafts and submissions
│   ├── data-availability/        # Published dataset archives
│   └── code-supplements/        # Analysis code for publications
│
└── resources/                    # Shared resources
    ├── templates/               # Document and code templates
    ├── guides/                 # How-to guides and documentation
    └── policies/              # Organization policies
```

## How to Use This Repository

### For New Members

1. **Getting Started**
   ```bash
   # Clone the resources repository first
   git clone https://github.com/geoecology-halle/resources.git
   
   # Review the guides directory
   cd resources/guides
   ```

2. **Access Requirements**
   - Request organization access from your supervisor
   - Set up two-factor authentication
   - Read the CONTRIBUTING.md guide

### For Research Projects

1. **Starting a New Project**
   ```bash
   # Clone the research-projects repository
   git clone https://github.com/geoecology-halle/research-projects.git
   
   # Create a new project from template
   cp -r resources/templates/project-template new-project-name
   ```

2. **Data Management**
   - Store raw data in `/data-collection`
   - Document collection methods in `/field-protocols`
   - Place analysis scripts in `/analysis`
   - Use standard naming conventions (YYYY-MM-DD_descriptor)

### For Teaching Materials

1. **Adding Course Content**
   ```bash
   # Clone teaching-materials
   git clone https://github.com/geoecology-halle/teaching-materials.git
   
   # Create new course directory
   mkdir -p courses/new-course-name/{lectures,exercises,assignments}
   ```

2. **Material Organization**
   - Use markdown for documentation
   - Include R/Python scripts as separate files
   - Add README.md in each subdirectory

### For Data Tools

1. **Tool Development**
   ```bash
   # Clone data-tools repository
   git clone https://github.com/geoecology-halle/data-tools.git
   
   # Create new tool directory
   mkdir -p data-tools/new-tool/{src,tests,docs}
   ```

2. **Documentation Requirements**
   - API documentation in `/docs`
   - Usage examples in README.md
   - Test cases in `/tests`

## Standard Workflows

### Field Data Collection
```bash
research-projects/
└── project-name/
    ├── field-protocols/           # Start here - review protocols
    ├── data-collection/
    │   ├── raw/                  # Store raw data files
    │   └── processed/            # Store processed data
    └── analysis/                 # Add analysis scripts
```

### Data Analysis
```bash
# Standard analysis workflow
1. data-collection/raw/           # Original data
2. data-collection/processed/     # Cleaned data
3. analysis/scripts/              # Analysis code
4. analysis/outputs/              # Results
5. analysis/figures/              # Visualizations
```

## Best Practices

### Version Control
- Commit messages: "type(scope): description"
- Branch naming: `feature/`, `bugfix/`, `docs/`
- Pull request required for main branch

### Data Management
- Raw data is read-only
- Include metadata files
- Use open formats (CSV, GeoTIFF)
- Document processing steps

### Code Style
- Python: Follow PEP 8
- R: Follow tidyverse style
- Document functions and workflows

## Communication

### Issues and Projects
- Use GitHub Issues for tasks
- Tag with appropriate labels
- Link issues to projects
- Use project boards for tracking

### Documentation
- Update README.md files
- Document setup steps
- Include requirements.txt
- Add example usage

## Support

- Technical issues: Open GitHub issue
- Access requests: Contact lab manager
- General questions: Use discussion board

Remember to check the `/resources/guides` directory for detailed documentation on specific workflows and procedures.
