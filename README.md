# AI-Threat-Modeling-Agricultural-System-PEAT

## Objective


Conduct a threat modeling assessment of an AI-powered crop monitoring system to identify potential security, integrity, and privacy risks. The project evaluates how AI models handling crop and soil data could be impacted by attacks such as data poisoning, adversarial inputs, model theft, and denial of service, and recommends mitigations to enhance system resilience and secure sensitive agricultural data.

### Skills Learned


- Analyzing AI system workflows and identifying potential risks
- Understanding AI-specific threats like data poisoning and adversarial inputs
- Mapping threats to MITRE ATT&CK-style techniques
- Designing mitigation strategies for cloud and AI systems
- Risk assessment and documentation for non-technical audiences
- Applying structured threat modeling frameworks (STRIDE / ATT&CK concepts)

### Tools Used


- AI Crop Monitoring Systems (PEAT) – Studied AI-powered plant disease detection systems to understand potential security risks and threat vectors.
- Diagramming / Documentation Tools – For creating visual threat models and reporting findings in Draw io.

## System Overview:

An AI-powered agricultural system that allows users to upload images of crops or plant leaves, which are analyzed using machine learning–based computer vision models to identify signs of disease, pest damage, or nutrient deficiencies. The system then provides diagnostic insights and recommended treatment actions to support early intervention and improve crop health and yield.

## Assets at Risk

- AI training data

- AI model

- User-submitted images

- Cloud infrastructure

## Threat Actors

# 1. Malicious Users
  
 Who they are:
- Individuals intentionally submitting fake or manipulated images or abusing the system.
    
# Motives: 

- Disrupt system accuracy

- Cause incorrect diagnoses

- Undermine trust in the AI

# Threats:
- Data Poisoning
- Adversarial inputs

# 2. Competitors
  
 Who they are:
- Rival companies seeking insight into proprietary AI models or training data.
    
# Motives: 

- Steal intellectual property

- Reverse-engineer AI capabilities

- Gain market advantage

# Threats:

- Model extraction

- Data scraping


# 3. Cybercriminals
  
 Who they are:
- Attackers seeking financial gain or access to valuable data.
    
# Motives: 

- Monetize stolen data

- Abuse cloud resources

- Sell access or insights

# Threats:

- Unauthorized access

- Data exfiltration

- Denial of service


# 4. Automated Bots
  
 Who they are:
- Scripts or automated systems probing APIs or flooding services.
    
# Motives: 

- Exploit vulnerabilities at scale

- Disrupt service availability

# Threats:

- Denial of service

- Credential stuffing

- API abuse


# 5. Insider Threats (Low Likelihood, High Impact)
  
 Who they are:
- Employees or contractors with legitimate access.
    
# Motives: 

- Negligence

- Intellectual property theft

# Threats:

- Data leakage

- Model tampering


# 6. Hacktivists or Saboteurs (Less Common)
  
 Who they are:
- Individuals targeting agricultural technology for ideological or political reasons.
    
# Motives: 

- Disrupt food supply systems

- Damage organizational reputation

# Threats:

- Service disruption

- Data manipulation

# Threat-Actor Summary:
Threat actors targeting AI-powered agricultural systems may include malicious users, competitors, cybercriminals, automated bots, and insiders, each motivated by disruption, financial gain, or intellectual property theft.

# Treat Scenarios and Mitigations:
  
| Threat Scenario                       | Actor          | Impact                              | Mitigation                                |
| ------------------------------------- | -------------- | ----------------------------------- | ----------------------------------------- |
| Submission of manipulated crop images | Malicious user | Incorrect disease diagnosis         | Input validation and confidence scoring   |
| Reverse engineering the AI model      | Competitor     | Intellectual property theft         | Rate limiting and monitoring              |
| API abuse or credential misuse        | Cybercriminal  | Data exposure or service disruption | Strong authentication and access controls |
| Flooding image uploads                | Automated bots | Denial of service                   | Rate limiting and traffic monitoring      |


# Risk Assessment:

High-Risk:
- Data poisoning and manipulated inputs, as they can directly impact the accuracy and reliability of AI-generated diagnoses.

- Unauthorized access to AI services or data, due to the potential for data exposure, service abuse, and loss of trust.

 Acceptable or Lower Risk:

- Model extraction attempts, which are less likely when rate limiting and monitoring are in place.

- Denial-of-service attacks, as their impact can be reduced through traffic controls and scalable infrastructure.

# In Conclusion:

- AI systems introduce unique security risks beyond traditional applications, particularly around data integrity and model abuse.

- Effective threat modeling can be performed without hands-on exploitation by using structured analysis and risk assessment.

- Mapping AI-related threats to frameworks such as MITRE ATT&CK helps prioritize risks and guide mitigation strategies.

- Clear documentation is critical for communicating security risks to non-technical stakeholders.
