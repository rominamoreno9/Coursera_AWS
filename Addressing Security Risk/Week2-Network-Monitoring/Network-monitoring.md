## **Network Isolation**
## Amazon VPC
Amazon Virtual Private Cloud (Amazon VPC) lets you provision a logically isolated section of the AWS Cloud where you can launch AWS resources in a virtual network that you define. You have complete control over your virtual networking environment, including selection of your own IP address range, creation of subnets, and configuration of route tables and network gateways. You can use both IPv4 and IPv6 in your VPC for secure and easy access to resources and applications.  More information is available at: https://aws.amazon.com/vpc/ 

## Route Tables
A route table contains a set of rules, called routes, that are used to determine where network traffic is directed.

Each subnet in your VPC must be associated with a route table; the table controls the routing for the subnet. A subnet can only be associated with one route table at a time, but you can associate multiple subnets with the same route table.

## AWS Direct Connect
AWS Direct Connect is a cloud service solution that makes it easy to establish a dedicated network connection from your premises to AWS. Using AWS Direct Connect, you can establish private connectivity between AWS and your datacenter, office, or colocation environment, which in many cases can reduce your network costs, increase bandwidth throughput, and provide a more consistent network experience than Internet-based connections.

AWS Direct Connect lets you establish a dedicated network connection between your network and one of the AWS Direct Connect locations. Using industry standard 802.1q VLANs, this dedicated connection can be partitioned into multiple virtual interfaces. This allows you to use the same connection to access public resources such as objects stored in Amazon S3 using public IP address space, and private resources such as Amazon EC2 instances running within an Amazon Virtual Private Cloud (VPC) using private IP space, while maintaining network separation between the public and private environments. Virtual interfaces can be reconfigured at any time to meet your changing needs.  More information including pricing for AWS Direct Connect is available at: https://aws.amazon.com/directconnect/ .


## **Monitoring**

**Amazon GuardDuty**

Amazon GuardDuty is a threat detection service that continuously monitors for malicious activity and unauthorized behavior to protect your AWS accounts and workloads. With the cloud, the collection and aggregation of account and network activities is simplified, but it can be time consuming for security teams to continuously analyze event log data for potential threats. With GuardDuty, you now have an intelligent and cost-effective option for continuous threat detection in the AWS Cloud. The service uses machine learning, anomaly detection, and integrated threat intelligence to identify and prioritize potential threats. GuardDuty analyzes tens of billions of events across multiple AWS data sources, such as AWS CloudTrail, Amazon VPC Flow Logs, and DNS logs. With a few clicks in the AWS Management Console, GuardDuty can be enabled with no software or hardware to deploy or maintain. By integrating with AWS CloudWatch Events, GuardDuty alerts are actionable, easy to aggregate across multiple accounts, and straightforward to push into existing event management and workflow systems.  More information about Amazon GuardDuty can be found at: https://aws.amazon.com/guardduty/ 


**AWS Security Hub**

AWS Security Hub gives you a comprehensive view of your high-priority security alerts and compliance status across AWS accounts. With Security Hub, you have a single place that aggregates, organizes, and prioritizes your security alerts, or findings, from multiple AWS services, such as Amazon GuardDuty, Amazon Inspector, and Amazon Macie, as well as from AWS Partner solutions. Your findings are visually summarized on integrated dashboards with actionable graphs and tables. You can also continuously monitor your environment using automated compliance checks based on the AWS best practices and industry standards your organization follows.   More information about AWS Security Hub can be found at: https://aws.amazon.com/security-hub/ 


**AWS CloudTrail**

AWS CloudTrail es un servicio que le permite realizar auditorías de gobernanza, de conformidad, operativas y de riesgo en su cuenta de AWS. Con CloudTrail, puede registrar, monitorear de manera continua y retener la actividad de la cuenta relacionada con acciones en toda su infraestructura de AWS. CloudTrail proporciona el historial de los eventos de actividad de su cuenta de AWS, incluidas las acciones efectuadas a través de la consola de administración de AWS, los SDK de AWS, las herramientas de línea de comandos y otros servicios de AWS. El historial de eventos simplifica el análisis de seguridad, el seguimiento de cambios de recursos y la resolución de problemas. Además, puede usar CloudTrail para detectar actividad inusual en sus cuentas de AWS. Estas funciones ayudan a simplificar los análisis operativos y la solución de problemas.

**Amazon CloudWatch**

Amazon CloudWatch es un servicio de monitorización y observación creado para ingenieros de DevOps, desarrolladores, ingenieros de fiabilidad de sitio (SRE) y administradores de TI. CloudWatch ofrece datos e información procesable para monitorizar sus aplicaciones, responder a cambios de rendimiento que afectan a todo el sistema, optimizar el uso de recursos y lograr una vista unificada del estado de las operaciones. CloudWatch recopila datos de monitorización y operaciones en formato de registros, métricas y eventos, lo cual ofrece una vista unificada de los recursos, las aplicaciones y los servicios de AWS que se ejecutan en servidores locales y de AWS. Puede usar CloudWatch para detectar comportamientos anómalos en sus entornos, definir alarmas, comparar registros y métricas, realizar acciones automatizadas, resolver problemas y descubrir información para mantener sus aplicaciones
en ejecución sin problemas.

**AWS Config**

AWS Config es un servicio que permite examinar, auditar y evaluar las configuraciones de sus recursos de AWS. Config monitorea y registra constantemente las configuraciones de sus recursos de AWS y le permite automatizar la evaluación de las configuraciones registradas con respecto a las configuraciones deseadas. Con Config, puede revisar los cambios en las configuraciones y las relaciones entre los recursos de AWS, profundizar en los historiales detallados de configuración de recursos y determinar la conformidad general con respecto a las configuraciones especificadas en sus pautas internas. Esto le permite simplificar las auditorías de conformidad, los análisis de seguridad, la administración de cambios y la resolución de problemas operativos.


**AWS Well-Architected and the Five Pillars (Architecture)**

[Link](https://aws.amazon.com/architecture/well-architected/?nc1=h_ls&wa-lens-whitepapers.sort-by=item.additionalFields.sortDate&wa-lens-whitepapers.sort-order=desc)


**Amazon Inspector**

Amazon Inspector is an automated security assessment service that helps improve the security and compliance of applications deployed on AWS. Amazon Inspector automatically assesses applications for exposure, vulnerabilities, and deviations from best practices. After performing an assessment, Amazon Inspector produces a detailed list of security findings prioritized by level of severity. These findings can be reviewed directly or as part of detailed assessment reports which are available via the Amazon Inspector console or API.

Amazon Inspector security assessments help you check for unintended network accessibility of your Amazon EC2 instances and for vulnerabilities on those EC2 instances. Amazon Inspector assessments are offered to you as pre-defined rules packages mapped to common security best practices and vulnerability definitions. Examples of built-in rules include checking for access to your EC2 instances from the internet, remote root login being enabled, or vulnerable software versions installed. These rules are regularly updated by AWS security researchers.

[Amazon Inspector](https://aws.amazon.com/inspector/)