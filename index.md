# Amazon DynamoDB Developer Guide

-----
*****Copyright &copy; 2019 Amazon Web Services, Inc. and/or its affiliates. All rights reserved.*****

-----
Amazon's trademarks and trade dress may not be used in 
     connection with any product or service that is not Amazon's, 
     in any manner that is likely to cause confusion among customers, 
     or in any manner that disparages or discredits Amazon. All other 
     trademarks not owned by Amazon are the property of their respective
     owners, who may or may not be affiliated with, connected to, or 
     sponsored by Amazon.

-----
## Contents
+ [What Is Amazon DynamoDB?](Introduction.md)
   + [Amazon DynamoDB: How It Works](HowItWorks.md)
      + [DynamoDB Core Components](HowItWorks.CoreComponents.md)
      + [The DynamoDB API](HowItWorks.API.md)
      + [Naming Rules and Data Types](HowItWorks.NamingRulesDataTypes.md)
      + [Read Consistency](HowItWorks.ReadConsistency.md)
      + [Read/Write Capacity Mode](HowItWorks.ReadWriteCapacityMode.md)
      + [Partitions and Data Distribution](HowItWorks.Partitions.md)
   + [From SQL to NoSQL](SQLtoNoSQL.md)
      + [Accessing the Database](SQLtoNoSQL.Accessing.md)
      + [Creating a Table](SQLtoNoSQL.CreateTable.md)
      + [Getting Information About a Table](SQLtoNoSQL.GetTableInfo.md)
      + [Writing Data to a Table](SQLtoNoSQL.WriteData.md)
      + [Reading Data from a Table](SQLtoNoSQL.ReadData.md)
         + [Reading an Item Using Its Primary Key](SQLtoNoSQL.ReadData.SingleItem.md)
         + [Querying a Table](SQLtoNoSQL.ReadData.Query.md)
         + [Scanning a Table](SQLtoNoSQL.ReadData.Scan.md)
      + [Managing Indexes](SQLtoNoSQL.Indexes.md)
         + [Querying and Scanning an Index](SQLtoNoSQL.Indexes.QueryAndScan.md)
      + [Modifying Data in a Table](SQLtoNoSQL.UpdateData.md)
      + [Deleting Data from a Table](SQLtoNoSQL.DeleteData.md)
      + [Removing a Table](SQLtoNoSQL.RemoveTable.md)
+ [Setting Up DynamoDB](SettingUp.md)
   + [Setting Up DynamoDB Local (Downloadable Version)](DynamoDBLocal.md)
      + [DynamoDB (Downloadable Version) on Your Computer](DynamoDBLocal.DownloadingAndRunning.md)
      + [DynamoDB (Downloadable Version) and Apache Maven](DynamoDBLocal.Maven.md)
      + [DynamoDB (Downloadable Version) and Docker](DynamoDBLocal.Docker.md)
      + [DynamoDB Usage Notes](DynamoDBLocal.UsageNotes.md)
   + [Setting Up DynamoDB (Web Service)](SettingUp.DynamoWebService.md)
+ [Accessing DynamoDB](AccessingDynamoDB.md)
   + [Using the Console](ConsoleDynamoDB.md)
      + [Working with User Preferences](user-preferences.md)
   + [Using the CLI](Tools.CLI.md)
   + [Using the API](Using.API.md)
   + [IP Address Ranges](Using.IPRanges.md)
+ [Getting Started with DynamoDB](GettingStartedDynamoDB.md)
   + [Basic Concepts in DynamoDB](GettingStarted.CoreComponents.md)
   + [Prerequisites](GettingStarted.SettingUp.DynamoWebService.md)
   + [Step 1: Create a Table](getting-started-step-1.md)
   + [Step 2: Write Data to a Table](getting-started-step-2.md)
   + [Step 3: Read Data from a Table](getting-started-step-3.md)
   + [Step 4: Update Data in a Table](getting-started-step-4.md)
   + [Step 5: Query Data in a Table](getting-started-step-5.md)
   + [Step 6: Create a Global Secondary Index](getting-started-step-6.md)
   + [Step 7: Query the Global Secondary Index](getting-started-step-7.md)
   + [Step 8: (Optional) Clean Up Resources](getting-started-step-8.md)
   + [Getting Started with DynamoDB: Next Steps](getting-started-NextSteps.md)
+ [Getting Started with DynamoDB SDK](GettingStarted.md)
   + [Java and DynamoDB](GettingStarted.Java.md)
      + [Step 1: Create a Table](GettingStarted.Java.01.md)
      + [Step 2: Load Sample Data](GettingStarted.Java.02.md)
      + [Step 3: Create, Read, Update, and Delete an Item](GettingStarted.Java.03.md)
      + [Step 4: Query and Scan the Data](GettingStarted.Java.04.md)
      + [Step 5: (Optional) Delete the Table](GettingStarted.Java.05.md)
      + [Summary](GettingStarted.Java.Summary.md)
   + [JavaScript and DynamoDB](GettingStarted.JavaScript.md)
      + [Step 1: Create a Table](GettingStarted.Js.01.md)
      + [Step 2: Load Sample Data](GettingStarted.Js.02.md)
      + [Step 3: Create, Read, Update, and Delete an Item](GettingStarted.Js.03.md)
      + [Step 4: Query and Scan the Data](GettingStarted.Js.04.md)
      + [Step 5: (Optional): Delete the Table](GettingStarted.Js.05.md)
      + [Summary](GettingStarted.Js.Summary.md)
   + [Node.js and DynamoDB](GettingStarted.NodeJs.md)
      + [Step 1: Create a Table](GettingStarted.NodeJs.01.md)
      + [Step 2: Load Sample Data](GettingStarted.NodeJs.02.md)
      + [Step 3: Create, Read, Update, and Delete an Item](GettingStarted.NodeJs.03.md)
      + [Step 4: Query and Scan the Data](GettingStarted.NodeJs.04.md)
      + [Step 5: (Optional): Delete the Table](GettingStarted.NodeJs.05.md)
      + [Summary](GettingStarted.NodeJs.Summary.md)
   + [Tutorial: Microsoft .NET and DynamoDB](GettingStarted.NET.md)
      + [.NET and DynamoDB Tutorial Prerequisites](GettingStarted.NET.Prereqs.md)
      + [Step 1: Create a DynamoDB Client](GettingStarted.NET.01.md)
      + [Step 2: Create a Table Using the Low-Level API](GettingStarted.NET.02.md)
      + [Step 3: Load Sample Data into the Movies Table](GettingStarted.NET.03.md)
      + [Step 4: Add a New Movie to the Movies Table](GettingStarted.NET.04.md)
      + [Step 5: Read and Display a Record from the Movies Table](GettingStarted.NET.05.md)
      + [Step 6: Update the New Movie Record](GettingStarted.NET.06.md)
      + [Step 7: Try to Conditionally Delete the Movie](GettingStarted.NET.07.md)
      + [Step 8: Query the Movies Table](GettingStarted.NET.08.md)
      + [Step 9: Scan the Movies Table](GettingStarted.NET.09.md)
      + [Step 10: Delete the Movies Table](GettingStarted.NET.10.md)
   + [PHP and DynamoDB](GettingStarted.PHP.md)
      + [Step 1: Create a Table](GettingStarted.PHP.01.md)
      + [Step 2: Load Sample Data](GettingStarted.PHP.02.md)
      + [Step 3: Create, Read, Update, and Delete an Item](GettingStarted.PHP.03.md)
      + [Step 4: Query and Scan the Data](GettingStarted.PHP.04.md)
      + [Step 5: (Optional) Delete the Table](GettingStarted.PHP.05.md)
      + [Summary](GettingStarted.PHP.Summary.md)
   + [Python and DynamoDB](GettingStarted.Python.md)
      + [Step 1: Create a Table](GettingStarted.Python.01.md)
      + [Step 2: Load Sample Data](GettingStarted.Python.02.md)
      + [Step 3: Create, Read, Update, and Delete an Item](GettingStarted.Python.03.md)
      + [Step 4: Query and Scan the Data](GettingStarted.Python.04.md)
      + [Step 5: (Optional) Delete the Table](GettingStarted.Python.05.md)
      + [Summary](GettingStarted.Python.Summary.md)
   + [Ruby and DynamoDB](GettingStarted.Ruby.md)
      + [Step 1: Create a Table](GettingStarted.Ruby.01.md)
      + [Step 2: Load Sample Data](GettingStarted.Ruby.02.md)
      + [Step 3: Create, Read, Update, and Delete an Item](GettingStarted.Ruby.03.md)
      + [Step 4: Query and Scan the Data](GettingStarted.Ruby.04.md)
      + [Step 5: (Optional) Delete the Table](GettingStarted.Ruby.05.md)
      + [Summary](GettingStarted.Ruby.Summary.md)
+ [Programming with DynamoDB and the AWS SDKs](Programming.md)
   + [Overview of AWS SDK Support for DynamoDB](Programming.SDKOverview.md)
   + [Programmatic Interfaces](Programming.SDKs.Interfaces.md)
      + [Low-Level Interfaces](Programming.SDKs.Interfaces.LowLevel.md)
      + [Document Interfaces](Programming.SDKs.Interfaces.Document.md)
      + [Object Persistence Interface](Programming.SDKs.Interfaces.Mapper.md)
   + [DynamoDB Low-Level API](Programming.LowLevelAPI.md)
   + [Error Handling](Programming.Errors.md)
   + [Higher-Level Programming Interfaces for DynamoDB](HigherLevelInterfaces.md)
      + [Java: DynamoDBMapper](DynamoDBMapper.md)
         + [Supported Data Types](DynamoDBMapper.DataTypes.md)
         + [Java Annotations for DynamoDB](DynamoDBMapper.Annotations.md)
         + [DynamoDBMapper Class](DynamoDBMapper.Methods.md)
         + [Optional Configuration Settings for DynamoDBMapper](DynamoDBMapper.OptionalConfig.md)
         + [Example: CRUD Operations](DynamoDBMapper.CRUDExample1.md)
         + [Example: Batch Write Operations](DynamoDBMapper.BatchWriteExample.md)
         + [Example: Query and Scan](DynamoDBMapper.QueryScanExample.md)
         + [Example: Transaction Operations](DynamoDBMapper.Transactions.md)
         + [Optimistic Locking with Version Number](DynamoDBMapper.OptimisticLocking.md)
         + [Mapping Arbitrary Data](DynamoDBMapper.ArbitraryDataMapping.md)
      + [.NET: Document Model](DotNetSDKMidLevel.md)
         + [Working with Items in DynamoDB Using the AWS SDK for .NET Document Model](WorkingWithItemsDocumentClasses.md)
         + [Example: CRUD Operations Using the AWS SDK for .NET Document Model](ItemCRUDDotNetDocumentAPI.md)
         + [Example: Batch Operations Using the AWS SDK for .NET Document Model API](example-batch-operations-net-doc-model.md)
         + [Querying Tables in DynamoDB Using the AWS SDK for .NET Document Model](QueryAndScanMidLevelDotNet.md)
            + [Table.Query Method in the AWS SDK for .NET](QueryMidLevelDotNet.md)
            + [Table.Scan Method in the AWS SDK for .NET](ScanMidLevelDotNet.md)
      + [.NET: Object Persistence Model](DotNetSDKHighLevel.md)
         + [DynamoDB Attributes](DeclarativeTagsList.md)
         + [DynamoDBContext Class](DotNetDynamoDBContext.md)
         + [Optimistic Locking Using a Version Number with DynamoDB Using the AWS SDK for .NET Object Persistence Model](DynamoDBContext.VersionSupport.md)
         + [Mapping Arbitrary Data with DynamoDB Using the AWS SDK for .NET Object Persistence Model](DynamoDBContext.ArbitraryDataMapping.md)
         + [Batch Operations Using the AWS SDK for .NET Object Persistence Model](DotNetDynamoDBContext.BatchOperations.md)
         + [Example: CRUD Operations Using the AWS SDK for .NET Object Persistence Model](CRUDHighLevelExample1.md)
         + [Example: Batch Write Operation Using the AWS SDK for .NET Object Persistence Model](orm-dotnet-batchoperations-example.md)
         + [Example: Query and Scan in DynamoDB Using the AWS SDK for .NET Object Persistence Model](DynamoDBContext.QueryScan.md)
   + [Running the Code Examples in This Developer Guide](CodeSamples.md)
      + [Creating Tables and Loading Sample Data](SampleData.md)
         + [Step 1: Create Example Tables](SampleData.CreateTables.md)
         + [Step 2: Load Data into Tables](SampleData.LoadData.md)
         + [Step 3: Query the Data](SampleData.Query.md)
         + [Step 4: (Optional) Clean Up](SampleData.DeleteTables.md)
         + [Summary](Summary.md)
      + [Java Code Examples](CodeSamples.Java.md)
      + [.NET Code Examples](CodeSamples.DotNet.md)
+ [Working with DynamoDB](WorkingWithDynamo.md)
   + [Working with Tables in DynamoDB](WorkingWithTables.md)
      + [Basic Operations for Tables](WorkingWithTables.Basics.md)
      + [Considerations When Changing Read/Write Capacity Mode](switching.capacitymode.md)
      + [Managing Throughput Settings on Provisioned Tables](ProvisionedThroughput.md)
      + [DynamoDB Item Sizes](CapacityUnitCalculations.md)
      + [Managing Throughput Capacity Automatically with DynamoDB Auto Scaling](AutoScaling.md)
         + [Using the AWS Management Console with DynamoDB Auto Scaling](AutoScaling.Console.md)
         + [Using the AWS CLI to Manage DynamoDB Auto Scaling](AutoScaling.CLI.md)
         + [Application Programming With DynamoDB Auto Scaling](AutoScaling.HowTo.SDK.md)
      + [Tagging for DynamoDB](Tagging.md)
         + [Tagging Restrictions](TaggingRestrictions.md)
         + [Tagging Operations](Tagging.Operations.md)
         + [Cost Allocation Reports](CostAllocationReports.md)
      + [Working with Tables: Java](JavaDocumentAPIWorkingWithTables.md)
         + [Example: Create, Update, Delete, and List Tables Using the AWS SDK for Java Document API](JavaDocumentAPITablesExample.md)
      + [Working with Tables: .NET](LowLevelDotNetWorkingWithTables.md)
         + [Example: Create, Update, Delete, and List Tables Using the AWS SDK for .NET Low-Level API](LowLevelDotNetTableOperationsExample.md)
   + [Working with Items in DynamoDB](WorkingWithItems.md)
      + [Using Expressions in DynamoDB](Expressions.md)
         + [Specifying Item Attributes](Expressions.Attributes.md)
         + [Projection Expressions](Expressions.ProjectionExpressions.md)
         + [Expression Attribute Names](Expressions.ExpressionAttributeNames.md)
         + [Expression Attribute Values](Expressions.ExpressionAttributeValues.md)
         + [Condition Expressions](Expressions.ConditionExpressions.md)
            + [Comparison Operator and Function Reference](Expressions.OperatorsAndFunctions.md)
         + [Update Expressions](Expressions.UpdateExpressions.md)
      + [Time To Live](TTL.md)
         + [Time To Live: How It Works](howitworks-ttl.md)
         + [Before You Begin Using Time To Live](time-to-live-ttl-before-you-start.md)
         + [Enabling Time To Live](time-to-live-ttl-how-to.md)
      + [Working with Items: Java](JavaDocumentAPIItemCRUD.md)
         + [Example: CRUD Operations Using the AWS SDK for Java Document API](JavaDocumentAPICRUDExample.md)
         + [Example: Batch Operations Using AWS SDK for Java Document API](batch-operation-document-api-java.md)
         + [Example: Handling Binary Type Attributes Using the AWS SDK for Java Document API](JavaDocumentAPIBinaryTypeExample.md)
      + [Working with Items: .NET](LowLevelDotNetItemCRUD.md)
         + [Example: CRUD Operations Using the AWS SDK for .NET Low-Level API](LowLevelDotNetItemsExample.md)
         + [Example: Batch Operations Using AWS SDK for .NET Low-Level API](batch-operation-lowlevel-dotnet.md)
         + [Example: Handling Binary Type Attributes Using the AWS SDK for .NET Low-Level API](LowLevelDotNetBinaryTypeExample.md)
   + [Working with Queries](Query.md)
      + [Querying Tables and Indexes: Java](QueryingJavaDocumentAPI.md)
      + [Querying Tables and Indexes: .NET](LowLevelDotNetQuerying.md)
   + [Working with Scans](Scan.md)
      + [Scanning Tables and Indexes: Java](ScanJavaDocumentAPI.md)
      + [Scanning Tables and Indexes: .NET](LowLevelDotNetScanning.md)
   + [Improving Data Access with Secondary Indexes](SecondaryIndexes.md)
      + [Global Secondary Indexes](GSI.md)
         + [Managing Global Secondary Indexes](GSI.OnlineOps.md)
            + [Detecting and Correcting Index Key Violations](GSI.OnlineOps.ViolationDetection.md)
         + [Working with Global Secondary Indexes: Java](GSIJavaDocumentAPI.md)
            + [Example: Global Secondary Indexes Using the AWS SDK for Java Document API](GSIJavaDocumentAPI.Example.md)
         + [Working with Global Secondary Indexes: .NET](GSILowLevelDotNet.md)
            + [Example: Global Secondary Indexes Using the AWS SDK for .NET Low-Level API](GSILowLevelDotNet.Example.md)
      + [Local Secondary Indexes](LSI.md)
         + [Working with Local Secondary Indexes: Java](LSIJavaDocumentAPI.md)
            + [Example: Local Secondary Indexes Using the Java Document API](LSIJavaDocumentAPI.Example.md)
         + [Working with Local Secondary Indexes: .NET](LSILowLevelDotNet.md)
            + [Example: Local Secondary Indexes Using the AWS SDK for .NET Low-Level API](LSILowLevelDotNet.Example.md)
   + [Capturing Table Activity with DynamoDB Streams](Streams.md)
      + [DynamoDB Streams and Time To Live](time-to-live-ttl-streams.md)
      + [Using the DynamoDB Streams Kinesis Adapter to Process Stream Records](Streams.KCLAdapter.md)
         + [Walkthrough: DynamoDB Streams Kinesis Adapter](Streams.KCLAdapter.Walkthrough.md)
            + [Complete Program: DynamoDB Streams Kinesis Adapter](Streams.KCLAdapter.Walkthrough.CompleteProgram.md)
      + [DynamoDB Streams Low-Level API: Java Example](Streams.LowLevel.Walkthrough.md)
      + [Cross-Region Replication](Streams.CrossRegionRepl.md)
      + [DynamoDB Streams and AWS Lambda Triggers](Streams.Lambda.md)
         + [Tutorial: Processing New Items in a DynamoDB Table](Streams.Lambda.Tutorial.md)
         + [Best Practices](Streams.Lambda.BestPracticesWithDynamoDB.md)
+ [On-Demand Backup and Restore for DynamoDB](BackupRestore.md)
   + [Backup and Restore: How It Works](backuprestore_HowItWorks.md)
   + [Backing Up a DynamoDB Table](Backup.Tutorial.md)
   + [Restoring a DynamoDB Table from a Backup](Restore.Tutorial.md)
   + [Deleting a DynamoDB Table Backup](Delete.Tutorial.md)
   + [Using IAM with DynamoDB Backup and Restore](backuprestore_IAM.md)
+ [Point-in-Time Recovery for DynamoDB](PointInTimeRecovery.md)
   + [Point-in-Time Recovery: How It Works](PointInTimeRecovery_Howitworks.md)
   + [Before You Begin Using Point In Time Recovery](pointintimerecovery_beforeyoubegin.md)
   + [Restoring a DynamoDB Table to a Point in Time](PointInTimeRecovery.Tutorial.md)
+ [Global Tables](GlobalTables.md)
   + [Global Tables: How It Works](globaltables_HowItWorks.md)
   + [Requirements and Best Practices](globaltables_reqs_bestpractices.md)
   + [Creating a Global Table](globaltables.tutorial.md)
   + [Monitoring Global Tables](globaltables_monitoring.md)
   + [Using IAM with Global Tables](gt_IAM.md)
+ [Amazon DynamoDB Transactions](transactions.md)
   + [Amazon DynamoDB Transactions: How It Works](transaction-apis.md)
   + [Using IAM with DynamoDB Transactions](transaction-apis-iam.md)
   + [DynamoDB Transactions Example](transaction-example.md)
+ [In-Memory Acceleration with DAX](DAX.md)
   + [Concepts](DAX.concepts.md)
   + [DAX Cluster Components](DAX.concepts.cluster.md)
   + [Creating a DAX Cluster](DAX.create-cluster.md)
      + [AWS CLI](DAX.create-cluster.cli.md)
         + [Step 1: Create an IAM service role for DAX to access DynamoDB](DAX.create-cluster.cli.create-service-role.md)
         + [Step 2: Create a Subnet Group](DAX.create-cluster.cli.create-subnet-group.md)
         + [Step 3: Create a DAX Cluster](DAX.create-cluster.cli.create-cluster.md)
         + [Step 4: Configure Security Group Inbound Rules](DAX.create-cluster.cli.configure-inbound-rules.md)
      + [AWS Management Console](DAX.create-cluster.console.md)
         + [Step 1: Create a Subnet Group](DAX.create-cluster.console.create-subnet-group.md)
         + [Step 2: Create a DAX Cluster](DAX.create-cluster.console.create-cluster.md)
         + [Step 3: Configure Security Group Inbound Rules](DAX.create-cluster.console.configure-inbound-rules.md)
   + [DAX and DynamoDB Consistency Models](DAX.consistency.md)
   + [Using the DAX Client in an Application](DAX.client.md)
      + [Tutorial: Running a Sample Application Using DAX](DAX.client.sample-app.md)
         + [Step 1: Launch an Amazon EC2 Instance](DAX.client.launch-ec2-instance.md)
         + [Step 2: Create an IAM User and Policy](DAX.client.create-user-policy.md)
         + [Step 3: Configure Your Amazon EC2 Instance](DAX.client.configure-ec2-instance.md)
         + [Step 4: Run a Sample Application](DAX.client.run-application.md)
            + [DAX SDK for Go](DAX.client.run-application-go.md)
            + [Java and DAX](DAX.client.run-application-java.md)
               + [TryDax.java](DAX.client.run-application-java.TryDax.md)
               + [TryDaxHelper.java](DAX.client.run-application-java.TryDaxHelper.md)
               + [TryDaxTests.java](DAX.client.run-application-java.TryDaxTests.md)
            + [.NET and DAX](DAX.client.run-application-dotnet.md)
               + [01-CreateTable.cs](DAX.client.run-application-dotnet.01-CreateTable.md)
               + [02-Write-Data.cs](DAX.client.run-application-dotnet.02-Write-Data.md)
               + [03-GetItem-Test.cs](DAX.client.run-application-dotnet.03-GetItem-Test.md)
               + [04-Query-Test.cs](DAX.client.run-application-dotnet.04-Query-Test.md)
               + [05-Scan-Test.cs](DAX.client.run-application-dotnet.05-Scan-Test.md)
               + [06-DeleteTable.cs](DAX.client.run-application-dotnet.06-DeleteTable.md)
            + [Node.js and DAX](DAX.client.run-application-nodejs.md)
               + [01-create-table.js](DAX.client.run-application-nodejs.01-create-table.md)
               + [02-write-data.js](DAX.client.run-application-nodejs.02-write-data.md)
               + [03-getitem-test.js](DAX.client.run-application-nodejs.03-getitem-test.md)
               + [04-query-test.js](DAX.client.run-application-nodejs.04-query-test.md)
               + [05-scan-test.js](DAX.client.run-application-nodejs.05-scan-test.md)
               + [06-delete-table.js](DAX.client.run-application-nodejs.06-delete-table.md)
            + [Python and DAX](DAX.client.run-application-python.md)
               + [01-create-table.py](DAX.client.run-application-python.01-create-table.md)
               + [02-write-data.py](DAX.client.run-application-python.02-write-data.md)
               + [03-getitem-test.py](DAX.client.run-application-python.03-getitem-test.md)
               + [04-query-test.py](DAX.client.run-application-python.04-query-test.md)
               + [05-scan-test.py](DAX.client.run-application-python.05-scan-test.md)
               + [06-delete-table.py](DAX.client.run-application-python.06-delete-table.md)
      + [Modifying an Existing Application to Use DAX](DAX.client.modify-your-app.md)
   + [Managing DAX Clusters](DAX.cluster-management.md)
   + [Using Service-Linked Roles for DAX](using-service-linked-roles.md)
   + [DAX API Reference](DAX.api.md)
+ [Security in Amazon DynamoDB](security.md)
   + [Data Protection in DynamoDB](data-protection.md)
      + [DynamoDB Encryption at Rest](EncryptionAtRest.md)
         + [Encryption at Rest: How It Works](encryption.howitworks.md)
         + [Encryption at Rest Usage Notes](encryption.usagenotes.md)
         + [Managing Encrypted Tables](encryption.tutorial.md)
      + [DAX Encryption at Rest](DAXEncryptionAtRest.md)
      + [Internetwork Traffic Privacy](inter-network-traffic-privacy.md)
   + [Identity and Access Management](identity-and-access-mgmt.md)
      + [Identity and Access Management in Amazon DynamoDB](authentication-and-access-control.md)
         + [Overview of Managing Access Permissions to Your Amazon DynamoDB Resources](access-control-overview.md)
         + [Using Identity-Based Policies (IAM Policies) for Amazon DynamoDB](using-identity-based-policies.md)
         + [DynamoDB API Permissions: Actions, Resources, and Conditions Reference](api-permissions-reference.md)
         + [Using IAM Policy Conditions for Fine-Grained Access Control](specifying-conditions.md)
         + [Using Web Identity Federation](WIF.md)
            + [Preparing to Use Web Identity Federation](WIF.PreparingForUse.md)
            + [Writing Your App to Use Web Identity Federation](WIF.RunningYourApp.md)
      + [Identity and Access Management in DAX](DAX.access-control.md)
   + [Logging and Monitoring](monitoring-security.md)
      + [Logging and Monitoring in DynamoDB](MonitoringDynamoDB.md)
         + [Monitoring Tools](monitoring-automated-manual.md)
         + [Monitoring with Amazon CloudWatch](monitoring-cloudwatch.md)
            + [DynamoDB Metrics and Dimensions](metrics-dimensions.md)
            + [Creating CloudWatch Alarms to Monitor DynamoDB](creating-alarms.md)
         + [Logging DynamoDB Operations by Using AWS CloudTrail](logging-using-cloudtrail.md)
      + [Logging and Monitoring in DAX](DAX.Monitoring.md)
         + [Monitoring Tools](dax-monitoring-automated-manual.md)
         + [Monitoring with Amazon CloudWatch](dax-monitoring-cloudwatch.md)
            + [Viewing DAX Metrics and Dimensions](dax-metrics-dimensions-dax.md)
            + [Creating CloudWatch Alarms to Monitor DAX](dax-creating-alarms.md)
         + [Logging DAX Operations Using AWS CloudTrail](dax-logging-using-cloudtrail.md)
   + [Compliance Validation for DynamoDB](Compliance.md)
   + [Resilience and Disaster Recovery in Amazon DynamoDB](disaster-recovery-resiliency.md)
   + [Infrastructure Security in Amazon DynamoDB](network-isolation.md)
      + [Using Amazon VPC Endpoints to Access DynamoDB](vpc-endpoints-dynamodb.md)
         + [Tutorial: Using a VPC Endpoint for DynamoDB](vpc-endpoints-dynamodb-tutorial.md)
   + [Configuration and Vulnerability Analysis in Amazon DynamoDB](configuration-vulnerability.md)
   + [Security Best Practices for Amazon DynamoDB](best-practices-security.md)
      + [DynamoDB Preventative Security Best Practices](best-practices-security-preventative.md)
      + [DynamoDB Detective Security Best Practices](best-practices-security-detective.md)
+ [Best Practices for DynamoDB](best-practices.md)
   + [NoSQL Design for DynamoDB](bp-general-nosql-design.md)
   + [Best Practices for Designing and Using Partition Keys Effectively](bp-partition-key-design.md)
      + [Designing Partition Keys to Distribute Your Workload Evenly](bp-partition-key-uniform-load.md)
      + [Using Write Sharding to Distribute Workloads Evenly](bp-partition-key-sharding.md)
      + [Distributing Write Activity Efficiently During Data Upload](bp-partition-key-data-upload.md)
   + [Best Practices for Using Sort Keys to Organize Data](bp-sort-keys.md)
   + [Best Practices for Using Secondary Indexes in DynamoDB](bp-indexes.md)
      + [General Guidelines for Secondary Indexes in DynamoDB](bp-indexes-general.md)
      + [Take Advantage of Sparse Indexes](bp-indexes-general-sparse-indexes.md)
      + [Using Global Secondary Indexes for Materialized Aggregation Queries](bp-gsi-aggregation.md)
      + [Overloading Global Secondary Indexes](bp-gsi-overloading.md)
      + [Using Global Secondary Index Write Sharding for Selective Table Queries](bp-indexes-gsi-sharding.md)
      + [Using Global Secondary Indexes to Create an Eventually Consistent Replica](bp-indexes-gsi-replica.md)
   + [Best Practices for Storing Large Items and Attributes](bp-use-s3-too.md)
   + [Best Practices for Handling Time-Series Data in DynamoDB](bp-time-series.md)
   + [Best Practices for Managing Many-to-Many Relationships](bp-adjacency-graphs.md)
   + [Best Practices for Implementing a Hybrid Database System](bp-hybrid.md)
   + [Best Practices for Modeling Relational Data in DynamoDB](bp-relational-modeling.md)
      + [First Steps for Modeling Relational Data in DynamoDB](bp-modeling-nosql.md)
      + [Example of Modeling Relational Data in DynamoDB](bp-modeling-nosql-B.md)
   + [Best Practices for Querying and Scanning Data](bp-query-scan.md)
   + [Best Practices for Using Global Tables](bp-global-tables.md)
+ [DynamoDB Integration with Other AWS Services](OtherServices.md)
   + [Configure AWS Credentials in Your Files Using Amazon Cognito](Cognito.Credentials.md)
   + [Loading Data From DynamoDB Into Amazon Redshift](RedshiftforDynamoDB.md)
   + [Processing DynamoDB Data With Apache Hive on Amazon EMR](EMRforDynamoDB.md)
      + [Tutorial: Working with Amazon DynamoDB and Apache Hive](EMRforDynamoDB.Tutorial.md)
         + [Step 1: Create an Amazon EC2 Key Pair](EMRforDynamoDB.Tutorial.EC2KeyPair.md)
         + [Step 2: Launch an Amazon EMR Cluster](EMRforDynamoDB.Tutorial.LaunchEMRCluster.md)
         + [Step 3: Connect to the Master Node](EMRforDynamoDB.Tutorial.ConnectToMasterNode.md)
         + [Step 4: Load Data into HDFS](EMRforDynamoDB.Tutorial.LoadDataIntoHDFS.md)
         + [Step 5: Copy Data to DynamoDB](EMRforDynamoDB.Tutorial.CopyDataToDDB.md)
         + [Step 6: Query the Data in the DynamoDB Table](EMRforDynamoDB.Tutorial.QueryDataInDynamoDB.md)
         + [Step 7: (Optional) Clean Up](EMRforDynamoDB.Tutorial.CleanUp.md)
      + [Creating an External Table in Hive](EMRforDynamoDB.ExternalTableForDDB.md)
      + [Processing HiveQL Statements](EMRforDynamoDB.ProcessingHiveQL.md)
      + [Querying Data in DynamoDB](EMRforDynamoDB.Querying.md)
      + [Copying Data to and from Amazon DynamoDB](EMRforDynamoDB.CopyingData.md)
         + [Copying Data Between DynamoDB and a Native Hive Table](EMRforDynamoDB.CopyingData.NativeHive.md)
         + [Copying Data Between DynamoDB and Amazon S3](EMRforDynamoDB.CopyingData.S3.md)
         + [Copying Data Between DynamoDB and HDFS](EMRforDynamoDB.CopyingData.HDFS.md)
         + [Using Data Compression](EMRforDynamoDB.CopyingData.Compression.md)
         + [Reading Non-Printable UTF-8 Character Data](EMRforDynamoDB.CopyingData.NonPrintableData.md)
      + [Performance Tuning](EMRforDynamoDB.PerformanceTuning.md)
         + [DynamoDB Provisioned Throughput](EMRforDynamoDB.PerformanceTuning.Throughput.md)
         + [Adjusting the Mappers](EMRforDynamoDB.PerformanceTuning.Mappers.md)
         + [Additional Topics](EMRforDynamoDB.PerformanceTuning.Misc.md)
+ [Limits in DynamoDB](Limits.md)
+ [API Reference](CurrentAPI.md)
+ [DynamoDB Appendix](Appendix.md)
   + [Troubleshooting SSL/TLS connection establishment issues](ats-certs.md)
   + [Example Tables and Data](AppendixSampleTables.md)
   + [Creating Example Tables and Uploading Data](AppendixSampleDataCode.md)
      + [Creating Example Tables and Uploading Data Using the AWS SDK for Java](AppendixSampleDataCodeJava.md)
      + [Creating Example Tables and Uploading Data Using the AWS SDK for .NET](AppendixSampleDataCodeDotNET.md)
   + [DynamoDB Example Application Using AWS SDK for Python (Boto): Tic-Tac-Toe](TicTacToe.md)
      + [Step 1: Deploy and Test Locally](TicTacToe.Phase1.md)
      + [Step 2: Examine the Data Model and Implementation Details](TicTacToe.Phase2.md)
      + [Step 3: Deploy in Production Using the DynamoDB Service](TicTacToe.Phase3.md)
      + [Step 4: Clean Up Resources](TicTacToe.AppClosure.md)
   + [Exporting and Importing DynamoDB Data Using AWS Data Pipeline](DynamoDBPipeline.md)
   + [Amazon DynamoDB Storage Backend for Titan](Tools.TitanDB.md)
   + [Reserved Words in DynamoDB](ReservedWords.md)
   + [Legacy Conditional Parameters](LegacyConditionalParameters.md)
      + [AttributesToGet](LegacyConditionalParameters.AttributesToGet.md)
      + [AttributeUpdates](LegacyConditionalParameters.AttributeUpdates.md)
      + [ConditionalOperator](LegacyConditionalParameters.ConditionalOperator.md)
      + [Expected](LegacyConditionalParameters.Expected.md)
      + [KeyConditions](LegacyConditionalParameters.KeyConditions.md)
      + [QueryFilter](LegacyConditionalParameters.QueryFilter.md)
      + [ScanFilter](LegacyConditionalParameters.ScanFilter.md)
      + [Writing Conditions With Legacy Parameters](LegacyConditionalParameters.Conditions.md)
   + [Previous Low-Level API Version (2011-12-05)](Appendix.APIv20111205.md)
      + [BatchGetItem](API_BatchGetItem_v20111205.md)
      + [BatchWriteItem](API_BatchWriteItem_v20111205.md)
      + [CreateTable](API_CreateTable_v20111205.md)
      + [DeleteItem](API_DeleteItem_v20111205.md)
      + [DeleteTable](API_DeleteTable_v20111205.md)
      + [DescribeTables](API_DescribeTables_v20111205.md)
      + [GetItem](API_GetItem_v20111205.md)
      + [ListTables](API_ListTables_v20111205.md)
      + [PutItem](API_PutItem_v20111205.md)
      + [Query](API_Query_v20111205.md)
      + [Scan](API_Scan_v20111205.md)
      + [UpdateItem](API_UpdateItem_v20111205.md)
      + [UpdateTable](API_UpdateTable_v20111205.md)
+ [Document History for DynamoDB](DocumentHistory.md)