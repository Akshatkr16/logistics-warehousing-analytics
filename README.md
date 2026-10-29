# Logistics & Warehousing Performance Analytics

An end-to-end logistics analytics project using **Python, Pandas, and Power BI** to evaluate transportation efficiency, freight costs, delivery performance, warehouse utilization, and inventory availability.

> **Dataset disclaimer:** This project uses a synthetic dataset created for portfolio and educational purposes. The analysis does not represent actual ITC operational data or verified business outcomes.

## Business Objectives

- Analyze freight cost per unit across transporters.
- Evaluate transit delays and delivery performance.
- Compare warehouse storage utilization and stockout rates.
- Monitor truck utilization, shipment damage, and truck turnaround time.
- Build an interactive Power BI dashboard for logistics KPI monitoring.

## Tools & Technologies

- Python
- Pandas and NumPy
- Matplotlib and Seaborn
- Jupyter Notebook
- Microsoft Power BI and DAX

## Dataset Overview

The synthetic dataset contains **900 shipment records and 25 columns**, covering:

- Shipment dates, districts, warehouses, and transporters
- Freight costs, shipment quantities, and transit times
- Truck utilization, shipment damage, and turnaround time
- Warehouse storage utilization and inventory indicators
- Stockout and OTIF flags

## Key Findings

The initial analysis of the synthetic dataset identified the following patterns:

- **Late shipment rate:** 69.00%
- **Recorded OTIF rate:** 80.78%
- **Stockout rate:** 22.78%
- **Warehouse WH-04:** approximately 26.90% stockout rate
- **Transporter D:** approximately 5.41 dataset currency units per shipped unit, the lowest weighted freight cost among the six transporters

Transporter D also recorded a higher average transit delay than Transporter A. This highlights why freight cost should be assessed alongside service performance.

These findings are descriptive results from synthetic data, not actual company performance.

## Power BI Dashboard

The interactive dashboard includes:

- Shipment volume, OTIF, late shipment, and stockout KPI cards
- Transporter freight cost comparison
- Warehouse stockout analysis
- Monthly shipment trend
- District, transporter, and product-category slicers

The Power BI report and dashboard preview will be included in this repository.

## Project Workflow

1. Data loading and inspection
2. Data quality and validation checks
3. Logistics KPI engineering
4. Transporter performance benchmarking
5. Warehouse and inventory analysis
6. Visualization and Power BI dashboard development
7. Business interpretation and recommendations

## Business Recommendations

- Review transporters with high delays even when their freight costs are low.
- Investigate warehouses with elevated stockout rates.
- Assess truck utilization and opportunities for load consolidation.
- Monitor delivery, cost, damage, and inventory KPIs together rather than optimizing a single metric.

These recommendations are hypotheses for further investigation, not proven savings or operational improvements.

## Repository Contents

- `data/` — synthetic shipment dataset
- `notebooks/` — Jupyter Notebook analysis
- `outputs/figures/` — charts and dashboard preview
- `outputs/tables/` — exported KPI and benchmarking tables
- `dashboard/` — Power BI report, if stored separately

## Limitations

The dataset is synthetic. The OTIF and stockout flags are provided practice indicators and have not been independently validated against real delivery or inventory records. Freight currency is unspecified. The results should not be used for real operational decisions.

## Future Improvements

- Validate OTIF using actual delivery dates and ordered-versus-delivered quantities.
- Add more detailed inventory replenishment and safety-stock analysis.
- Introduce automated data validation tests.
- Expand the dashboard with additional service-level and cost indicators.

