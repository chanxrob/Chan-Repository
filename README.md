# IoT Data Integration: Hospital Nursery

## Project Overview

This project integrates three IoT data sources from a hospital nursery into one dataset for security and environmental monitoring. It combines access-control events, room sensor readings, and newborn vital-sign observations.

## Source Files

The `source-data` folder contains three data files:

- `batch101.csv` - Nursery access-control records, including access decisions.
- `stream101.json` - Environmental sensor readings, including room temperature, humidity, and door status.
- `feed101.xml` - Newborn vital-sign observations and medical-condition fields.

## Part 3 Deliverables

- `integrated_nursery.csv` - Integrated dataset combining information from all three sources.
- `data_dictionary.csv` - Data dictionary documenting field names, data types, units, and descriptions.
- `final_report.docx` - Final report explaining integration methods, data cleaning, design decisions, use cases, and limitations.

## Previous Checkpoints

- `Data Pipeline Check #1.docx` - Initial data pipeline analysis and answers.
- Checkpoint 2 updates are preserved in the `source-data` folder.

## Data Integration

The integrated dataset uses CSV because its tabular structure is suitable for dashboards, filtering, and analysis.

The three original sources contain different types of information collected at different times and frequencies. The integrated dataset brings this information together for analysis.

The final report explains the record-matching approach, handling of missing values, and limitations of the integration.

## Potential Use Cases

1. Examine nursery access activity alongside room environmental conditions.
2. Analyze newborn vital signs in relation to nursery temperature and humidity.
3. Investigate whether unusual access events coincide with environmental or vital-sign changes.

## Data Dictionary

The `data_dictionary.csv` file documents the fields in the integrated dataset, including their names, data types, units where applicable, and descriptions.

## Project Limitations

The source files contain records collected at different frequencies. Some measurements may not have exact matching timestamps.

Missing values and differences in collection times can affect interpretation. The integrated dataset is intended for educational analysis rather than clinical decision-making.

## Conclusion

This project demonstrates how CSV, JSON, and XML data sources can be integrated into a unified dataset for IoT security and environmental monitoring.
The resulting dataset supports analysis across multiple sources while maintaining documentation of the integration process.

