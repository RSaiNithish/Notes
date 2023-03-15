
## Cloud reference model
![[Pasted image 20230315121716.png]]

![[Pasted image 20230315092105.png]]l
## Could Computing models:
 - **Software as a Service** (SaaS) 
	 - Software applications are delivered over the internet
	 - The software and associated infrastructure are managed and maintained by the SaaS provider
	 - Users pay for the service on a subscription basis.
	 - Examples: Gmail, Salesforce, and Microsoft 365.
 - **Platform as a Service** (PaaS)
	 - Cloud provider delivers a platform for developers to build and deploy applications.
	 - PaaS provider manages the infrastructure, operating system, and middleware.
	 - User is responsible for managing the application code and data.
	 - Examples: Google App Engine, Heroku, and Microsoft Azure.
	 ![[Pasted image 20230315121903.png]]
	 
 - **Infrastructure as a Service** (IaaS)
	 - Cloud provider delivers computing infrastructure, including servers, storage, and networking, as a service over the internet.
	 - User is responsible for managing the operating system, middleware, and applications
	 - IaaS provider manages the underlying infrastructure.
	 - Examples: Amazon Web Services (AWS), Microsoft Azure, and Google Cloud Platform.
![[Pasted image 20230315121926.png]]
| Feature      | SaaS          | PaaS          | IaaS          |
|--------------|---------------|---------------|---------------|
| Definition   | Software as a Service | Platform as a Service | Infrastructure as a Service |
| Main purpose | Deliver software application over the internet | Development and deployment of software applications | Provisioning of computing resources over the internet |
| Responsibility | Vendor responsible for maintenance, security, and upgrades | Vendor responsible for maintenance and security of the platform; user responsible for application deployment and upgrades | User responsible for maintenance, security, and upgrades |
| Scalability  | Limited by vendor infrastructure | Scalable within the limits of the platform | Scalable according to user needs |
| Flexibility  | Limited by vendor application | Moderate flexibility for application development | High flexibility for infrastructure customization |
| Examples     | Salesforce, Google Apps | Heroku, OpenShift | Amazon Web Services, Microsoft Azure |


## 7 steps to the cloud
### Migrating into cloud

 1. **Assess**
	  - Migration starts with an assessment of the issues relating  
	  - Proof of concepts for migration and the corresponding pricing details will help to assess these issues properly 
 2. **Isolate**
	 - Isolation of all environmental and systemic dependencies of enterprise application - 
	 - These include library, application and architectural dependencies 
	 - this results in a better understanding of the complexity of the migration 
 3. **Map**
	 - A mapping construct is generated to separate the components that should reside in data center from the ones that will go into the cloud
 4. **Re-archietect**
	 - A substantial part of the application has to be re-architected and implemented in the cloud
 5. **Augment**
	  - Features of cloud computing services are used to augment(extend) the application
 6. **Test**
	  - Application needs to be validated and tested
 7. **Optimize**
	  - Optimize based on the test results
	  - It may take several optimizing iterations for the migration to be sucessful.