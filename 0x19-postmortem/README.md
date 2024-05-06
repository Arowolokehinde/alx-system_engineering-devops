MY FIRST POSTMORTEM
Issue Summary
Duration of the outage: 2 hours, from 3:00 PM to 5:00 PM EST on April 20, 2023.
Impact: The company's e-commerce website was down, causing customers to be unable to access the site or place orders. It is estimated that approximately 70% of the user base was affected.
Root cause: A spike in traffic caused by a popular influencer promoting a new product line overwhelmed the server's resources, leading to the website crashing.

Timeline
3:15 PM- The issue was detected by the monitoring system, which triggered an alert for high CPU and memory usage on the web server.
3:20 PM - The on-call engineer investigated the issue and noticed that the website was unresponsive.
3:30 PM - The incident was escalated to the web development team, who began investigating potential causes.
3:45 PM - The team initially assumed that the issue was caused by a code deployment gone wrong and rolled back the most recent changes, but the website remained down.
4:00 PM - Further investigation revealed that the spike in traffic was causing the server to become overloaded, leading to the crash.
4:15 PM - The incident was escalated to the infrastructure team to investigate scaling options.
4:30 PM - The infrastructure team provisioned additional web servers and load balancers to handle the increased traffic.
5:00 PM - The website was back online and functioning normally.






Root Cause and Resolution
The root cause of the issue was a sudden spike in traffic that overwhelmed the server's resources. This spike was caused by a popular influencer promoting a new product line on the company's e-commerce website, resulting in a significantly higher number of visitors than usual.

The issue was resolved by provisioning additional web servers and load balancers to distribute the traffic more effectively. This allowed the website to handle the increased number of visitors without crashing due to resource exhaustion.

Corrective and Preventative Measures
Improve traffic monitoring and alerting systems to detect and respond to sudden spikes in traffic more effectively.
Implement auto-scaling mechanisms to automatically provision additional resources during periods of high traffic.
Conduct load testing and stress testing to identify potential bottlenecks and ensure the system can handle anticipated traffic spikes.
Review and optimize website performance to reduce resource consumption per visitor.
Implement caching mechanisms to reduce the load on the web servers.

Tasks
Set up monitoring alerts for sudden traffic spikes and configure appropriate thresholds.
Implement auto-scaling policies for web servers and load balancers based on CPU and memory utilization.
Conduct load testing simulating various traffic scenarios, including influencer promotions and marketing campaigns.
Optimize website performance by minimizing resource-intensive operations and implementing caching mechanisms.
Patch web servers and load balancers with the latest security updates and performance optimizations.
Review and update the incident response plan to improve communication and coordination during outages.

