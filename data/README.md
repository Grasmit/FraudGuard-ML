# Data Directory

This directory contains the datasets used for training and testing the fraud detection models.

## Dataset Structure

The fraud detection model uses financial transaction data with the following features:

### Features:
- **step**: Transaction timestamp (hour)
- **type**: Transaction type (PAYMENT, TRANSFER, CASH_OUT, DEBIT, CASH_IN)
- **amount**: Transaction amount
- **nameOrig**: Origin account identifier (anonymized)
- **oldbalanceOrg**: Origin account balance before transaction
- **newbalanceOrig**: Origin account balance after transaction
- **nameDest**: Destination account identifier (anonymized)
- **oldbalanceDest**: Destination account balance before transaction
- **newbalanceDest**: Destination account balance after transaction
- **isFraud**: Target variable (1 if fraud, 0 if legitimate)

## Data Privacy

⚠️ **Important**: No actual financial data files are included in this repository for privacy and security reasons.

To use this project:
1. Obtain anonymized transaction data that follows the structure above
2. Place your dataset files in this directory
3. Update the file paths in the notebook accordingly

## Recommended Data Format

- File format: CSV
- Size: 1M+ transactions for robust model training
- Anonymization: All personal identifiers should be anonymized
- Time period: Multiple months of transaction data for temporal patterns

## Data Sources

This project was developed using publicly available synthetic datasets that simulate real-world financial transaction patterns while maintaining privacy.
