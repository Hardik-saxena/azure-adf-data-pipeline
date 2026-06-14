# Azure Data Factory Data Pipeline
# Objective
End-to-end Azure Data Factory pipeline using Blob Storage, Get Metadata, Copy Data Activity, IAM roles, and pipeline monitoring.

# Azure Services Used:- 
1) Azure Resource Group
2) Azure Storage Account
3) Azure Blob Storage
4) Azure Data Factory
5) Azure IAM (Reader & Contributor Roles)

# Architecture
Blob Storage (Source) → Azure Data Factory → Blob Storage (Destination)

# Implementation Steps
## step1: Building a Resource Group
Designing leads to the creation of a resource group through the azure portal.

## step2: Blob Container and Storage Account
Create a storage account and blob containers in such a way as to upload the Superstore dataset to the source container.

## step3: Azure Data Factory Instance
Through your Azure Data Factory instance, you will be able to perform three functions, which include:
- Authoring
- Monitoring
- Managing

## Step 4: Services and Datasets Linked
Linked Service was configured for Azure Blob Storage.
Source and Destination datasets were created.

## Step 5: Get Metadata Activity
Configured Get Metadata activity to pull the following:
Determine file size
When the file was last modified
If the file exists

## Step 6: Copy Data Activity
Configured the Copy Data activity to copy data from the source container to the destination container.

## Step7: Identity and Access Management (IAM) Configuration
The next step was assigning the reader and contributor role to both Azure Data Factory and the Azure Storage Account. By having the proper permissions assigned, it allows secure access between Azure Data Factory and Azure Storage Account.

## Step8: Pipeline Execution
The step was to execute the pipeline. The pipeline was executed using both debug and trigger. The execution can be monitored from the monitor page of the pipeline.

## Results:
The results of this step are the pipeline executed successfully, the metadata was validated successfully, the dataset was copied from the source container to the destination container, and the access permissions were configured using the Azure IAM.

## Conclusion:
The project demonstrates the core fundamentals and the implementation of an end-to-end data pipeline in Microsoft Azure using an Azure Storage Account and Azure Data Factory.
