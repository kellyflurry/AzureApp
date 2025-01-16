# Write-up Template

### Analyze, choose, and justify the appropriate resource option for deploying the app.

*For **both** a VM or App Service solution for the CMS app:*
- *Analyze costs, scalability, availability, and workflow*
- *Choose the appropriate solution (VM or App Service) for deploying the app*
- *Justify your choice
- I choose App Service due to the lightweight size of the App Lightweight APIs tend to be well-suited to App Services over VMs, and won't approach the size limit for App Services very easily. Additionally, App Services cost less than VMs do. Lastly, since the ability to scale quickly is less of a concern, we don't need to factor that into the analysis.*

### Assess app changes that would change your decision.

* I would have done a VM if a vast increase in the number of users and the need for dedicated servers for security reasons. Handling the vast increase in the number of users, with separate, dedicated servers, is going to be better achieved this way* 
