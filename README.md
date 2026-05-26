# Market Stack API Data Transfer

A comprehensive data pipeline solution built with Azure Data Factory to transfer and process market data from the Market Stack API.

## Project Overview

This project automates the extraction, transformation, and loading (ETL) of market data from the Market Stack API into a data warehouse or analytics platform using Azure Data Factory (ADF).

## Project Structure

```
Market-Stack-API-Data-Transfer/
├── dataset/              # Dataset definitions
├── factory/              # Factory configurations
├── linkedService/        # Linked service connections
├── pipeline/             # Pipeline definitions and workflows
├── trigger/              # Trigger configurations
├── publish_config.json   # Publishing configuration
└── README.md             # Project documentation
```

### Directory Details

- **dataset/** - Contains dataset definitions that describe the structure of data being processed
- **factory/** - Core Azure Data Factory configurations and settings
- **linkedService/** - Linked service definitions for connecting to data sources and destinations (Market Stack API, storage, etc.)
- **pipeline/** - Data pipeline definitions that orchestrate the ETL workflows
- **trigger/** - Trigger configurations for scheduling and executing pipelines

## Features

- Automated data extraction from Market Stack API
- Data transformation and processing workflows
- Scheduled pipeline execution
- Data transfer to target destinations
- Configuration-driven approach for flexibility

## Prerequisites

- Azure subscription with Data Factory enabled
- Access to Market Stack API credentials
- Appropriate permissions in Azure Data Factory
- Configured linked services for data destinations

## Getting Started

1. **Clone the repository**
   ```bash
   git clone https://github.com/BharatDhiman4378/Market-Stack-API-Data-Transfer.git
   cd Market-Stack-API-Data-Transfer
   ```

2. **Configure Linked Services**
   - Update linked service configurations in the `linkedService/` directory
   - Provide your Market Stack API credentials
   - Configure destination storage or database connections

3. **Deploy Pipelines**
   - Use the `publish_config.json` to publish configurations to Azure Data Factory
   - Deploy pipeline definitions from the `pipeline/` directory

4. **Set Up Triggers**
   - Configure triggers in the `trigger/` directory
   - Schedule pipeline runs based on your requirements

## Configuration

All configurations are managed through JSON files in their respective directories. Update these files to match your environment and data requirements.

## Usage

Pipelines can be triggered:
- On a schedule (configured in trigger settings)
- Manually through Azure Data Factory UI
- Programmatically via Azure API

## Data Flow

1. **Extract** - Fetch market data from Market Stack API
2. **Transform** - Process and structure the data
3. **Load** - Transfer processed data to destination

## Troubleshooting

- Check linked service connections are properly configured
- Verify Market Stack API credentials and authentication
- Review Azure Data Factory pipeline run history for errors
- Ensure destination storage/database has appropriate permissions

## Contributing

Contributions are welcome! Please feel free to submit pull requests or open issues for bugs and feature requests.

## License

This project is provided as-is. Please refer to your organization's policies for usage and distribution.

## Support

For issues, questions, or suggestions, please create an issue in the repository.

---

**Last Updated:** May 2026
**Created by:** BharatDhiman4378
