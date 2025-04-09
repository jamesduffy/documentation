# Tabletop Scenarios

## Guide

This guide will help you set up and run tabletop exercises. Tabletop exercises should simulate real-world incidents, allowing your team to practice response strategies, communication, and decision-making skills.

### How to Run a Tabletop Exercise

1. **Assign a Scenario Leader**
    - The Scenario Leader will guide the exercise and provide new information as the team works through the scenario.
    - The Scenario Leader's role is to find gaps in the incident response process (IRP) and help the team learn to work together.

2. **Assign Roles**
    - **Incident Commander**: Leads the response, makes decisions, and coordinates the team's actions.
    - **Technical Lead(s)**: Handles technical troubleshooting and mitigation.
    - **Communication Lead**: Manages internal and external communication.

3. **Start the Scenario**
    - The team begins the scenario without any prior information about the incident. The Scenario Leader will provide an initial briefing to set the context.
    - The Incident Commander must lead the team in investigating and resolving the scenario using existing procedures.

4. **Introduce New Information**
    - The Scenario Leader introduces new information (injects) throughout the exercise to keep it progressing and add complexity.
    - Example Injects:
      - “The cloud provider’s support team is unresponsive.”
      - “A new log entry shows that the issue may be related to a recent deployment.”

5. **Conclude the Exercise**
    - Once the scenario is resolved, or the exercise time is up, the Scenario Leader concludes the exercise.
    - The team should discuss what went well, what was challenging, and what they would do differently next time.

6. **Document Findings**
    - Summarize the exercise, including observations and recommended action items.
    - Share the findings with the team to improve future responses.

### Tips for a Successful Tabletop Exercise

- **Keep It Simple**: Start with basic scenarios and progress to more complex ones as your team gains confidence.
- **Encourage Participation**: Make sure everyone has a chance to contribute.
- **Be Realistic**: Use scenarios that reflect your team's actual systems and services.
- **Focus on Learning**: The goal is to learn and improve, not to assign blame.
- **Practice Regularly**: Run tabletop exercises regularly to build team confidence and response skills.

## Example Scenarios

1. **Database is Unavailable**
   Your primary database is unreachable, causing outages for multiple services. Backup restoration is delayed due to an ongoing migration process.

2. **Kubernetes Cluster Nodes Are Unavailable**
   A majority of your Kubernetes cluster nodes have become unavailable due to an unknown issue, affecting the deployment and scaling of critical applications.

3. **Istio Service Mesh Is Not Routing Traffic**
   Your Istio service mesh is not routing traffic properly between microservices, causing timeouts and failures across all environments.

4. **Application Is Leaking PII Through Front-End Code**
   Sensitive information such as email addresses and partial credit card numbers are being exposed to users through an unexpected front-end bug.

5. **Zero-Day Vulnerability in a Core Dependency**
   A zero-day vulnerability is announced for a core dependency you use across multiple services. Patching will take at least 48 hours, and the exploit is publicly available.

6. **Certificate Expiry Brings Down API**
   An expired SSL certificate brings down your primary production API. All automated renewal attempts have failed, and the original configuration is undocumented.

7. **Administrator Account to Cloud Email Is Inaccessible**
   The administrator account for your cloud email service is no longer accessible. The recovery email belongs to a former employee using a custom domain that’s no longer active.

8. **Unplanned Financial Charges**
   A notification of unusually high spending on your cloud provider reveals that a resource-intensive test environment has been running for weeks at full capacity.

9. **Law Enforcement Contacts You About a Breach**
   Law enforcement notifies you of a breach, providing details about your database table structure. No official incident has been declared, and it’s unclear how they obtained the information.

10. **DNS A Records Are Being Modified Without Authorization**
    DNS A records for your main domain are being modified without any known change requests. Logs indicate these changes originated from your DNS provider’s API.

11. **Supply Chain Attack via CI/CD Pipeline**
    An external contributor to a critical open-source dependency has pushed a malicious update. After pulling the latest version, your build process starts connecting to unknown external IP addresses.

12. **Recovery Keys Are Inaccessible Due to an Ongoing Outage**
    Recovery keys necessary to restore services during an outage are themselves inaccessible because of the same outage.

13. **Rogue IoT Device on the Network**
    An unregistered IoT device is discovered on your internal network, communicating with external IP addresses using a legitimate certificate unique to your approved devices.

14. **Shadow IT Discovery**
    An audit reveals a shadow infrastructure environment running under an employee's personal cloud account. The environment has access to sensitive databases via a shared service account.

15. **Untrusted Code Accidentally Merged and Deployed**
    A feature branch containing untrusted and unverified code has been merged into your main branch. It’s deployed to production, and you only find out after customers report issues.

16. **Management Control Plane Is Down During an Outage**
    The management control plane you normally use to respond to outages is also down due to the outage, preventing your team from accessing critical tools.

17. **Customer Configuration Causes Widespread Errors**
    A specific customer makes a valid configuration change, causing 85% of your production systems to report errors.

18. **Disgruntled Maintainer Bricks Their Dependency**
    The maintainer of a dependency you rely on has purposefully introduced a breaking change, disrupting all systems dependent on that library.

19. **Data Warehouse Schema Changed Without Authorization**
    Your analytics team notices discrepancies in reports. It’s revealed that schema changes were made from a compromised employee account.

20. **SSO Service Has Announced a Breach**
    Your SSO service provider has declared a breach, and all connected applications are at risk. The incident response team is unable to confirm which accounts have been affected.

21. **Primary Domain Suspended by Registrar**
    Your domain registrar has suspended your primary domain. Basic support inquiries are not being answered, and critical services are impacted.

22. **Senior Developer Leaves Abruptly, Taking Knowledge With Them**
    Your most senior developer, responsible for the CI/CD pipeline, leaves unexpectedly, taking crucial undocumented knowledge and scripts with them.

23. **Adversary Has Read All Values on Secrets Management Platform**
    It’s discovered that an adversary has read all values on your secrets management platform. The team needs to rotate secrets for all services in a short period of time.

For more inspiration, check out [@badthingsdaily](https://x.com/badthingsdaily).
