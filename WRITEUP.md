# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.


- I choose App Service due to the lightweight size of the App Lightweight APIs tend to be well-suited to App Services over VMs (see cost analysis below), and won't approach the size limit for App Services very easily. Additionally, App Services cost less than VMs do. Lastly, since the ability to scale quickly is less of a concern, we don't need to factor that into the analysis.*
- Cost Comparison: Azure App Services vs. Azure Virtual Machines
![image](https://github.com/user-attachments/assets/3f3282e5-b179-41b4-8a40-1fbf089693ae)

Explanation of Cost Differences
Azure App Service: This is a fully managed platform-as-a-service (PaaS) that is optimized for web and API applications. It offers various pricing tiers, from Free to Isolated, each providing different levels of performance, scalability, and features. The cost increases with higher tiers due to additional resources and capabilities provided.

Azure Virtual Machines: VMs offer more control and flexibility compared to App Services. They are infrastructure-as-a-service (IaaS) and come in various sizes and configurations to suit different workloads. The cost of VMs varies based on the type of VM, its size, and the region in which it is deployed. Burstable VMs are the cheapest, while high-performance VMs like M32ls are more expensive due to their advanced capabilities.

Scenarios
![image](https://github.com/user-attachments/assets/51244f80-514f-4835-9eec-2534e46b738a)


![image](https://github.com/user-attachments/assets/8d4166b3-3d7b-4c6a-b36f-d124dcde9aa3)
Explanation of Scalability and Availability Differences
Azure App Service: This service offers both vertical scaling (scale up) and horizontal scaling (scale out). You can increase the resources allocated to your app by changing the pricing tier or increase the number of instances running your app. Autoscaling allows you to automatically adjust the number of instances based on demand. For availability, Azure App Service supports deployment across multiple availability zones and regions, ensuring high availability and disaster recovery12.

Azure Virtual Machines: VMs provide flexible scaling options through VM scale sets, which allow you to automatically adjust the number of VM instances based on demand. You can choose from a wide range of VM sizes and types to match your workload requirements. For availability, VMs can be grouped into availability sets to ensure that at least one VM is available during maintenance or hardware failures. Additionally, VMs can be distributed across multiple availability zones within a region and deployed in multiple regions for disaster recovery345.

Scenarios
![image](https://github.com/user-attachments/assets/1de7fc5b-999f-4a6c-a320-4ad4b03942a9)

### Assess app changes that would change your decision.

* I would have done a VM if this was a high traffic or high security application- which  a vast increase in the number of users and the need for dedicated servers for security reasons.  Handling the vast increase in the number of users, with separate, dedicated servers, is going to be better achieved this way*  Multi-Region Deployments: Deploy VMs in multiple regions for disaster recovery and high availability would be best for a high traffic high security application. The cost and scalablity is shwown below
* ![image](https://github.com/user-attachments/assets/e2f7966b-7c15-4bbf-8805-43a8cfb07a9a)
* ![image](https://github.com/user-attachments/assets/6e1d09e1-c817-4c0c-b192-1a44eeb5d009)


