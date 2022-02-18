# az900
AZ 900 Azure Fundamentals

Post account creation to create everything in GUI you need to elevate yourself https://docs.microsoft.com/en-us/azure/role-based-access-control/elevate-access-global-admin\
https://aad.portal.azure.com/#allservices\


Azure Netwroking -- \
https://aviatrix.com/learn-center/cloud-networking/azure-networking-fundamentals/



Lingos -- https://azure.microsoft.com/en-us/overview/cloud-computing-dictionary/ \
Behind the Scenes -- Every Rack has a server called the Fabric Controller and all such Fabric Controllers are connected to orchestrator via a Switch/router etc.\
When we fire a command on CLI or WebUI the same is sent to the Orchestrator and that in turn is sent to the best suitable Fabric Controller.


            Broad ctagories in Azure 
            Compute
            Networking
            Storage
            Mobile
            Databases
            Web
            Internet of Things
            Big Data
            Artificial Intelligence
            DevOps


---------------------------
For Azure there are 3 regions in India.
        West India (Mumbai)
        Central India (Pune)
        South India (Chennai)

Geographies\
Regions\
AZs
Paired Regions\

**Availability Zones are unique physical locations within an Azure region.
Each zone is made up of one or more datacenters equipped with independent power, cooling, and networking.
To ensure resiliency, there's a minimum of three separate zones in all enabled regions.**


https://docs.microsoft.com/en-us/azure/availability-zones/az-overview#regions-that-support-availability-zones

Geography -->An area of the world containing at least one Azure region. There are total 7 geographies in the World. India is a Geography!\
Azure Region --> Minimum 3 AZs in one region. India has 3 regions.\
AZ--> Each zone is made up of one or more datacenters.\


Organizations is Directories in Azure. One account can have multiple Directories i.e one account can be associated to multiple organizations.
Each Direcoty can have multiple Subscriptions.
The account can have multiple subscriptions.

https://www.youtube.com/watch?v=0Jx_oftPCLY


-----------------------------
    Our E2E application has multiple VMs these are grouped together as Availability sets.
    An **availability set** is a logical grouping of two or more VMs that help keep your application available during planned or unplanned maintenance.
    When the VM is part of an availability set, the Azure fabric updates are sequenced so not all of the associated VMs are rebooted at the same time.
    **Fault domain** is a single Rack with multiple Servers in it.
    Your VMs are then sequentially placed across the fault and update domains.
    
    ** With each AS we get 3 FDs and 5 UDs (max 20UDs).**
    

-----------------------------
A principal is an identity acting with certain roles or claims.
A service principal is an identity that is used by a service or application.


-----------------------------
An action group is a collection of notification preferences defined by the owner of an Azure subscription. Azure Monitor and Service Health alerts use action groups to notify users that an alert has been triggered.


-----------------------------
You can create multiple virtual networks per subscription and per region. You can create multiple subnets within each virtual network.\
Azure routes network traffic between all subnets in a virtual network, by default.
Resources of different regions can be grouped together in a single RG.
The underlying technology that powers resource groups is the Azure Resource Manager (ARM). 

A RG in one region can have VNETs of other region.

You cannot span a VNET across multiple RGs. Neither can you create a subnet of a vnet in another RG.


-----------------------------
Powershell can be installed on Linux, Macos also.
Same ways Azure cli can be installed on windows.

-----------------------------

Data that is copied to an Azure Storage account is maintained automatically in at least three copies is CORRECT because within the primary region, three copies of data are maintained synchronously and then it is copied asynchronously to the secondary region. Therefore, at least three copies of the data is maintained at all times by the Azure Storage account.

-----------------------------
Because when VMs are deployed in two or more resource groups it will NOT prevent the VMs from a single data center failure.

-----------------------------
GDPR is for EU.\
ISO is for all industries.\
Azure Government delivers a dedicated cloud enabling only US government agencies and their partners to transform mission-critical workloads to the cloud. These US government agencies include the US federal, US state and local government or their partners.

NIST -- >defines standards used by the United States government

-----------------------------
Help+Support is CORRECT because under this you can find the details regarding the “Planned Maintenance” (Screenshots attached for reference from Azure Portal)

Public preview is available to all customers.

-----------------------------
 Azure DevTest Labs enables developers on teams to efficiently manage virtual machines (VMs) and PaaS resources without waiting for approvals. DevTest Labs creates labs consisting of pre-configured bases or Azure Resource Manager templates. These have all the necessary tools and software that you can use to create environments. You can create environments in a few minutes, as opposed to hours or days.

-----------------------------
using a single azure firewall you can restrict traffic to multiple virtual networks in multiple subscriptions. It's a managed, cloud-based network security service that protects your Azure Virtual Network resources. It’s a fully stateful firewall as a service with built-in high availability and unrestricted cloud scalability.

-----------------------------

Compliance Manager is CORRECT here because it is designed to track an organization's status with regard to regulations or standards. 
Microsoft Trusted Cloud Initiative, and provides support and resources for the legal and compliance community

-----------------------------
Azure Security Center is an advanced, unified infrastructure security management that provides features such as security health monitoring for both cloud and on-premises workloads.
 Azure security center provides a high-level summary of your compliance status for the selected standard based on Security Center assessments data and is organized according to the controls of that standard. The report can be shared with relevant stakeholders and may serve to provide evidence to internal and external auditors.

-----------------------------
Microsoft will provide a minimum of 12 months' notification prior to ending support if no successor product or service is offered—excluding free services or preview releases.

-----------------------------
zure Key Vault” is used to store secrets such as passwords related to Azure Active Directory (Azure AD) user accounts. We an also store other secrets such as certificates, token, keys related to other Azure API services etc.

-----------------------------
Private Previews are generally the first release of a product and customers are invited to try the service to help provide feedback, to understand if the service is something that is needed as well as help to shape the future of the product.

Generally there is a limited number of customers that are invited into a private preview and these customers are expected to spend time with the Product Group* providing their feedback on the product.

When a service goes General availability, it is in full production mode. It is fully supported by SLAs, customer support and is viable for production workloads. Now that the service is live it is also chargeable.



-----------------------------

multiple subscriptions under one account. (generally 50 subscriptions under one account, after opening a support case they could increase up to 200)

-----------------------------
each subscription is a separate entity that you can't merge. Instead you can transfer the ownership of a subscription to another account which will end in, you would have two subscriptions to manage.



-----------------------------
 Management Groups, if a user has multiple subscriptions, he can manage compliance, policies and even access across those multiple Azure subscriptions. All subscriptions within a management group automatically inherit the conditions applied to the management group.


-----------------------------
Azure Security Center is CORRECT because, when the JIT access is configured, the inbound access to VMs is locked down by the Azure Security Center by creating a Network Security Group rule. The ports are locked down for inbound traffic. Security Center automatically configures the Network Security Groups (NSGs) and Azure Firewall to allow inbound traffic to the selected ports and requested source IP addresses or ranges, for the time that was specified. After the time has expired, the Security Center restores the NSGs to their previous states.

-----------------------------
Azure Active Directory Premium P2 guarantees at least 99.9 percent availability and

All paying Azure customers receive a credit if their monthly uptime percentage is below the guaranteed amount in the Service Level Agreement (SLA).



-----------------------------
Must be rehydrated before the data can be accessed is CORRECT because you must first change the tier of the blob to hot or cool. This process is known as rehydration and takes a matter of hours to complete.

-----------------------------

Azure Monitor” like the “Application Insights” and “Log Analytics” etc that will help us to diagnose our application’s issues.

-----------------------------
 it tells us about interactions Microsoft has with you and Microsoft products such as Microsoft services, websites, apps, software, servers, and devices. It is intended to provide openness and honesty about how Microsoft deals with personal data in its products and services. Microsoft privacy statement explains what personal data Microsoft processes, how Microsoft processes it, and for what purposes.

-----------------------------
virtual machines can be moved to the new subscription (please note the guidance for virtual machines).

-----------------------------
The resources in a resource group can be located in different regions than the resource group.
You can apply tags to a resource group. The resources in the resource group don't inherit those tags.
Moving a resource only moves it to a new resource group or subscription. It doesn't change the location of the resource.

-----------------------------

the data in an Azure storage account is automatically replicated (consider it as a “copy” or as a “backup”) within the data center only and NOT to another Azure data center

-----------------------------
You can move an app to another App Service plan, as long as the source plan and the target plan are in the same resource group and geographical region.

The region in which your app runs is the region of the App Service plan it's in. However, you cannot change an App Service plan's region.


-----------------------------
Page blobs are a collection of 512-byte pages optimized for random read and write operations.
An append blob is comprised of blocks and is optimized for append operations. When you modify an append blob, blocks are added to the end of the blob only, via the Append Block operation.


-----------------------------
“All Azure free accounts expire after a specific period”.
 Azure subscription can have only one account administrator.
 One account can have multiple subscriptions but one sunscrition will have only one account admin.
 Each Azure subscription can be managed by using a Microsoft account only”.
 Since Azure Public Cloud is offered by “Microsoft”, users who intend to open an Azure subscription need to have a valid Microsoft account
 Azure services in public preview are not covered under any Service Level Agreement (SLA).
 Inbound data transfer (into Azure) is ALWAYS FREE irrespective of the account in Azure (free or pay-as-you-go subscription).
 After account expires we cannot start a vm. Access to portal works.
 

-----------------------------
NOT all the Azure regions are available to all the customers and the general public.
 only one Azure Free account can be created using the same Microsoft account
 
Resource group belongs to only one subscription (one-to-one relationship), whereas a singe Azure Subscription can contain multiple Azure Resource groups (one-to-many relationship)

tags are NOT inherited and therefore if you assign a tag to a resource group, then all the resources in that resource group are NOT assigned to the same tag.


-----------------------------




-----------------------------

https://docs.microsoft.com/en-us/azure/architecture/aws-professional/databases



|AWS|GCP|Azure|
|-|-|-|
|EC2|Virtual machine instances|Azure Virtual Machines|
|S3|Google Cloud Storage|Azure Blob storage Continers|
|AWS S3 - Infrequent Access ||Azure Cool Blob Storage tier|
|AWS Glacier||Azure Archive Blob Storage|
|EC2|GCE --Google Compute Engine|
|ECS||Azure Container Instances|
|User-Data in EC2|Startup Scripts|Extensions or Cloud-init|
|ASG|Managed Instance Group|Azure Virtual Machine Scale Sets|
|Launch Configuration|Instance Template|
|AZ|Zones|7 Georaphies, each has atlest 1 Region, each region has min 3 AZ, each AZ has min 1 DC|
|ap-south-1|asia-south1 , Delhi WIP|3 regions West India (Mumbai) Central India (Pune) South India (Chennai)|
|ap-south-1 a,b,c|asia-south1 -a,-b,-c|
|VPC|VPC|VNET|
|VPC is AWS Region(In AWS Region means a geography)|VPC is Global|VNET is Region Specific(In Azure Region means a location in a Geography)|
|security groups|firewall rules in vpc| |
|SGs can be used in Inbound/outbound rule definitions.|GCP recommends using SAs for the same.||
|Public IP /NAT etc is needed for Outbound Internet.||Default all Services have outbound Internet connectivity.|
|EBS|Persistent Disk or PD|Data Disks in blob|
|Policies|Permissions|
|st1 and sc1 -- HDD |standard PD -- HDD|
|AWS Lightsail||Azure DevTest Labs||
|EC2 -- Only key|Only Key|VMs -- username and password and keys|
|ec2-user||azureuser|
|Public IP setting is VPC based, VM will get if in that VPC||Public IP is per VM|
|5 IPs are reserved per subnet(1st 4 and last 1)|4 IPs are reserved per primary subnet|5 IP addresses are reserved each subnet|
|CIDR cannot be extended, secondary can be added|for Custom, Subnet CIDR can be extended, for auto no|
|Allowed block min /28 to max /16|Min /29 max /9|/29 to /8|
|Elastic Beanstalk or Heroku|GAE|Azure App Service|
|Spot Instances |preemptible| Azure Spot VMs|
|2 Min Notice||30 Seconds Notice||
|AWS OpsWork||Azure Automation State Configuration|
|Placement groups || proximity placement group|
|Lambda|Cloud Functions|Azure Functions|
|Instance Store|Local SSD|Azure Temporary Disks|
|EFS (only for posix, cannot be mounted over internet witout direct-connect etc)|Cloud File Store|Azure Storage -- > Azure Files (for windows, linux and macos.They can be mounted on-prem over internet.)|
|Storage Gateway||StorSimple||
|Storage Gateway -- File Gateway||Azure File Sync|
|Data Sync||File Sync||
|AWS Image makes one each||Azure Capture/ Make Image make one IMG for all VHDs.|
|AWS Trusted Advisor ||Azure Security Advisor|
|Eventual consistency for Objects in S3|Strong Consistency|
|AWS RDS|Cloud SQL No MariaDB, No Oracle|
|Redhshift -Coloumnar and Athena |Bigquery -Coloumnar and serverless|
|DynamoDB, Cassandra, HBASE|BigTable -- NoSQL|
|Dynamo DB|Cloud Datastore|Azure Table storage, Azure Cosmos DB|
||firebase and |
|SnowCone, Snowball,Snowball Edge, Snow mobile|~~Data~~ Google Transfer Appliance|DataBox (DataBox Disk, Databox and Databox Heavy)|
|||Online Data Box (Databox Edge and Databox Gateway)|
||Storage Transfer Service||
|Route53 -- Registrar|Google Domains  -- Registrar -Supports DNSSEC|
|Route53|CloudDNS|Azure DNS|
|Elastic IP|Static IP|
|ELB(Elastic Load Balancing)|CLB(Cloud Load Balancing)|Azure Load Balancer|
|CloudFront, Akamai|CloudCDN|Azure Content Delivery Network|
|Direct Connect|Dedicated Interconnect| Azure ExpressRoute
|AWS VPN|Cloud VPN|
||Cloud InterConnect|
||Cloud Router|
||CDN Interconnect|
|AWS Sagemaker|Cloud ML engine (Tesnorflow, MXnet)|
|AWS REkognition|Cloud Vision API|
|Polly and Transcribe|Cloud Speech API|
|AWS Comprehend|Cloud Natural Language API|
|AWS Translate|Cloud Transalte API|
|AWS Lex|DialogFlow|
|AWS Rekognition|Cloud Video Intelligence API|
|AWS IoT|Cloud IoT Core|
|AWS SNS,SQS,Kinesis|Cloud Pub/Sub|Azure Queue storage|Event Grid, Notification Hub|
|AWS Glue -- ETL|DataPrep -- Does more of cleaning of data|
|AWS EMR |Cloud Dataproc|Azure Databricks|
|More Like EMR |Cloud DataFlow|
|jupyter|Cloud Datalab|
|AWS Quicksight or Tableau|Cloud Data Studio|
|AWS IAM |Cloud IAM||
|AWS Cognito User Pools||Azure AD B2C|
|AWS Cognito Idenity pools||Azure AD B2B|
|IAM Roles|Service Accounts|
|AWS Organisation|||
|Cloud Trail|Cloud Audit Logging|
|Shiled and WAF|CLoud Armor|Azure DDoS Protection|
|Similar to Macie|Cloud DLP API|
|AWS GuardDuty|Event Threat Detection|
|subnets are zonal|subnets are regional|
|AWS Security Hub -- SIEM|Cloud SCC -- SIEM|
|AWS KMS|Cloud KMS|Azure Key Vault|
|AWS HSM|CloudHSM|
|Cloudwatch|StackDriver|
|AWS XRay|Stackdriver Trace|Azure Application Insights (APM)
|CloudFormation|Deployment Manager| Azure Resource Manager Templates|
|AWS Code Commit /Git|Cloud Sorce Repos|
|AWS CodeBuild|Cloud Build -- Jenkins|
|AWS ECR |Container Registery|Container Registery|
|ALB||Azure Application Gateway|
|Somehwhat like API Gateway|Cloud Endpoints||
|AWS Device Farm|Test lab for Android|
|AWS Cloud9|CloudShell (Sudo yes)| Azure Cloud Shell (No Sudo)|
|AWS Health Dashboard https://status.aws.amazon.com/|GCP Health Dashboard https://status.cloud.google.com/| Azure https://status.azure.com/en-us/status |
|AWS Personal HD| NA|
|AWS https://console.aws.amazon.com/  |GCP https://console.cloud.google.com/|Azure https://portal.azure.com/ |
|EKS|GKE|Azure Kubernetes Service (AKS)|
|Fargate |~ Cloud Run||
|Dedicated Hosts|Sole-tenant nodes|Host Group|
|EC2 Bare Metal Instances |Bare Metal Solution|
|ElasticCache |Cloud Memorystore|Azure Cache for Redis|
|Amazon DocumentDB |Cloud Firestore|
|AWS AppMesh|Traffic Director|Service Fabric Mesh |
|Dual Stack VPC | IPv4 Only VPC|Dual Stack VNET|
|Dual Stack ELB|No Dual Stack CLB (Create 2 separate LBs)|Dual Stack LBs|
|Path Based Switching|URL Maps||
|Amazon CloudWatch alarms|Cloud Monitoring they are called alerting policies||
|Cloud Watch|Cloud Monitoring|Azure Monitor (Insights and Log anlytics)|
|https://calculator.aws/|https://cloud.google.com/products/calculator/ |https://azure.microsoft.com/en-us/pricing/calculator/|
|||https://azure.microsoft.com/en-us/pricing/tco/|
|Support Plans Basic,Developer($29),Enterprise($15,000) and Business($100) |Basic, Developer, Production and Premium Support |Free,Developer($29),Standard($100), professional Direct($1000)
| | |
| | |
| | |



-----------------------------\



Questions
Azure Batch
Azure Service Fabric

