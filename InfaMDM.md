# Informatica MDM

- [How to install Informatica MDM SaaS?](#how-to-install-informatica-mdm-saas)
  - [1. **Provision Informatica MDM SaaS Account**](#1-provision-informatica-mdm-saas-account)
  - [2. **Configure Infrastructure \& Security**](#2-configure-infrastructure--security)
  - [3. **Set Up MDM SaaS Environment**](#3-set-up-mdm-saas-environment)
  - [4. **Data Integration**](#4-data-integration)
  - [5. **Data Quality and Governance Configuration**](#5-data-quality-and-governance-configuration)
  - [6. **Deploy the MDM SaaS Solution**](#6-deploy-the-mdm-saas-solution)
  - [7. **Post Go-Live Maintenance**](#7-post-go-live-maintenance)
  - [Tools You'll Use](#tools-youll-use)
- [How to configure Informatica MDM match/merge rules?](#how-to-configure-informatica-mdm-matchmerge-rules)
  - [1. **Understand the Match/Merge Process**](#1-understand-the-matchmerge-process)
  - [2. **Access the Hub Console for Match/Merge Configuration**](#2-access-the-hub-console-for-matchmerge-configuration)
  - [3. **Define Match Columns**](#3-define-match-columns)
  - [4. **Configure Match Rule Logic**](#4-configure-match-rule-logic)
  - [5. **Set Match Rule Thresholds**](#5-set-match-rule-thresholds)
  - [6. **Configure Merge Rules (Survivorship Rules)**](#6-configure-merge-rules-survivorship-rules)
  - [7. **Test Match/Merge Configuration**](#7-test-matchmerge-configuration)
  - [8. **Deploy and Monitor**](#8-deploy-and-monitor)
  - [Example Scenario](#example-scenario)
- [How to config Informatica MDM SaaS?](#how-to-config-informatica-mdm-saas)
  - [1. **Access the Informatica MDM SaaS Platform**](#1-access-the-informatica-mdm-saas-platform)
  - [2. **Configure the Data Model**](#2-configure-the-data-model)
  - [3. **Define Match/Merge Rules**](#3-define-matchmerge-rules)
  - [4. **Set Up Data Governance and Stewardship**](#4-set-up-data-governance-and-stewardship)
  - [5. **Data Integration Configuration**](#5-data-integration-configuration)
  - [6. **Security and Role-Based Access Control**](#6-security-and-role-based-access-control)
  - [7. **Testing and Validation**](#7-testing-and-validation)
  - [8. **Monitoring and Alerts**](#8-monitoring-and-alerts)
  - [9. **Deployment and Maintenance**](#9-deployment-and-maintenance)
  - [Tools and Consoles Used](#tools-and-consoles-used)
- [How to migrate from informatica MDM Single Tenant to MDM SaaS?](#how-to-migrate-from-informatica-mdm-single-tenant-to-mdm-saas)
  - [1. **Planning and Assessment**](#1-planning-and-assessment)
  - [2. **Prepare the MDM SaaS Environment**](#2-prepare-the-mdm-saas-environment)
  - [3. **Data Migration**](#3-data-migration)
  - [4. **System Integration and API Configuration**](#4-system-integration-and-api-configuration)
  - [5. **Security and Compliance Setup**](#5-security-and-compliance-setup)
  - [6. **Testing and Validation**](#6-testing-and-validation)
  - [7. **Cutover and Go-Live**](#7-cutover-and-go-live)
  - [8. **Post-Migration Optimization and Maintenance**](#8-post-migration-optimization-and-maintenance)
  - [Tools and Services to Use](#tools-and-services-to-use)
- [Manual review](#manual-review)
  - [**Informatica Data Director (IDD) Overview**](#informatica-data-director-idd-overview)
  - [**Key Features of Informatica Data Director (IDD) for Manual Review:**](#key-features-of-informatica-data-director-idd-for-manual-review)
  - [**Why Use IDD Instead of a Custom Web App?**](#why-use-idd-instead-of-a-custom-web-app)
  - [**When to Consider Building a Custom Web App?**](#when-to-consider-building-a-custom-web-app)
  - [**Tools for Building a Custom Web App**](#tools-for-building-a-custom-web-app)
  - [**Recommendation:**](#recommendation)
- [How to config IDD?](#how-to-config-idd)
  - [1. **Prerequisites**](#1-prerequisites)
  - [2. **Login to the MDM Hub Console**](#2-login-to-the-mdm-hub-console)
  - [3. **Define Data Models in MDM Hub**](#3-define-data-models-in-mdm-hub)
  - [4. **Set Up IDD Configuration in the Hub Console**](#4-set-up-idd-configuration-in-the-hub-console)
  - [5. **Configure Task Management and Workflows**](#5-configure-task-management-and-workflows)
  - [6. **Configure Suspect Processing for Match/Merge**](#6-configure-suspect-processing-for-matchmerge)
  - [7. **Customize IDD UI**](#7-customize-idd-ui)
  - [8. **Define Role-Based Access Control (RBAC)**](#8-define-role-based-access-control-rbac)
  - [9. **Deploy the IDD Application**](#9-deploy-the-idd-application)
  - [10. **Monitor and Optimize**](#10-monitor-and-optimize)
  - [Summary of Key Configurations in IDD](#summary-of-key-configurations-in-idd)
- [What are all entities in Informatica MDM? e.g. "Customer" "Orders."](#what-are-all-entities-in-informatica-mdm-eg-customer-orders)
  - [1. **Customer Data Domain**](#1-customer-data-domain)
  - [2. **Product Data Domain**](#2-product-data-domain)
  - [3. **Supplier and Vendor Data Domain**](#3-supplier-and-vendor-data-domain)
  - [4. **Finance and Transactional Data Domain**](#4-finance-and-transactional-data-domain)
  - [5. **Location and Address Data Domain**](#5-location-and-address-data-domain)
  - [6. **Employee Data Domain**](#6-employee-data-domain)
  - [7. **Asset and Resource Data Domain**](#7-asset-and-resource-data-domain)
  - [8. **Contract and Legal Data Domain**](#8-contract-and-legal-data-domain)
  - [9. **Healthcare and Patient Data Domain** (Specific to healthcare organizations)](#9-healthcare-and-patient-data-domain-specific-to-healthcare-organizations)
  - [10. **Industry-Specific Entities**](#10-industry-specific-entities)
  - [Key Considerations When Defining Entities in Informatica MDM](#key-considerations-when-defining-entities-in-informatica-mdm)
  - [Conclusion](#conclusion)
- [For a Telco, it has business on wireless, high-speed internet, health etc. what entities should we choose for its MDM app?](#for-a-telco-it-has-business-on-wireless-high-speed-internet-health-etc-what-entities-should-we-choose-for-its-mdm-app)
  - [1. **Telecommunications (Wireless and Internet Services)**](#1-telecommunications-wireless-and-internet-services)
  - [2. **Healthcare (Telco Health)**](#2-healthcare-telco-health)
  - [3. **Internet and TV Services**](#3-internet-and-tv-services)
  - [4. **Enterprise and Business Solutions**](#4-enterprise-and-business-solutions)
  - [5. **Common Cross-Domain Entities**](#5-common-cross-domain-entities)
  - [Summary of Key Entities for Telco MDM](#summary-of-key-entities-for-telco-mdm)
- [How to build a custom app using Informatica APIs?](#how-to-build-a-custom-app-using-informatica-apis)
  - [1. **Identify Your Use Cases**](#1-identify-your-use-cases)
  - [2. **Understand Informatica APIs**](#2-understand-informatica-apis)
  - [3. **Set Up Your Development Environment**](#3-set-up-your-development-environment)
  - [4. **Authenticate and Access Informatica APIs**](#4-authenticate-and-access-informatica-apis)
  - [5. **Fetch Master Data from Informatica MDM**](#5-fetch-master-data-from-informatica-mdm)
  - [6. **Create, Update, or Merge Data**](#6-create-update-or-merge-data)
    - [**Create a New Record**](#create-a-new-record)
    - [**Update a Record**](#update-a-record)
    - [**Merge Records**](#merge-records)
  - [7. **Integrate Data Quality Checks**](#7-integrate-data-quality-checks)
  - [8. **Create a Front-End for Data Stewards**](#8-create-a-front-end-for-data-stewards)
  - [9. **Security and Role-Based Access Control (RBAC)**](#9-security-and-role-based-access-control-rbac)
  - [10. **Test and Deploy**](#10-test-and-deploy)
  - [Summary](#summary)
- [What are the results after this API call? The 12346 will be merged to 12345?](#what-are-the-results-after-this-api-call-the-12346-will-be-merged-to-12345)
  - [**API Call Breakdown**](#api-call-breakdown)
  - [**Expected Results of the Merge Operation**](#expected-results-of-the-merge-operation)
  - [**Post-Merge State**](#post-merge-state)
  - [Conclusion](#conclusion-1)
- [How to undo a merge?](#how-to-undo-a-merge)
  - [Steps to Undo a Merge in Informatica MDM](#steps-to-undo-a-merge-in-informatica-mdm)
    - [1. **Identify the Records**](#1-identify-the-records)
    - [2. **Use the Unmerge API**](#2-use-the-unmerge-api)
    - [3. **Check Response for Success**](#3-check-response-for-success)
    - [4. **Verify the Unmerge**](#4-verify-the-unmerge)
  - [Important Considerations](#important-considerations)
  - [Alternative: Manual Unmerge in Informatica Data Director (IDD)](#alternative-manual-unmerge-in-informatica-data-director-idd)
  - [Conclusion](#conclusion-2)
- [How to deploy and use Informatica MDM SaaS in GCP?](#how-to-deploy-and-use-informatica-mdm-saas-in-gcp)
  - [1. **Provision Informatica MDM SaaS**](#1-provision-informatica-mdm-saas)
  - [2. **Access the Informatica MDM SaaS Console**](#2-access-the-informatica-mdm-saas-console)
  - [3. **Configure the MDM Environment**](#3-configure-the-mdm-environment)
  - [4. **Integrate Data Sources**](#4-integrate-data-sources)
  - [5. **Security Configuration**](#5-security-configuration)
  - [6. **Testing the Configuration**](#6-testing-the-configuration)
  - [7. **Go Live with MDM SaaS**](#7-go-live-with-mdm-saas)
  - [8. **Ongoing Maintenance and Optimization**](#8-ongoing-maintenance-and-optimization)
  - [9. **Leverage GCP Capabilities**](#9-leverage-gcp-capabilities)
  - [10. **Integration with Other GCP Services**](#10-integration-with-other-gcp-services)
  - [Conclusion](#conclusion-3)
- [What are the components / tools in a end to end Informatica MSM SaaS app?](#what-are-the-components--tools-in-a-end-to-end-informatica-msm-saas-app)
  - [1. **Informatica MDM SaaS**](#1-informatica-mdm-saas)
  - [2. **Data Integration Tools**](#2-data-integration-tools)
  - [3. **Data Quality Tools**](#3-data-quality-tools)
  - [4. **User Interface Components**](#4-user-interface-components)
  - [5. **APIs**](#5-apis)
  - [6. **Monitoring and Analytics Tools**](#6-monitoring-and-analytics-tools)
  - [7. **Security and Compliance Components**](#7-security-and-compliance-components)
  - [8. **Cloud Infrastructure Components**](#8-cloud-infrastructure-components)
  - [9. **Integration with External Systems**](#9-integration-with-external-systems)
  - [Summary](#summary-1)
- [How to use Informatica Cloud Integration to integrate data from external or legacy applications?](#how-to-use-informatica-cloud-integration-to-integrate-data-from-external-or-legacy-applications)
  - [Step-by-Step Guide to Using Informatica Cloud Integration](#step-by-step-guide-to-using-informatica-cloud-integration)
  - [1. **Log in to Informatica Cloud**](#1-log-in-to-informatica-cloud)
  - [2. **Set Up Connections**](#2-set-up-connections)
  - [3. **Create a Mapping**](#3-create-a-mapping)
  - [4. **Configure the Task**](#4-configure-the-task)
  - [5. **Run the Task**](#5-run-the-task)
  - [6. **Monitor and Manage Integrations**](#6-monitor-and-manage-integrations)
  - [7. **Handling Data Quality**](#7-handling-data-quality)
  - [8. **Set Up Incremental Loads (Optional)**](#8-set-up-incremental-loads-optional)
  - [9. **Error Handling and Notifications**](#9-error-handling-and-notifications)
  - [Example Use Case](#example-use-case)
  - [Conclusion](#conclusion-4)
- [I've attached my CV for a role Informatica MDM Lead. I will have an interview soon. What should I do?](#ive-attached-my-cv-for-a-role-informatica-mdm-lead-i-will-have-an-interview-soon-what-should-i-do)
    - [1. **Review Key Job Responsibilities**](#1-review-key-job-responsibilities)
    - [2. **Emphasize Relevant Experience**](#2-emphasize-relevant-experience)
    - [3. **Focus on Technical Skills**](#3-focus-on-technical-skills)
    - [4. **Demonstrate Leadership**](#4-demonstrate-leadership)
    - [5. **Prepare for Scenario-based Questions**](#5-prepare-for-scenario-based-questions)
    - [6. **Brush Up on Agile and DevOps Methodologies**](#6-brush-up-on-agile-and-devops-methodologies)

## How to install Informatica MDM SaaS?

Installing **Informatica MDM SaaS** (Master Data Management as a Service) involves several steps, from provisioning the service on the cloud to configuring and integrating it with your enterprise systems. Here's a high-level guide to help you through the process:

### 1. **Provision Informatica MDM SaaS Account**

- **Sign Up for Informatica Cloud**: If you don't already have an account, you'll need to sign up for the Informatica Cloud (MDM SaaS) service via Informatica's website.
- **Choose Subscription Plan**: Based on your organization's needs, choose a suitable Informatica MDM SaaS plan. This will depend on factors like data volume, number of users, and data governance requirements.
- **Set Up the Account**: Once you have access to the Informatica Cloud services, you'll need to set up your account with appropriate security configurations, including role-based access controls for different teams.

### 2. **Configure Infrastructure & Security**

- **Cloud Environment Setup**: Identify the cloud environment that will host the MDM (e.g., AWS, Azure, or GCP). You'll need to integrate the MDM SaaS with your existing cloud infrastructure.
- **Network Configuration**: Ensure that the network settings are secure, including firewall rules, VPN, and access controls to securely connect to your cloud services. You'll want to whitelist IP addresses or enable secure VPN access if needed.
- **Security Settings**: Enable encryption at rest and in transit for all sensitive data stored in the cloud, configure authentication mechanisms, and apply data masking and encryption techniques for compliance.

### 3. **Set Up MDM SaaS Environment**

- **Create Master Data Model**: Once you have access to the MDM SaaS dashboard, the first step is to set up the master data model (Business Entities, Relationships, etc.). Define your business entities (customers, products, etc.) and the relationships between them.
- **Data Stewardship and Workflows**: Configure the data stewardship workflows that will manage data ownership, validation, and exception handling in the cloud-based environment.
- **Match/Merge Rules**: Define the match and merge rules for data deduplication and survivorship. This ensures that data across multiple systems is consistent, accurate, and up to date.

### 4. **Data Integration**

- **Integrate with Source Systems**: Connect the MDM SaaS to your source systems (e.g., databases, ERP systems, CRM systems). Informatica's **Cloud Application Integration** and **Cloud Data Integration** tools will help you set up these connections and manage data flows.
- **API Setup**: If your organization uses APIs to pull data, configure API-driven integration within the MDM SaaS platform. Informatica provides pre-built connectors for common systems, but custom connectors can also be created using RESTful or SOAP APIs.
- **Configure Data Synchronization**: Set up real-time or batch synchronization jobs to continuously pull data from your source systems into the MDM SaaS. This can be configured using **Informatica Cloud Integration** tools for ETL (Extract, Transform, Load) operations.

### 5. **Data Quality and Governance Configuration**

- **Configure Data Quality**: Implement data quality rules to cleanse and validate the data being ingested into MDM SaaS. This ensures data is accurate, consistent, and complete.
- **Set Up Data Governance Policies**: Use Informatica's governance tools to set up policies for data access, quality, and ownership. Configure dashboards and monitoring tools to track data quality KPIs.

### 6. **Deploy the MDM SaaS Solution**

- **Final Testing**: Test the entire setup by running pilot data loads or synchronizations. Check for data integrity, performance, and quality across all connected systems.
- **Go Live**: Once the testing is successful, deploy the MDM SaaS solution live. Ensure your teams are trained on how to manage and use the system for ongoing data stewardship.
- **Monitor and Optimize**: Set up monitoring and alerting for the MDM SaaS environment to ensure performance, availability, and security. Use the provided dashboards and reports to track the status of your master data in real time.

### 7. **Post Go-Live Maintenance**

- **Monitor Performance**: Continuously monitor the performance of MDM processes, ensuring that real-time data flows and batch jobs are functioning optimally.
- **Data Stewardship**: Ensure that the data stewardship team can manage master data workflows and resolve any issues in the system.
- **Regular Updates**: Apply updates and patches to the system as Informatica releases new versions and features.

---

### Tools You'll Use

- **Informatica Cloud**: For managing cloud-based MDM services.
- **Informatica Cloud Data Integration**: For connecting and integrating various data sources.
- **Informatica Cloud Application Integration**: For real-time application integrations.
- **Informatica Data Quality**: For ensuring data integrity and cleansing in the cloud.

<!-- Would you like more details on a specific step, such as setting up integration or configuring match/merge rules? -->

## How to configure Informatica MDM match/merge rules?

Configuring **Informatica MDM match/merge rules** is essential for identifying and merging duplicate records to create a single, consolidated "golden record" in your Master Data Management (MDM) system. Here's a step-by-step guide to configure match/merge rules in **Informatica MDM**:

---

### 1. **Understand the Match/Merge Process**

- **Match Rules**: These are rules that help identify duplicate records by comparing specific fields (such as names, emails, addresses) across different records. Based on thresholds, records are either considered matches or non-matches.
- **Merge Rules**: Once duplicate records are identified, merge rules determine how the system consolidates those records into a single "golden record" by prioritizing certain data fields (e.g., keeping the most recent or the most reliable value).

---

### 2. **Access the Hub Console for Match/Merge Configuration**

- **Log in to the MDM Hub Console**: Use your administrator credentials to log in.
- Navigate to the **Data Director** and go to the **Match & Merge** section.
- Select the **Entity** (such as Customer, Product, Supplier, etc.) for which you want to configure match/merge rules.

---

### 3. **Define Match Columns**

- **Choose Match Columns**: The first step in setting up match rules is defining which columns (attributes) you want to compare. For example, for customer records, you might choose `First Name`, `Last Name`, `Email`, `Address`, and `Phone Number`.
  - Select columns that are critical for identifying duplicates based on your business needs.
  - These columns must exist in the source data model.
- **Standardization**: Before matching, apply standardization rules to ensure that data is consistently formatted. For example:
  - Convert names to uppercase.
  - Remove special characters (like hyphens) from phone numbers.
  - Format addresses using consistent postal code formats.

   **Steps**:

- In the Hub Console, navigate to **Schema** > **Match Column**.
- Select the business entity and define which columns will be used in matching.

---

### 4. **Configure Match Rule Logic**

- **Exact Match vs. Fuzzy Match**:
  - **Exact Match**: This requires the data in the selected fields to be exactly the same. Use this for fields like **email addresses** or **social security numbers**.
  - **Fuzzy Match**: For fields where data might have slight variations (e.g., names, addresses), use fuzzy matching to account for typos, abbreviations, or formatting differences.
    - Common techniques include **Soundex** (for names) or **Edit Distance** (for minor spelling variations).

   **Steps**:

- Go to **Match Rule Sets** in the Hub Console.
- Choose the appropriate match columns and configure **exact** or **fuzzy matching** for each column.
- For example:
  - For the `First Name` column, use **fuzzy matching** (Soundex).
  - For the `Email` column, use **exact matching**.

- **Weighted Matching**: Assign weights to each match column to indicate its importance in the matching process. For instance:
  - Give a higher weight to `Email` than `First Name` because email addresses are typically more reliable identifiers.

---

### 5. **Set Match Rule Thresholds**

- **Match Threshold**: Set a **threshold score** to determine when records should be considered a match. The threshold is based on the total score calculated from the weights assigned to each column. For example:
  - If the total score exceeds 85%, the records are considered a match.
- **Suspect Threshold**: You can also set a **suspect threshold** for records that don't meet the exact match criteria but are flagged for manual review (e.g., records that score between 70% and 85%).

   **Steps**:

- Go to the **Match Rules** configuration section and set the **threshold** and **suspect threshold**.
- Test different threshold values to strike a balance between too many false positives and too many missed matches.

---

### 6. **Configure Merge Rules (Survivorship Rules)**

- **Survivorship Rules** determine which record attributes will be retained when two records are merged. You can specify which record's data should be prioritized based on business rules.
- Common approaches include:
  - **Most Recent**: Keep the most recent data based on a timestamp field.
  - **Most Reliable Source**: Keep data from the most trusted or preferred source system.
  - **Field-Based Priority**: Define a priority for specific fields (e.g., keep `Phone Number` from Source A but `Email` from Source B).

   **Steps**:

- In the Hub Console, navigate to **Merge Rules**.
- For each attribute, define how the system will handle conflicting values during merging. For example:
  - Use **latest update** for the `Phone Number` field.
  - Use **preferred source system** for the `Address` field.

---

### 7. **Test Match/Merge Configuration**

- **Test Matching**: Run test batches to check if your match rules correctly identify duplicates without generating too many false positives. Adjust weights and thresholds as necessary.
  - Use a **test data set** to validate that the match rules identify duplicates accurately.
- **Test Merging**: Simulate merging of duplicate records and ensure that the **survivorship rules** are working as expected (e.g., correct data is kept in the golden record).

---

### 8. **Deploy and Monitor**

- **Deploy Match/Merge Rules**: Once the rules are finalized and tested, deploy them in the production environment.
- **Set Up Monitoring**: Monitor the system for matching errors, performance issues, or incorrect merges. You can configure dashboards to track match/merge efficiency.
- **Ongoing Tuning**: Continuously fine-tune match/merge rules as data sources evolve or new patterns in data quality emerge.

---

### Example Scenario

For a **Customer Master** in MDM, your match/merge configuration might look like this:

- **Match Columns**: `First Name`, `Last Name`, `Email`, `Phone Number`, `Address`
- **Matching Logic**:
  - `First Name` and `Last Name`: Fuzzy match with Soundex.
  - `Email`: Exact match.
  - `Phone Number`: Exact match.
  - `Address`: Fuzzy match using edit distance or address standardization.
- **Match Threshold**: 85% (above this, records are considered a match).
- **Suspect Threshold**: 70% to 85% (manual review required).
- **Merge Rules**:
  - Keep the **most recent update** for the `Phone Number`.
  - Prioritize data from **preferred systems** for `Address`.
  - Retain the `Email` field from the source with the **highest reliability score**.

---

By following these steps, you can configure effective match/merge rules in Informatica MDM to improve data quality and create a unified, accurate master record.

## How to config Informatica MDM SaaS?

Configuring **Informatica MDM SaaS** involves setting up key components such as master data models, match/merge rules, workflows, security policies, and data governance. Here's a step-by-step guide to help you configure Informatica MDM SaaS:

### 1. **Access the Informatica MDM SaaS Platform**

- **Login**: Log in to your Informatica Cloud account and navigate to the **MDM SaaS module**.
- **MDM Hub Console**: Open the MDM Hub console, which is the interface for configuring all aspects of the MDM solution.

### 2. **Configure the Data Model**

- **Business Entity Creation**:
  - Define **business entities** (such as Customer, Product, Supplier) that you will manage in the MDM. Each entity represents a master data record.
  - Create relationships between different business entities (e.g., Customer and Orders).
  - You can use pre-configured templates or customize your own entity definitions based on your organization's needs.

- **Attributes and Hierarchies**:
  - Define the attributes for each business entity (e.g., Customer Name, Address, Email for Customer entity).
  - Set up **hierarchies** that establish parent-child relationships between business entities. For example, you may have a hierarchy where a "Region" is a parent of "Country" entities.

- **Cross-Referencing**:
  - Configure cross-references to track where data is coming from across various source systems (e.g., ERP, CRM, legacy systems).
  - Ensure that your master data is linked to the corresponding records from the source systems.

### 3. **Define Match/Merge Rules**

- **Match Rule Configuration**:
  - Define **match rules** that identify duplicate records based on certain attributes. For example, you can configure rules to match customers by name, email, or phone number.
  - Use **fuzzy matching** techniques to account for data variations such as typos or formatting differences.
  - Fine-tune match rule thresholds to control how strictly records need to match for them to be considered duplicates.

- **Merge Rule Configuration**:
  - Set up **merge rules** that dictate how duplicate records should be merged into a single "golden record". You can prioritize certain data sources or rely on certain attributes for the merge process.
  - Implement **survivorship rules** that determine which data values are kept after the merge (e.g., keep the most recent address).

### 4. **Set Up Data Governance and Stewardship**

- **Data Governance Policies**:
  - Define governance policies to ensure data accuracy, completeness, and compliance. These may include data validation rules, ownership assignments, and approval workflows.
  - Set up **data lineage** to track where data originates and how it moves through the system.

- **Data Stewardship Workflows**:
  - Configure workflows to handle data stewardship activities such as resolving data discrepancies, merging records manually, or validating changes.
  - Assign data stewardship roles and permissions to different users. For example, some users may have the ability to approve changes, while others may only review flagged data.
  - Use Informatica's **Data Steward Console** for data validation, exception management, and manual corrections.

### 5. **Data Integration Configuration**

- **Informatica Cloud Integration**:
  - Use **Informatica Cloud Data Integration** to configure how data is imported into the MDM from source systems. This may include batch processing or real-time integrations using APIs.
  - Configure **connectors** to various systems like Salesforce, ERP systems, or custom databases (Oracle, SQL Server, etc.).

- **Data Synchronization**:
  - Set up **data synchronization** jobs to ensure that the MDM receives up-to-date data from your source systems on a regular basis.
  - Define **ETL processes** for extracting, transforming, and loading (ETL) data from source systems into the MDM.

### 6. **Security and Role-Based Access Control**

- **Access Control**:
  - Set up **role-based access control** (RBAC) to manage which users or groups can view, modify, or manage master data. You can define roles like **Data Stewards**, **Data Owners**, or **Administrators**.

- **Data Masking**:
  - Implement **data masking** to protect sensitive data such as personal information (e.g., Social Security Numbers, credit card details) based on user roles.

- **Encryption**:
  - Configure **encryption** for data both at rest and in transit. Ensure that the appropriate encryption keys are managed securely.

- **Audit Trails**:
  - Set up **audit logs** to track changes to master data, including who made the changes and when. This helps maintain compliance with data governance policies.

### 7. **Testing and Validation**

- **Data Validation**:
  - After setting up the configurations, run **test batches** to ensure that your match/merge rules, governance workflows, and data quality rules are functioning correctly.
  - Validate that data is correctly transformed, loaded, and displayed in the MDM system.

- **Performance Testing**:
  - Perform **performance testing** to ensure that the MDM system can handle data volumes and data processing tasks, especially if you're working with large-scale data.

### 8. **Monitoring and Alerts**

- **Dashboard Configuration**:
  - Set up **dashboards** to monitor the performance of your MDM system, track key metrics such as data quality scores, and visualize master data distribution across the system.

- **Alerts and Notifications**:
  - Configure alerts for key events such as data discrepancies, failed match/merge processes, or system performance issues.
  - Ensure data stewards are notified in real-time if there's an issue with the data, allowing for immediate correction.

### 9. **Deployment and Maintenance**

- **Deployment to Production**:
  - After thoroughly testing in a development or staging environment, deploy the MDM configurations to production.

- **Ongoing Maintenance**:
  - Regularly monitor the system for performance and data integrity issues. Update configurations, rules, and workflows as business requirements evolve.
  - Schedule regular backups and ensure disaster recovery plans are in place for the MDM system.

---

### Tools and Consoles Used

- **MDM Hub Console**: For configuring data models, match/merge rules, and governance workflows.
- **Informatica Cloud Integration**: For connecting and synchronizing data from different source systems.
- **Data Steward Console**: For managing data validation and manual data stewardship activities.
- **Informatica Cloud Data Quality**: For setting up and monitoring data quality rules.

By following these steps, you'll be able to configure your Informatica MDM SaaS environment effectively and ensure that your master data is clean, accurate, and properly governed.

<!-- Would you like more detailed information on a particular configuration step, such as match/merge rules or setting up governance workflows? -->

## How to migrate from informatica MDM Single Tenant to MDM SaaS?

Migrating from **Informatica MDM Single Tenant** (on-premise or self-hosted) to **Informatica MDM SaaS** involves multiple phases, including planning, data migration, configuration, testing, and validation. Here's a detailed guide on how to migrate from Informatica MDM Single Tenant to MDM SaaS:

---

### 1. **Planning and Assessment**

- **Assess the Current MDM Environment**:
  - Evaluate the existing single-tenant MDM environment, including data volumes, business entities, match/merge rules, and integrations.
  - Review customizations, data models, workflows, and any integrations with other systems (like ERP, CRM, etc.) to ensure they are compatible with MDM SaaS.

- **Identify SaaS Requirements**:
  - Gather business and technical requirements for the new SaaS platform. This includes performance, data integrity, security, scalability, and compliance needs.
  - Plan for any potential changes in infrastructure, data governance, or cloud integration.

- **Determine Data Migration Strategy**:
  - Identify the **ETL (Extract, Transform, Load)** approach for migrating master data from on-premise to the cloud.
  - Define if the migration will be done **all at once (big bang)** or in **phases** (staggered cutover), and whether you need real-time data sync during the migration process.

---

### 2. **Prepare the MDM SaaS Environment**

- **Provision MDM SaaS**:
  - Set up the MDM SaaS environment in Informatica Cloud, ensuring cloud-specific configurations such as networking, access control, and security policies are in place.

- **Configure the MDM SaaS Data Model**:
  - Replicate your **data model** (business entities, attributes, and relationships) from the single-tenant system in the MDM SaaS environment.
  - Configure hierarchies, relationships, and reference data based on the existing on-premise configuration.

- **Match/Merge and Data Quality Configuration**:
  - Re-create your match/merge rules, survivorship rules, and data quality configurations in MDM SaaS.
  - Ensure that all data governance and data quality rules are aligned with the cloud system.

- **Set Up Data Stewardship Workflows**:
  - Define and configure workflows for data stewardship and data validation. Ensure these workflows are compatible with the MDM SaaS architecture.

---

### 3. **Data Migration**

- **Extract Data from Single Tenant System**:
  - Extract master data, metadata, and configuration data (match/merge rules, business entities, workflows) from the on-premise MDM system.
  - Ensure that the data is transformed into a format that is compatible with the MDM SaaS environment.

- **Data Cleansing and Validation**:
  - Perform **data cleansing** to ensure that only high-quality data is migrated to the cloud. This includes deduplication, data standardization, and data validation.
  - Use **Informatica Data Quality** to apply data validation rules and prepare the data for migration.

- **Data Transformation**:
  - If the data models or attributes have changed between the on-premise and SaaS versions, apply the necessary data transformations. Ensure schema alignment with the new cloud-based data model.

- **Data Loading to MDM SaaS**:
  - Load the data into the MDM SaaS platform using **Informatica Cloud Data Integration** or similar tools.
  - Configure batch jobs or real-time sync jobs for migrating large datasets.
  - Validate the data in MDM SaaS to ensure that it matches the source data from the single-tenant system.

---

### 4. **System Integration and API Configuration**

- **Integration with External Systems**:
  - Recreate integrations with other systems (e.g., CRM, ERP, third-party applications) in the MDM SaaS platform. Use **API-driven integration** to connect MDM SaaS with other cloud-based systems or on-prem systems.
  - Leverage pre-built connectors in Informatica Cloud, or use REST/SOAP APIs to rebuild custom integrations.

- **Real-time and Batch Synchronization**:
  - Configure real-time or batch synchronization to ensure that master data in the SaaS environment stays up-to-date with source systems.
  - Set up **Informatica Cloud Application Integration** for real-time data sync where needed.

---

### 5. **Security and Compliance Setup**

- **Configure Role-Based Access Control (RBAC)**:
  - Set up role-based access controls (RBAC) in MDM SaaS to manage who can view, edit, or manage master data. Map user roles from the single-tenant system to the cloud environment.

- **Implement Data Security Policies**:
  - Configure **data encryption**, both at rest and in transit, to protect sensitive data.
  - Ensure compliance with data protection regulations like **GDPR**, **HIPAA**, or **CCPA**, depending on your industry.

- **Set Up Data Masking**:
  - Implement **data masking** techniques for sensitive information (e.g., personal data, financial records) in the MDM SaaS environment.

---

### 6. **Testing and Validation**

- **Test Data Migration**:
  - Validate the accuracy and completeness of the migrated data by comparing it to the source data in the single-tenant system.
  - Ensure that the **match/merge rules** and **survivorship rules** are functioning correctly, and that there are no duplicates or incorrect data merges.

- **Test Integrations**:
  - Test integrations between MDM SaaS and other systems (e.g., ERP, CRM). Ensure that data flows between systems in real-time or batch as intended.

- **Performance Testing**:
  - Conduct **performance testing** to ensure that the MDM SaaS platform can handle the expected data volume and load efficiently.

---

### 7. **Cutover and Go-Live**

- **Final Data Migration**:
  - Once testing is complete, perform the final data migration (if needed) and ensure that any real-time updates during the migration process are captured.
  - Synchronize any final changes made in the single-tenant system after the initial migration, and ensure all data is current in the SaaS environment.

- **Switch Over to SaaS**:
  - Decommission the single-tenant system and switch over to the SaaS environment for live operations.
  - Ensure that the users, data stewards, and other stakeholders are trained on how to use the new MDM SaaS platform.

- **Monitoring and Post-Go-Live Support**:
  - Set up **monitoring tools** to track system performance and data quality in real-time.
  - Provide ongoing support to resolve any issues, optimize workflows, or address post-migration concerns.

---

### 8. **Post-Migration Optimization and Maintenance**

- **Monitor System Performance**:
  - Continuously monitor the performance of the MDM SaaS platform using dashboards and alerts. Identify and resolve any bottlenecks or issues.

- **Refine Data Governance and Quality**:
  - Regularly audit the master data to ensure that data governance policies are being followed and data quality remains high.

- **Ongoing Updates**:
  - Apply updates and patches provided by Informatica to keep the SaaS platform current and secure.

---

### Tools and Services to Use

- **Informatica Cloud Data Integration**: For ETL and migrating data from the on-prem system to the cloud.
- **Informatica Cloud Application Integration**: For API-driven and real-time integration between MDM SaaS and other systems.
- **Informatica Data Quality**: For data cleansing, validation, and quality management during the migration process.
- **MDM Hub Console**: To configure and manage the MDM environment in SaaS.

By following these steps, you can ensure a smooth and secure migration from an Informatica MDM Single Tenant to the cloud-based MDM SaaS.

## Manual review

**Informatica MDM** provides a built-in user interface for **manual review** through the **Informatica Data Director (IDD)**. IDD allows data stewards to manually review, resolve, and merge duplicate records that are flagged by the match/merge process as "suspects." You can configure and use this UI without needing to build a custom web app, but a custom web app can also be developed if you want more tailored functionality.

### **Informatica Data Director (IDD) Overview**

The IDD tool is a web-based interface designed specifically for data stewardship and manual data management tasks in MDM. With IDD, you can:

- Review and manage **suspect records** that are flagged by the MDM match process but don't meet the automatic merge threshold.
- **Manually merge or unmerge** records if required.
- View **audit logs** of changes made to master data.
- **Approve or reject match/merge decisions** suggested by the system.

---

### **Key Features of Informatica Data Director (IDD) for Manual Review:**

1. **Suspect Record Management:**
   - In the IDD UI, data stewards can easily see records that fall into the "suspect" category, i.e., those records that didn't meet the automatic merge threshold but are similar enough to be flagged for manual review.
   - From here, you can review the matching criteria (such as email, name, or phone number discrepancies) and decide whether the records should be merged or kept as separate entities.

2. **Manual Merging of Records:**
   - The **Merge Manager** in IDD allows users to manually merge records that the match process flagged but didn't automatically merge. Data stewards can review conflicting fields (e.g., addresses, phone numbers) and choose which values should be kept in the final master record.
   - You can configure **survivorship rules** in IDD to assist with merging decisions.

3. **Unmerge Records:**
   - If two records were incorrectly merged, IDD allows data stewards to **unmerge** them. This ensures data accuracy and gives control over maintaining the correct master records.

4. **Data Stewardship Workflows:**
   - **Approval Workflows**: When suspect records are flagged, they may need approval from data stewards. IDD allows you to set up workflows where records are routed to specific users or teams for approval.
   - You can configure the workflows based on various factors like data quality, source systems, or business rules.

5. **Audit Trails and Change Logs:**
   - Every action taken within IDD, including manual merges, unmerges, or changes to master data, is logged. This provides a detailed **audit trail** for compliance and data governance purposes.
   - Data stewards can review these logs to track changes, who made them, and when.

6. **User Role Management:**
   - Role-based access control (RBAC) is supported in IDD, allowing different users to have specific privileges (e.g., viewing records, merging records, approving changes).
   - You can configure roles for data stewards, administrators, and others to manage access to various data stewardship activities.

---

### **Why Use IDD Instead of a Custom Web App?**

1. **Out-of-the-box Functionality**:
   - IDD is specifically designed for managing master data in Informatica MDM, with all the necessary tools for reviewing, managing, and merging records built-in.
   - It integrates seamlessly with MDM, avoiding the need for additional API integration or manual setup.

2. **Customizable UI**:
   - While IDD provides a default UI, you can customize it to match your organization's specific needs (e.g., custom fields, specific workflows, branding).

3. **Cost and Maintenance**:
   - Using IDD reduces the need for building and maintaining a custom web application. Informatica continuously updates and supports IDD, reducing your overall maintenance efforts.

4. **Workflow Integration**:
   - IDD integrates well with other Informatica tools, including **Informatica Data Quality (IDQ)**, for seamless data validation and cleansing workflows.

---

### **When to Consider Building a Custom Web App?**

You might consider building a custom web app if:

- **Complex Custom Requirements**: Your organization has highly specialized workflows or UI requirements that cannot be met by IDD.
- **Integration with Other Systems**: If you need tighter integration with non-Informatica tools or business systems and want more control over the user experience.
- **Custom Branding or User Experience**: If your organization prefers a branded, highly customized web interface with unique UX features for data stewards.

In this case, you could use the **Informatica MDM APIs** to develop a custom application that pulls data from the MDM, enables manual reviews and merges, and then writes the updated data back to the MDM system.

### **Tools for Building a Custom Web App**

- **Informatica MDM REST APIs**: Use these APIs to interact with the MDM Hub, allowing your custom app to retrieve and update master data.
- **Informatica Cloud Application Integration**: If integrating with other systems, use Informatica's cloud application integration tools to streamline real-time communication between the MDM and other business systems.

---

### **Recommendation:**

Start with **Informatica Data Director (IDD)** if it meets your business requirements. It's a purpose-built tool with strong functionality for managing master data, performing manual reviews, and handling workflows.

If you find that your organization has very unique needs, or if IDD's capabilities fall short for your use cases, then you can consider building a custom web app using Informatica MDM APIs.

<!-- Would you like guidance on configuring IDD, or do you want to explore options for building a custom app using Informatica APIs? -->

## How to config IDD?

Configuring **Informatica Data Director (IDD)** involves setting up the UI to manage data stewardship, workflows, and manual data review processes. The goal of configuring IDD is to ensure that data stewards can easily manage, validate, and manually review master data within your **Informatica MDM** system. Here's a step-by-step guide to configure IDD:

---

### 1. **Prerequisites**

- Ensure that **Informatica MDM Hub** and **IDD** are installed and set up in your environment.
- You should have access to the **Informatica MDM Hub Console** and **MDM Hub Server**.
- You need to have administrative privileges to create and configure IDD applications.

---

### 2. **Login to the MDM Hub Console**

- **Open the MDM Hub Console**: Log in using your administrator credentials.
- Navigate to the **Configuration** section where you can manage and configure the IDD application.

---

### 3. **Define Data Models in MDM Hub**

Before configuring IDD, you need to have **Business Entities** and **Relationships** defined in the MDM Hub. This is necessary because IDD uses these entities for data management and review.

- **Define Business Entities**: In the MDM Hub Console, ensure that **Business Entities** like Customer, Product, or Supplier are already configured. These will represent the master data that data stewards will manage in IDD.
- **Define Relationships**: Set up relationships between entities if needed. For example, a "Customer" can be related to "Orders."

---

### 4. **Set Up IDD Configuration in the Hub Console**

   1. **Create a New IDD Application**:
      - In the MDM Hub Console, go to the **Data Director** section.
      - Click **Add Application** to create a new IDD application.
      - Provide a **Name** for the application (e.g., "Customer Management") and assign the appropriate **Entity Type** (e.g., Customer).

   2. **Configure the Application Layout**:
      - **Configure Pages and Tabs**: Define the layout for the data stewards. You can set up pages, tabs, and sections where business entities, attributes, and relationships will be displayed. For example, you can have separate tabs for customer details, contact information, and orders.
      - **Entity Details Page**: Configure the main page where users can view and manage records for a specific entity. Add fields and attributes (like name, address, phone number) to this page based on your business needs.

   3. **Configure Record Views**:
      - Set up **record views** for data stewards to search, filter, and view records in IDD. Define search parameters, such as searching by `Customer ID`, `Name`, or `Email`.
      - Use filters to allow stewards to search by different attributes and display results in a list or grid format.
      - **Example**: In the Customer Management app, configure record views to show records based on the `Last Name` or `Customer ID`.

---

### 5. **Configure Task Management and Workflows**

- **Workflow Configuration**:
  - Set up workflows for handling tasks such as manual review, validation, and approvals. This allows data stewards to follow a guided process when resolving data conflicts or reviewing suspect records.
  - Define **task assignment** and approval workflows. For example, configure tasks to be automatically assigned to specific data stewards or groups based on predefined rules (e.g., geographic region or business unit).
  - Configure statuses such as "Pending," "In Review," "Approved," or "Rejected" to track task progress.

- **Task Inbox Configuration**:
  - The **Task Inbox** is where data stewards will find tasks assigned to them for review. Configure the inbox layout so that stewards can easily see which tasks need attention and take action.
  - Add columns to the inbox view, such as `Task Name`, `Assigned To`, `Due Date`, `Priority`, and `Status`.

---

### 6. **Configure Suspect Processing for Match/Merge**

- **Set Up Suspect Record Management**:
  - Enable the **Suspect Processing** feature to allow data stewards to review and resolve suspect records. These are records that the match/merge rules have flagged but require manual intervention.
  - Define how suspect records will be displayed in the IDD UI. For example, show all suspect records for a specific business entity (e.g., all customers flagged as potential duplicates).

- **Manual Merge and Unmerge**:
  - Configure manual merge/unmerge functionality. This allows data stewards to manually review two or more records flagged as duplicates and decide whether to merge them or keep them separate.
  - Set up the **merge preview** so that stewards can see which attributes will be merged before confirming the action.

---

### 7. **Customize IDD UI**

- **Field Layout**:
  - Customize the display of fields for each business entity. For example, you can define which fields should be mandatory, which fields should be editable, and how data should be presented (e.g., text box, dropdown).
  - Configure **validation rules** and error messages for each field to ensure data quality during manual entry or updates.

- **Localization** (Optional):
  - If your organization operates in multiple regions, you can configure localization for the IDD application. This ensures that the UI supports different languages and formats (e.g., date, time, number formats).

- **Custom Actions**:
  - Create custom actions that data stewards can trigger from the IDD UI. For example, you can set up actions to export data, send notifications, or trigger automated workflows.

---

### 8. **Define Role-Based Access Control (RBAC)**

- **Set Up User Roles**:
  - Configure role-based access control (RBAC) to ensure that only authorized users can access or modify certain records. Assign roles like **Data Steward**, **Administrator**, or **Viewer**, and configure the appropriate access levels.
  - Define what each role can do within IDD, such as viewing records, editing fields, merging records, or resolving data conflicts.

- **Field-Level Security**:
  - In addition to role-based access, you can configure **field-level security** to restrict access to sensitive fields. For example, a junior data steward might not have access to view or edit financial or personally identifiable information (PII).

---

### 9. **Deploy the IDD Application**

- Once the configuration is complete, **deploy** the IDD application to the environment.
- Test the application by logging in as a data steward and verifying that all the views, workflows, and permissions are working as expected.

---

### 10. **Monitor and Optimize**

- **Monitor Data Stewardship Tasks**: Use built-in monitoring tools to track data stewardship tasks, approvals, and manual merges.
- **Performance Tuning**: Optimize performance by reviewing audit logs and resolving bottlenecks in workflows or data management tasks.

---

### Summary of Key Configurations in IDD

- **Data model**: Business entities and relationships from MDM Hub.
- **UI layout**: Configuring pages, tabs, record views, and field layouts.
- **Suspect processing**: Managing suspect records flagged for manual review.
- **Task management**: Setting up workflows, task inbox, and approval processes.
- **Role-based access**: Defining user roles and field-level security.
- **Merge/unmerge functionality**: Allowing manual review and management of duplicate records.

By following these steps, you can configure Informatica Data Director (IDD) to streamline data stewardship activities and ensure high-quality master data management within your organization.

## What are all entities in Informatica MDM? e.g. "Customer" "Orders."

In **Informatica MDM**, **entities** represent the key data objects that you manage in your master data. These entities vary depending on the business domain, such as customer, product, or supplier data, and they reflect the core objects that need to be de-duplicated, governed, and merged to create a single "golden record." Here's a breakdown of commonly used entities in Informatica MDM, organized by business domain:

---

### 1. **Customer Data Domain**

- **Customer**: Represents an individual or organization that interacts with your business, such as buyers, clients, or subscribers. Attributes may include `Name`, `Email`, `Phone`, `Address`, and `Customer ID`.
- **Account**: Represents the account associated with a customer, which could include information such as `Account Number`, `Status`, `Type`, and `Balance`.
- **Contacts**: Individuals associated with an organization or customer, such as a point of contact for business dealings.
- **Demographics**: Information related to customer attributes like `Age`, `Gender`, `Income`, etc.
- **Preferences**: Customer preferences, such as `Preferred Communication Method`, `Marketing Opt-ins`, etc.

---

### 2. **Product Data Domain**

- **Product**: Represents the products or services your business offers. Attributes include `Product ID`, `Product Name`, `Category`, `Price`, and `Description`.
- **Product Catalog**: The complete list of products, including variations, SKUs, and product hierarchies.
- **Inventory**: Information related to stock levels, warehouses, and availability of products.
- **Pricing**: Contains pricing details, discounts, and special offers for products.
- **Product Lifecycle**: Captures data about the stages in a product's life, such as launch, active, discontinued, or end-of-life.
- **Bill of Materials (BOM)**: Data about the components and materials required to manufacture a product.

---

### 3. **Supplier and Vendor Data Domain**

- **Supplier**: Represents vendors or suppliers who provide goods or services to the business. Attributes include `Supplier Name`, `Supplier ID`, `Contact Information`, `Products Supplied`, etc.
- **Contract**: Captures details of agreements between suppliers and the business, including `Contract ID`, `Start Date`, `End Date`, and `Terms`.
- **Supplier Location**: Represents the various locations or distribution centers associated with a supplier.
- **Purchase Orders**: Orders placed with suppliers, including `PO Number`, `Order Date`, `Delivery Date`, `Quantity`, and `Price`.

---

### 4. **Finance and Transactional Data Domain**

- **Orders**: Represents sales or purchase orders, including `Order ID`, `Order Date`, `Customer`, `Product`, `Quantity`, and `Total Price`.
- **Invoice**: Data related to customer billing, including `Invoice Number`, `Invoice Date`, `Amount`, `Payment Status`, and `Due Date`.
- **Payments**: Information about payments made by customers or to suppliers, including `Payment ID`, `Payment Method`, `Amount`, and `Date`.
- **Transaction**: Details about financial transactions, such as sales, returns, or refunds. Attributes include `Transaction ID`, `Type`, `Date`, and `Amount`.
- **Account Balances**: Represents the current balance of customer or supplier accounts.

---

### 5. **Location and Address Data Domain**

- **Location**: Represents a physical or virtual location, such as office locations, warehouses, or regions.
- **Address**: Captures address details associated with customers, suppliers, or products. Attributes may include `Street`, `City`, `State`, `Postal Code`, and `Country`.
- **Geography**: Geospatial data, such as `Latitude`, `Longitude`, and `Geographical Region`.
- **Shipping Information**: Captures shipping addresses, delivery preferences, and carrier details.

---

### 6. **Employee Data Domain**

- **Employee**: Represents employees of the organization. Attributes include `Employee ID`, `Name`, `Email`, `Phone Number`, `Position`, and `Department`.
- **Job Role**: Defines roles within the organization, such as `Title`, `Level`, and `Responsibilities`.
- **Compensation**: Employee compensation details, including `Salary`, `Bonuses`, and `Benefits`.
- **Performance**: Information about employee performance evaluations, ratings, and feedback.
- **Hierarchy**: Represents organizational structure, defining managers, reports, and team structures.

---

### 7. **Asset and Resource Data Domain**

- **Asset**: Represents business-owned resources, such as IT equipment, vehicles, or real estate. Attributes may include `Asset ID`, `Asset Type`, `Purchase Date`, `Value`, and `Depreciation`.
- **Inventory**: Data on items held in stock, including `SKU`, `Quantity`, and `Location`.
- **Maintenance Records**: Information about service history, repairs, and maintenance schedules for assets.
- **Warranty**: Captures warranty information for business-owned assets or products sold.

---

### 8. **Contract and Legal Data Domain**

- **Contract**: Legal agreements between entities, such as customers, suppliers, or partners. Attributes include `Contract ID`, `Start Date`, `End Date`, `Terms`, and `Parties Involved`.
- **Compliance**: Records related to compliance with industry standards, regulations, and legal requirements.
- **Policy**: Represents policies related to business operations, data management, or employee guidelines.

---

### 9. **Healthcare and Patient Data Domain** (Specific to healthcare organizations)

- **Patient**: Represents individuals receiving healthcare services. Attributes include `Patient ID`, `Name`, `Age`, `Medical History`, and `Treatment Plan`.
- **Provider**: Healthcare providers or medical professionals, including `Provider ID`, `Name`, `Specialty`, `Location`, and `License`.
- **Claims**: Represents insurance claims made for medical services, including `Claim ID`, `Date`, `Amount`, and `Status`.
- **Treatment**: Information about medical treatments or procedures performed on a patient.

---

### 10. **Industry-Specific Entities**

- **Vehicle** (Automotive industry): Captures vehicle details such as `VIN`, `Make`, `Model`, `Year`, and `Ownership History`.
- **Real Estate** (Real estate industry): Represents property listings or holdings, including `Property ID`, `Address`, `Price`, `Square Footage`, and `Owner`.
- **Energy Asset** (Energy sector): Represents assets in energy management, such as `Power Plant`, `Wind Turbine`, or `Grid`.

---

### Key Considerations When Defining Entities in Informatica MDM

- **Business Relevance**: The entities you define should align with your organization's business domain and the type of master data you want to manage.
- **Relationships**: Defining relationships between entities (e.g., Customers and Orders, Suppliers and Products) is critical for maintaining data integrity.
- **Custom Entities**: You can create **custom entities** based on your specific business requirements if they aren't available out-of-the-box.

---

### Conclusion

The entities in Informatica MDM will depend on the domain and data you manage. Standard entities like **Customer**, **Product**, **Order**, and **Supplier** are common across most industries. However, you can extend the MDM schema to include custom entities that reflect the unique needs of your organization.

<!-- Would you like further details on how to define custom entities or set up relationships between entities in MDM? -->

## For a Telco, it has business on wireless, high-speed internet, health etc. what entities should we choose for its MDM app?

For **Telco**, which operates in wireless, high-speed internet, and health sectors, the **entities** in the MDM application should be tailored to these diverse business areas. Below are some suggested entities that would be suitable for Telco's MDM system, organized by business domain:

### 1. **Telecommunications (Wireless and Internet Services)**

- **Customer**:
  - Represents individuals or businesses subscribing to Telco services (wireless, internet, etc.).
  - Attributes: `Customer ID`, `Name`, `Phone Number`, `Email`, `Address`, `Account Type (individual/business)`.

- **Service Subscription**:
  - Represents the services that a customer subscribes to, such as wireless, internet, or TV.
  - Attributes: `Subscription ID`, `Customer ID`, `Service Type (wireless/internet)`, `Plan Type (monthly/prepaid)`, `Activation Date`, `Status`, `Data Cap`, `Speed`.

- **Device**:
  - Represents wireless devices like smartphones or modems that are tied to customer accounts.
  - Attributes: `Device ID`, `IMEI`, `Device Type`, `Make`, `Model`, `Operating System`, `Activation Date`.

- **Billing and Payments**:
  - Represents billing details and payment history associated with a customer's account.
  - Attributes: `Invoice ID`, `Customer ID`, `Billing Cycle`, `Amount Due`, `Due Date`, `Payment Status`, `Payment Method`.

- **Network Location**:
  - Represents geographic areas where services like wireless and internet are offered.
  - Attributes: `Location ID`, `Area Code`, `Region`, `Latitude`, `Longitude`, `Service Availability (wireless/internet)`.

- **Service Plan**:
  - Represents the details of various plans and packages offered by Telco.
  - Attributes: `Plan ID`, `Plan Name`, `Price`, `Data Limit`, `Speed (internet)`, `Features (unlimited talk, roaming)`.

- **Contract**:
  - Represents contractual agreements with customers for specific service plans.
  - Attributes: `Contract ID`, `Start Date`, `End Date`, `Terms`, `Cancellation Fees`.

- **Call and Data Usage**:
  - Represents the details of a customer's usage of wireless services.
  - Attributes: `Usage ID`, `Customer ID`, `Call Duration`, `Data Usage`, `Billing Period`.

---

### 2. **Healthcare (Telco Health)**

- **Patient**:
  - Represents individuals receiving healthcare services through Telco Health.
  - Attributes: `Patient ID`, `Name`, `Date of Birth`, `Gender`, `Address`, `Medical History`.

- **Healthcare Provider**:
  - Represents doctors, nurses, or other medical professionals registered with Telco Health.
  - Attributes: `Provider ID`, `Name`, `Specialty`, `License Number`, `Location`, `Contact Information`.

- **Appointment**:
  - Represents the details of patient appointments with healthcare providers.
  - Attributes: `Appointment ID`, `Patient ID`, `Provider ID`, `Date`, `Time`, `Service Type`.

- **Medical Device**:
  - Represents any healthcare devices provided to patients through Telco Health services (e.g., monitoring devices).
  - Attributes: `Device ID`, `Device Type`, `Serial Number`, `Patient ID`, `Issue Date`.

- **Health Insurance**:
  - Represents insurance policies linked to patients for healthcare services.
  - Attributes: `Insurance ID`, `Patient ID`, `Provider`, `Coverage`, `Effective Date`.

---

### 3. **Internet and TV Services**

- **Internet Subscription**:
  - Represents the details of high-speed internet service provided to customers.
  - Attributes: `Subscription ID`, `Plan ID`, `Speed`, `Data Cap`, `Activation Date`, `Customer ID`.

- **Set-Top Box/Modem**:
  - Represents devices provided for internet or TV service.
  - Attributes: `Device ID`, `Serial Number`, `Model`, `Firmware`, `Activation Date`, `Customer ID`.

- **Channel Package**:
  - Represents the details of TV channel packages offered by Telco.
  - Attributes: `Package ID`, `Package Name`, `Channels Included`, `Price`, `Activation Date`.

---

### 4. **Enterprise and Business Solutions**

- **Business Customer**:
  - Represents business entities that subscribe to Telco services.
  - Attributes: `Business ID`, `Business Name`, `Industry`, `Contact Person`, `Phone`, `Email`, `Business Type (SME, Enterprise)`.

- **Enterprise Service Agreement**:
  - Represents contractual agreements with business customers for services like internet, wireless, or cloud solutions.
  - Attributes: `Agreement ID`, `Business ID`, `Service Level`, `Start Date`, `End Date`, `Terms`.

- **Cloud Service Subscription**:
  - Represents subscriptions to cloud-based services provided by Telco to business customers.
  - Attributes: `Subscription ID`, `Business ID`, `Service Type`, `Storage Size`, `Price`, `Start Date`, `End Date`.

---

### 5. **Common Cross-Domain Entities**

- **Location**:
  - Represents a customer's or business's physical address.
  - Attributes: `Location ID`, `Customer ID`, `Street`, `City`, `Province`, `Postal Code`, `Country`.

- **Service Ticket**:
  - Represents issues or support requests related to a service.
  - Attributes: `Ticket ID`, `Customer ID`, `Issue Description`, `Service Type`, `Status`, `Resolution Date`.

---

### Summary of Key Entities for Telco MDM

1. **Customer**: Individuals or businesses subscribed to wireless, internet, TV, or health services.
2. **Service Subscription**: Details of services like wireless, high-speed internet, or cloud services.
3. **Device**: Devices used by customers, such as smartphones, modems, or healthcare devices.
4. **Patient** and **Healthcare Provider**: Entities specific to Telco Health, representing patients and healthcare professionals.
5. **Billing and Payments**: Billing cycles, payment statuses, and invoices for customers.
6. **Service Plan and Contract**: Information about service plans and contractual agreements with customers.
7. **Call and Data Usage**: Details about customer usage of wireless services.
8. **Business Customer**: Businesses subscribed to Telco enterprise services.

These entities should be aligned with Telco's diverse business offerings and serve as the backbone for managing master data across their services.

<!-- Would you like help with defining relationships between these entities or configuring them in Informatica MDM? -->

## How to build a custom app using Informatica APIs?

Building a custom app using **Informatica APIs** allows you to extend the capabilities of your **Informatica MDM** system and create a user-friendly interface tailored to your business needs. Whether you want to create a data stewardship app, custom workflows, or integrate with other systems, the **Informatica REST APIs** enable you to programmatically interact with the MDM Hub.

Here's a step-by-step guide to building a custom app using Informatica APIs:

---

### 1. **Identify Your Use Cases**

   Before diving into development, define the specific functionalities your custom app needs to handle. Common use cases include:

- Managing master data (e.g., customer, product, or supplier records).
- Viewing, editing, or merging records.
- Performing data quality checks.
- Implementing custom workflows for data stewardship.
- Integrating with third-party systems (e.g., CRM, ERP) to push/pull data.

### 2. **Understand Informatica APIs**

   Informatica MDM offers several API types:

- **Informatica MDM REST APIs**: These APIs allow you to interact with MDM Hub programmatically, including querying, creating, updating, and merging master data.
- **Informatica Cloud APIs**: For cloud-based services like Informatica Cloud Integration, these APIs enable data movement and integration with cloud sources.
- **Informatica Data Quality (IDQ) APIs**: If your app involves data quality checks, you can leverage IDQ APIs to validate and cleanse data.

### 3. **Set Up Your Development Environment**

- Choose a **backend technology** for your app, such as **Node.js**, **Java**, **Python**, or **.NET**, depending on your development team's expertise.
- Set up a **front-end framework** like **React**, **Angular**, or **Vue.js** to build the user interface (UI).
- Ensure you have access to your **Informatica MDM Hub** or **Informatica Cloud** environment with appropriate API credentials (API keys, OAuth tokens, etc.).

---

### 4. **Authenticate and Access Informatica APIs**

- **Authentication**: Use **OAuth 2.0** or **Basic Authentication** depending on the API type. For Informatica Cloud APIs, you’ll typically use OAuth tokens, while for on-prem MDM APIs, you might use basic authentication.
  - Obtain the required credentials such as **Client ID**, **Client Secret**, and **OAuth Token**.
  - Authenticate your app to obtain an access token:

       ```bash
       curl -X POST https://<InformaticaURL>/auth/login \
       -H 'Content-Type: application/json' \
       -d '{"username": "your-username", "password": "your-password"}'
       ```

       This call will return a token that you can use in subsequent API calls.

- **Base URL**: Identify the correct **base URL** for your API calls:
  - For MDM Hub: `https://<MDM-Hub-URL>/mdm/api`
  - For Informatica Cloud: `https://<Cloud-Environment-URL>/ic/api`

- **API Documentation**: Use **Informatica API documentation** to explore available endpoints. Here’s the official documentation for reference:
  - **MDM REST API**: <https://docs.informatica.com/data-governance-and-quality/mdm/apis/rest-api.html>
  - **Informatica Cloud REST API**: <https://docs.informatica.com/cloud-api>
  
---

### 5. **Fetch Master Data from Informatica MDM**

   Use the **MDM REST API** to retrieve master data. For example, to fetch a **Customer** entity:

- **Endpoint**: `/mdm/api/v1/resources/entity/customers`
- **GET Request** Example:

     ```bash
     curl -X GET https://<MDM-Hub-URL>/mdm/api/v1/resources/entity/customers \
     -H "Authorization: Bearer <Access-Token>" \
     -H "Content-Type: application/json"
     ```

   This returns the list of customers, including attributes like `CustomerID`, `Name`, `Address`, etc.

- **Response** (JSON format):

     ```json
     {
       "customers": [
         {
           "CustomerID": "12345",
           "Name": "John Doe",
           "Email": "john.doe@example.com",
           "PhoneNumber": "+1-555-555-5555"
         },
         ...
       ]
     }
     ```

### 6. **Create, Update, or Merge Data**

#### **Create a New Record**

   To create a new customer in the MDM system:

- **POST Request**:

     ```bash
     curl -X POST https://<MDM-Hub-URL>/mdm/api/v1/resources/entity/customers \
     -H "Authorization: Bearer <Access-Token>" \
     -H "Content-Type: application/json" \
     -d '{
           "CustomerID": "12346",
           "Name": "Jane Doe",
           "Email": "jane.doe@example.com",
           "PhoneNumber": "+1-555-555-5556"
         }'
     ```

   This creates a new customer record in the MDM system.

#### **Update a Record**

   To update an existing record:

- **PUT Request**:

     ```bash
     curl -X PUT https://<MDM-Hub-URL>/mdm/api/v1/resources/entity/customers/12345 \
     -H "Authorization: Bearer <Access-Token>" \
     -H "Content-Type: application/json" \
     -d '{
           "Name": "John Doe",
           "PhoneNumber": "+1-555-555-1234"
         }'
     ```

#### **Merge Records**

   Use the **merge** API to combine duplicate records based on match/merge rules:

- **POST Request**:

     ```bash
     curl -X POST https://<MDM-Hub-URL>/mdm/api/v1/resources/entity/customers/merge \
     -H "Authorization: Bearer <Access-Token>" \
     -H "Content-Type: application/json" \
     -d '{
           "masterId": "12345",
           "survivorId": "12346"
         }'
     ```

---

### 7. **Integrate Data Quality Checks**

   Use **Informatica Data Quality (IDQ) APIs** to validate and cleanse data before saving it to MDM. For example, you might call an API to check for invalid phone numbers or addresses before submitting a new record.

- **API Endpoint**: `/dq/api/v1/resources/validation`
- **Example Request**:

     ```bash
     curl -X POST https://<DQ-URL>/dq/api/v1/resources/validation \
     -H "Authorization: Bearer <Access-Token>" \
     -H "Content-Type: application/json" \
     -d '{
           "data": {
             "PhoneNumber": "+1-555-555-1234"
           }
         }'
     ```

---

### 8. **Create a Front-End for Data Stewards**

- **React (or Angular/Vue)**: Use **React** to create a user-friendly interface that data stewards can use to view, edit, and merge records.
  - Set up a page for viewing **Customer Records**, where you fetch customer data from the API and display it in a table.
  - Create **forms** for editing customer details, where changes are submitted via the API.

   Example using React to fetch and display customer data:

   ```javascript
   useEffect(() => {
     fetch('https://<MDM-Hub-URL>/mdm/api/v1/resources/entity/customers', {
       method: 'GET',
       headers: {
         'Authorization': `Bearer ${accessToken}`,
         'Content-Type': 'application/json'
       }
     })
     .then(response => response.json())
     .then(data => setCustomers(data.customers))
   }, []);
   ```

---

### 9. **Security and Role-Based Access Control (RBAC)**

- Implement **RBAC** to ensure only authorized users can access or modify sensitive data.
- Use the API to enforce access control, ensuring certain endpoints or data modifications are restricted to users with specific roles.

---

### 10. **Test and Deploy**

- **Test the API calls** extensively to ensure data accuracy, performance, and security.
- Set up continuous integration/continuous deployment (CI/CD) pipelines to automate testing and deployment of your custom app.
- **Deploy** the app in your cloud environment (e.g., AWS, Azure) or on-prem servers.

---

### Summary

By using Informatica APIs, you can build a fully functional custom app that integrates with your MDM system, allowing data stewards to interact with master data, resolve duplicates, and manage data quality. The app can be tailored to your business needs with a custom UI, API integration, and workflow automation.

<!-- Would you like more help with a specific feature, such as building the front-end or configuring specific API calls? -->

## What are the results after this API call? The 12346 will be merged to 12345?

```bash
curl -X POST https://<MDM-Hub-URL>/mdm/api/v1/resources/entity/customers/merge \
-H "Authorization: Bearer <Access-Token>" \
-H "Content-Type: application/json" \
-d '{
      "masterId": "12345",
      "survivorId": "12346"
    }'
```

Yes, in the provided `curl` command, the API call is designed to merge two records in the Informatica MDM system. Here's a breakdown of the operation and the expected results:

### **API Call Breakdown**

- **Endpoint**:

  ```text
  POST https://<MDM-Hub-URL>/mdm/api/v1/resources/entity/customers/merge
  ```

  This endpoint is used for merging customer records.

- **Headers**:
  - **Authorization**: The `Bearer <Access-Token>` is used to authenticate the request. Ensure the access token has the necessary permissions to perform merge operations.
  - **Content-Type**: Set to `application/json`, indicating that the payload is in JSON format.

- **Payload** (`-d` option):

  ```json
  {
    "masterId": "12345",
    "survivorId": "12346"
  }
  ```

  - **masterId**: This is the ID of the "master" record that will be retained after the merge. In this case, it's `12345`.
  - **survivorId**: This is the ID of the "survivor" record that will be merged into the master record. In this case, it's `12346`.

### **Expected Results of the Merge Operation**

1. **Record Consolidation**:
   - The record with `survivorId` (`12346`) will be merged into the record with `masterId` (`12345`).
   - Attributes from `12346` may be combined with those from `12345` according to the **survivorship rules** configured in your MDM system. This means that depending on your setup, certain fields may prioritize values from one record over the other.

2. **Data Quality**:
   - The system will ensure that any data quality rules are adhered to during the merge process, preserving the integrity of the master data.

3. **Audit Logs**:
   - An entry will typically be created in the audit log, documenting the merge action, including who performed the action, the date and time, and any changes made to the master record.

4. **Success Response**:
   - If the merge operation is successful, you should receive a success response (usually a `200 OK` status or a specific success message) indicating that the merge has completed successfully.

   Example response:

   ```json
   {
     "status": "success",
     "message": "Records merged successfully.",
     "mergedRecordId": "12345",
     "mergedInto": "12346"
   }
   ```

5. **Error Handling**:
   - If there are issues with the merge (e.g., if the records do not exist, conflicts arise due to data quality rules, or if the user lacks permissions), you will receive an error response with an appropriate status code (like `400 Bad Request` or `403 Forbidden`) and a message detailing the problem.

### **Post-Merge State**

- After the merge:
  - The record with `survivorId` (`12346`) will no longer exist as a separate record.
  - All relevant data from `12346` will be incorporated into `12345` according to the defined survivorship rules.
  
### Conclusion

By executing the provided API call, you will effectively merge `12346` into `12345`, consolidating the customer data into a single master record while ensuring adherence to the system's data governance policies.

## How to undo a merge?

To **undo a merge** in **Informatica MDM**, you typically need to rely on the **unmerge functionality** provided by the MDM system. When you merge records, Informatica MDM retains historical information about the merge operation, allowing you to revert to the original state if necessary. Here's how to perform an unmerge operation:

### Steps to Undo a Merge in Informatica MDM

#### 1. **Identify the Records**

   Before you can undo a merge, you need to know:

- The **master record ID** that was retained after the merge.
- The **survivor record ID** that was merged into the master record.

#### 2. **Use the Unmerge API**

   If you have access to the Informatica MDM REST API, you can perform an unmerge operation programmatically.

- **Endpoint**: The typical endpoint to perform an unmerge would look like:

     ```text
     POST https://<MDM-Hub-URL>/mdm/api/v1/resources/entity/customers/unmerge
     ```

- **Payload**: You will need to specify the IDs of the records involved in the unmerge operation. The payload usually looks like this:

     ```json
     {
       "masterId": "12345",
       "survivorId": "12346"
     }
     ```

- **cURL Example**:

     ```bash
     curl -X POST https://<MDM-Hub-URL>/mdm/api/v1/resources/entity/customers/unmerge \
     -H "Authorization: Bearer <Access-Token>" \
     -H "Content-Type: application/json" \
     -d '{
           "masterId": "12345",
           "survivorId": "12346"
         }'
     ```

#### 3. **Check Response for Success**

- If the unmerge operation is successful, you should receive a response indicating success:

     ```json
     {
       "status": "success",
       "message": "Records unmerged successfully."
     }
     ```

- The system will restore the original state of the records before the merge, meaning that `12346` will now exist as a separate record again.

#### 4. **Verify the Unmerge**

- After performing the unmerge, it's a good practice to verify that the records are restored as expected. You can do this by querying the customer records:

     ```bash
     curl -X GET https://<MDM-Hub-URL>/mdm/api/v1/resources/entity/customers/12346 \
     -H "Authorization: Bearer <Access-Token>"
     ```

- Check that the attributes are correctly populated and that the record exists independently from `12345`.

### Important Considerations

- **Access and Permissions**: Ensure that the API user has the necessary permissions to perform unmerge operations.
- **Data Integrity**: Be aware that unmerging records might lead to data quality issues if the records were merged based on certain data quality rules. Review any inconsistencies that might arise.
- **Audit Trail**: The MDM system typically logs unmerge actions for audit purposes. Check audit logs if you need to review previous merge and unmerge actions.

### Alternative: Manual Unmerge in Informatica Data Director (IDD)

If you're using **Informatica Data Director (IDD)** for manual data management, you can also perform an unmerge operation directly in the UI:

1. **Navigate to the Suspect Records**: Find the merged record (master record).
2. **Select the Merged Record**: Open the details for the master record.
3. **Unmerge Option**: Look for an option like **"Unmerge"** within the record details or under actions.
4. **Confirm Unmerge**: Follow any prompts to confirm the unmerge action.

### Conclusion

Using the API or the IDD UI, you can effectively undo a merge operation in Informatica MDM. This allows you to restore previously merged records while maintaining data integrity and governance standards.

## How to deploy and use Informatica MDM SaaS in GCP?

Deploying and using **Informatica MDM SaaS** in **Google Cloud Platform (GCP)** involves several steps, from provisioning the Informatica service to configuring it for use with your data sources. Below is a comprehensive guide to help you through the process.

### 1. **Provision Informatica MDM SaaS**

- **Sign Up for Informatica MDM SaaS**: If you don't already have an account, sign up for Informatica MDM SaaS on the Informatica website.
- **Choose a Subscription Plan**: Select a subscription plan that suits your organization’s requirements regarding data volume, user count, and features.
- **Provision the Environment**: During the provisioning process, choose GCP as the cloud provider. Informatica will set up the necessary infrastructure on GCP for your MDM SaaS environment.

### 2. **Access the Informatica MDM SaaS Console**

- After provisioning, you’ll receive access credentials to log in to the **Informatica MDM SaaS Console**.
- Use these credentials to log in and start configuring your MDM environment.

### 3. **Configure the MDM Environment**

- **Set Up Business Entities**: Define the business entities (like Customer, Product, Supplier) that will be managed in MDM. Specify attributes, relationships, and hierarchies for these entities.
- **Match and Merge Rules**: Configure match and merge rules to identify and consolidate duplicate records. Define how records will be matched based on certain criteria and what the survivorship rules will be.
- **Data Governance**: Set up data governance policies to ensure data quality, security, and compliance. Configure data stewardship workflows for manual review and validation of master data.

### 4. **Integrate Data Sources**

- **Connect to Data Sources**: Use Informatica’s data integration capabilities to connect to your source systems. This can include databases, cloud applications, and on-premises systems.
- **Data Mapping and ETL**: Define how data will be extracted, transformed, and loaded (ETL) into the MDM system. Use Informatica’s Cloud Data Integration tools for this purpose.
- **Configure API Access**: If you need to connect to third-party systems or expose MDM data through APIs, set up API endpoints as needed.

### 5. **Security Configuration**

- **User Management**: Set up user accounts and roles in Informatica MDM SaaS. Define permissions based on user roles to control access to data and functionalities.
- **Data Security**: Implement data security measures such as encryption at rest and in transit. Configure access controls and data masking for sensitive information.

### 6. **Testing the Configuration**

- **Load Test Data**: Before going live, load some test data into the MDM system to validate the configuration. Check that match/merge rules work as expected.
- **Verify Integrations**: Test all integrations to ensure data flows correctly from source systems into MDM and that any data quality checks are functioning.

### 7. **Go Live with MDM SaaS**

- **Final Data Migration**: If applicable, perform the final data migration from existing systems to the MDM system.
- **Training and Documentation**: Provide training to users on how to use the Informatica MDM SaaS platform, including how to access data, perform merges, and manage records.
- **Monitor the Environment**: Once live, actively monitor the MDM system for performance and data quality. Use the built-in analytics and monitoring tools provided by Informatica.

### 8. **Ongoing Maintenance and Optimization**

- **Performance Tuning**: Continuously monitor and optimize the performance of your MDM system based on usage patterns and data growth.
- **Regular Audits**: Conduct regular data audits to ensure compliance with data governance policies and maintain data quality.
- **Update Policies and Rules**: Periodically review and update match/merge rules and governance policies as business requirements change.

### 9. **Leverage GCP Capabilities**

- Utilize GCP services to enhance your Informatica MDM deployment:
  - **BigQuery**: For advanced analytics and reporting on master data.
  - **Cloud Storage**: To store backups or staging data before loading it into MDM.
  - **Cloud Functions**: For serverless integration or processing tasks.
  - **Dataflow**: For real-time data processing and ETL jobs.

### 10. **Integration with Other GCP Services**

- If you are using other GCP services, you can integrate them with Informatica MDM SaaS to enhance your data ecosystem. For example:
  - Use **Cloud Pub/Sub** for event-driven architecture and real-time data processing.
  - Use **Cloud Scheduler** for automating data load tasks or ETL jobs.

---

### Conclusion

Deploying and using Informatica MDM SaaS in GCP involves careful planning and configuration to ensure that your master data is effectively managed and integrated with your existing systems. By following these steps, you can create a robust MDM solution that leverages the capabilities of both Informatica and Google Cloud Platform.

## What are the components / tools in a end to end Informatica MSM SaaS app?

Building an end-to-end **Informatica MDM SaaS** application involves various components and tools that work together to manage master data efficiently. Here's a breakdown of the key components and tools typically involved in an Informatica MDM SaaS application:

### 1. **Informatica MDM SaaS**

- **Core MDM Hub**: The central component that manages master data entities (e.g., customers, products, suppliers) and enforces data governance policies. It includes features for data matching, merging, and validation.
- **Match and Merge Engine**: This engine identifies duplicate records and merges them based on configurable match/merge rules.

### 2. **Data Integration Tools**

- **Informatica Cloud Data Integration**: Used for ETL (Extract, Transform, Load) processes to move data from source systems (e.g., databases, cloud applications) into the MDM hub.
- **Informatica Cloud Application Integration**: Facilitates real-time integrations with other applications and data sources, ensuring data consistency across systems.

### 3. **Data Quality Tools**

- **Informatica Data Quality (IDQ)**: Helps ensure that the data loaded into the MDM system is clean, accurate, and consistent. This includes profiling, cleansing, and validating data.
- **Data Governance Tools**: Tools to define data policies, manage data lineage, and ensure compliance with data standards and regulations.

### 4. **User Interface Components**

- **Informatica Data Director (IDD)**: A web-based user interface that allows data stewards to manage and validate master data. It provides functionalities for manual review of suspect records, merging/unmerging records, and executing data stewardship workflows.
- **Custom Web Applications**: In some cases, organizations may develop custom applications using the Informatica REST APIs to provide a tailored UI for specific user needs or workflows.

### 5. **APIs**

- **Informatica REST APIs**: These APIs allow for programmatic interaction with the MDM hub. They enable operations such as creating, reading, updating, and deleting records, as well as performing merges and unmerges.

### 6. **Monitoring and Analytics Tools**

- **Informatica Administrator**: Provides tools for monitoring the health of the MDM environment, managing user access, and configuring system settings.
- **Analytics and Reporting Tools**: Use reporting tools like **Tableau**, **Power BI**, or built-in Informatica reporting features to analyze master data, monitor data quality, and generate insights.

### 7. **Security and Compliance Components**

- **Role-Based Access Control (RBAC)**: Manage user roles and permissions to ensure that only authorized personnel can access sensitive master data.
- **Data Masking and Encryption**: Ensure data security through masking sensitive information and encrypting data both at rest and in transit.

### 8. **Cloud Infrastructure Components**

- **Google Cloud Platform (GCP)** (or other cloud providers): The underlying infrastructure where the Informatica MDM SaaS application is hosted. This includes:
  - **Compute Engine**: For running applications and services.
  - **Cloud Storage**: For storing backups, staging data, or temporary data during ETL processes.
  - **BigQuery**: For running analytics on master data and integrating with reporting tools.

### 9. **Integration with External Systems**

- **CRM Systems**: Integration with customer relationship management systems (e.g., Salesforce, Microsoft Dynamics) to synchronize customer data.
- **ERP Systems**: Integration with enterprise resource planning systems (e.g., SAP, Oracle) to manage product and supplier data.
- **Other Business Applications**: Integration with additional business applications (e.g., marketing automation tools, helpdesk systems) to ensure consistent data across the enterprise.

---

### Summary

An end-to-end Informatica MDM SaaS application is comprised of several integrated components and tools, each playing a critical role in managing master data effectively. The combination of MDM core functionality, data integration, data quality, user interfaces, and cloud infrastructure ensures that organizations can maintain high-quality master data while meeting business needs and compliance requirements.

## How to use Informatica Cloud Integration to integrate data from external or legacy applications?

Using **Informatica Cloud Integration** to integrate data from external or legacy applications involves several key steps, including setting up the connections, defining the data mappings, configuring the integration tasks, and executing the jobs. Below is a detailed guide on how to achieve this:

### Step-by-Step Guide to Using Informatica Cloud Integration

### 1. **Log in to Informatica Cloud**

- Access the **Informatica Intelligent Cloud Services (IICS)** portal by logging in with your credentials.
- Navigate to the **Cloud Data Integration** section.

### 2. **Set Up Connections**

   Connections define how Informatica connects to your source and target systems (e.g., databases, applications, or file systems).

- **Create Connection for Source**:
  - Go to the **Connections** tab in the IICS portal.
  - Click on **New Connection** and select the appropriate connection type based on your source (e.g., Oracle, SQL Server, Salesforce, REST API, etc.).
  - Provide the necessary details (e.g., connection name, database URL, username, password, etc.) and test the connection to ensure it’s working.
  
- **Create Connection for Target** (if applicable):
  - Follow the same steps to create a connection for the target system where you want to load the data.

### 3. **Create a Mapping**

   Mappings define how data is transformed and moved from source to target.

- **Go to the Mapping Designer**:
  - Navigate to the **Mappings** tab and click on **New Mapping**.
  - Select your source connection and drag the source object (tables, files, etc.) onto the canvas.

- **Define the Transformation Logic**:
  - You can add transformations as needed (e.g., Filter, Joiner, Expression, Aggregator) to process the data according to your business rules.
  - Map the fields from the source to the target by dragging and dropping fields onto the target object.

- **Set Up Target**:
  - Drag your target object onto the mapping canvas and connect it to the source fields to specify how data should be written to the target.

### 4. **Configure the Task**

   After creating the mapping, you’ll configure a task that will execute the mapping.

- **Create a Task**:
  - Go to the **Tasks** tab and click on **New Task**.
  - Choose **Mapping Task** and select the mapping you created in the previous step.
  - Configure the task properties, including task name, description, and schedule (if you want it to run on a schedule).

- **Task Properties**:
  - Specify parameters such as the execution mode (e.g., **Incremental Load**, **Full Load**) based on your requirements.
  - Set up the **Error Handling** options to manage any errors that may occur during the integration process.

### 5. **Run the Task**

- Once the task is configured, you can run it manually or schedule it to run at specific intervals.
- To run the task:
  - Click on the **Run** button in the task details.
  - Monitor the task execution for any errors or warnings in the **Task Execution Log**.

### 6. **Monitor and Manage Integrations**

- Use the **Monitor** tab to view the status of your tasks, including successful runs, failures, and warnings.
- Review execution logs to troubleshoot any issues or validate data movement.

### 7. **Handling Data Quality**

- If you have data quality rules, consider using **Informatica Data Quality** services to clean, standardize, or validate the data before loading it into the target system.
- You can integrate data quality tasks into your mapping using **Data Quality transformations**.

### 8. **Set Up Incremental Loads (Optional)**

- If you’re integrating from legacy systems, consider setting up incremental loads to capture only the changed data since the last load. This typically involves:
  - Using timestamps or change data capture (CDC) techniques to identify new or updated records.
  - Configuring the mapping and task to filter and process only the necessary records.

### 9. **Error Handling and Notifications**

- Set up error handling in your mapping and task to manage and log errors effectively.
- You can configure notifications to alert users in case of failures or significant events during integration.

### Example Use Case

Suppose you want to integrate customer data from an on-premises SQL Server database into a cloud-based CRM like Salesforce. Here’s a high-level approach:

1. **Set Up Connections**: Create connections for SQL Server (source) and Salesforce (target).
2. **Create Mapping**: Use the mapping designer to define how customer fields (e.g., name, email) from SQL Server should map to Salesforce fields.
3. **Create Task**: Configure a mapping task to execute the data transfer and schedule it to run daily.
4. **Run and Monitor**: Execute the task and monitor its execution through the Informatica Cloud interface.

---

### Conclusion

Using **Informatica Cloud Integration** allows you to seamlessly integrate data from external or legacy applications into your MDM system or other target applications. By following these steps, you can establish reliable data flows that support your business processes and enhance data accuracy and consistency.


