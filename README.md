# Prefect Article Series: Retail Analytics Pipeline

A comprehensive 8-article series that takes you from Prefect beginner to advanced practitioner through a progressive retail analytics project.

## 📚 Article Series Overview

### Foundation Level (Article 0)
0. **Prefect Introduction & Comparison** - Tool comparison and setup

### Beginner Level (Articles 1-4)
1. **Prefect Fundamentals** - Your first data pipeline
2. **Building Robust Pipelines** - Error handling & scheduling
3. **ETL Patterns with Prefect** - Multi-source data processing
4. **Advanced Flow Patterns** - Dynamic & modular workflows

### Intermediate Level (Articles 5-6)
5. **External Data Integration** - Building connected pipelines
6. **Monitoring and Observability** - Production-ready pipelines

### Advanced Level (Articles 7-8)
7. **Production Deployment** - Containerization & infrastructure
8. **Cloud & Enterprise Features** - Scaling to production

### Business & Economics (Article 9)
9. **Cost Analysis & Real-World Economics** - TCO and ROI analysis

## 🚀 Quick Start

### Prerequisites
- Python 3.8+
- Git
- Basic understanding of Python and data processing

### Installation
```bash
# Clone the repository
git clone git@github.com:spky-io/prefect-tutorials.git
cd prefect-tutorials

# Set up virtual environment and install dependencies
./setup_environment.sh

# Activate virtual environment (if not already activated)
source venv/bin/activate  # On Windows: venv\Scripts\activate
```

### Project Structure
```
retail-analytics-pipeline/
├── src/
│   ├── flows/
│   │   ├── beginner/          # Articles 1-4
│   │   ├── intermediate/      # Articles 5-6
│   │   └── advanced/          # Articles 7-8
│   ├── tasks/
│   │   ├── data_ingestion/
│   │   ├── data_validation/
│   │   ├── data_transformation/
│   │   └── data_storage/
│   ├── utils/
│   │   ├── config.py
│   │   ├── logging.py
│   │   └── helpers.py
│   └── models/
│       └── data_models.py
├── data/
│   ├── raw/                   # Raw datasets
│   ├── processed/             # Processed data
│   └── outputs/               # Analysis outputs
├── tests/                     # Test files
├── docker/                    # Docker configurations
├── deployments/               # Deployment configurations
└── docs/                      # Documentation
```

## 📁 Dataset Information

### Article 0: Foundation Concepts
- **Purpose**: Understand workflow orchestration landscape
- **Focus**: Tool comparisons and setup guidance

### Article 1-2: Titanic Dataset
- **Purpose**: Learn basic Prefect concepts
- **Source**: Local CSV files
- **Focus**: Passenger demographics and survival analysis

### Article 3-4: Online Retail Dataset
- **Purpose**: Real-world ETL patterns
- **Source**: Kaggle/UCI Machine Learning Repository
- **Focus**: Sales transactions and customer behavior

### Article 5-8: Multi-source Data
- **Purpose**: Advanced integrations and production deployment
- **Sources**: APIs, web scraping, databases, cloud storage
- **Focus**: Enterprise-grade data pipeline

### Article 9: Economic Analysis
- **Purpose**: Cost optimization and business justification
- **Focus**: TCO, ROI, and real-world economics

## 🛠️ Development Setup

### Local Development
```bash
# Start Prefect UI locally
prefect server start

# Run a flow
python -m src.flows.beginner.article1_titanic_analysis
```

### Testing
```bash
# Run tests
pytest tests/

# Run with coverage
pytest --cov=src tests/
```

### Code Quality
```bash
# Format code
black src/ tests/

# Lint code
flake8 src/ tests/

# Type checking
mypy src/
```

## 📊 Learning Path

### Beginner Skills (After Article 4)
- ✅ Understand Prefect core concepts (Flows, Tasks, Parameters)
- ✅ Build basic data pipelines with error handling
- ✅ Implement ETL patterns and parallel execution
- ✅ Create dynamic and modular workflows

### Intermediate Skills (After Article 6)  
- ✅ Integrate with external APIs and databases
- ✅ Implement comprehensive monitoring and alerting
- ✅ Optimize pipeline performance
- ✅ Handle real-world data integration challenges

### Advanced Skills (After Article 8)
- ✅ Deploy production-ready containerized pipelines
- ✅ Manage infrastructure with Prefect Server/Cloud
- ✅ Implement CI/CD for data workflows
- ✅ Scale pipelines for enterprise workloads

## 🔧 Configuration

### Environment Variables
Create a `.env` file for local development:
```bash
# Prefect Configuration
PREFECT_API_URL=http://localhost:4200/api
PREFECT_UI_URL=http://localhost:4200

# Database Configuration
DATABASE_URL=sqlite:///data/retail_analytics.db

# API Keys (for Articles 5-8)
MARKET_DATA_API_KEY=your_api_key_here
```

### Prefect Configuration
The project uses Prefect 2.x with modern configuration patterns. Key configuration files:
- `src/utils/config.py` - Application configuration
- `deployments/` - Flow deployment configurations
- `docker/` - Containerization configurations

## 🤝 Contributing

This project follows the article series structure. Each article builds upon the previous one, so contributions should maintain the progressive learning approach.

### Contribution Guidelines
1. Follow the existing code structure and naming conventions
2. Ensure each article's code is self-contained and runnable
3. Include comprehensive tests for new functionality
4. Update documentation when adding new features

## 📝 License

This project is designed for educational purposes as part of a technical article series.

## 📞 Support

For questions about the article series or code examples:
- Check the detailed article content
- Review the code comments and docstrings
- Refer to the Prefect documentation: https://docs.prefect.io/

## 🎯 Next Steps

1. **Start with Article 1** in the `src/flows/beginner/` directory
2. Follow the progressive learning path through each article
3. Experiment with the code examples and exercises
4. Apply the concepts to your own data pipeline projects

---

*This series is designed to take you from zero to production-ready with Prefect, building real-world data engineering skills along the way.*