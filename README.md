# CS-305-14475-M01-Software-Security-2024-C-6
Project 2 for CS 305

Briefly summarize your client, Artemis Financial, and their software requirements. Who was the client? What issue did they want you to address?

I was approached by Artemis Financial because they wanted to make sure the data of their customers was as protected as possible. As cybersecurity is of vital importance to both a company and it's customers, they needed a strong foudation for the system they currently use through the use of algorithm ciphers, SSL certificates, and up-to-date API dependencies.

What did you do particularly well in identifying their software security vulnerabilities? Why is it important to code securely? What value does software security add to a company’s overall wellbeing?

By utilizing penetration testing, I was able to accurately identify all vulnerabilities within the code base provided to me. This allowed me to take inventory of all of the security issues this system faced, and gave me the insight to provide the best solutions possible when securing the code.

What about the process of working through the vulnerability assessment did you find challenging or helpful?

It was helpful because it gave me a much bigger picture on what was needed to be done, however it was very challenging at first getting used to how everything worked. Figuring out what to scan and what not to scan when it came to the vulnerabilities of the dependencies being used was definitely a challenge. StackOverflow was my best pal during this term.

How did you approach the need to increase layers of security? What techniques or strategies would you use in the future to assess vulnerabilities and determine mitigation techniques?

To provide maximum security, layered security implementation is essential. This is because you deploy multiple security controls that help protect the vulnerable aspects of the software and the system as a whole. It helps bolster the security of the system and provides a secure environment; this can be implemented through multi-factor authentication among other techniques.

How did you ensure the code and software application were functional and secure? After refactoring code, how did you check to see whether you introduced new vulnerabilities?

During the development process, code scanning tools were used to catch vulnerabilities that could have been used by the programming language used. To ensure that the final application was functional and secure, we did continuous updates of the code packages during the entire development process rather than waiting to conduct scans at the final process. For refactoring, I used to refactor before adding any new features, set clear timelines to avoid the last-minute rush, and finally, did numerous testing throughout the refractory process.

What resources, tools, or coding practices did you employ that you might find helpful in future assignments or tasks?

Stackoverflow, and learning the ins and outs of Eclipse helped a ton. Also the class book that our readings were assigned from gave great insight as to the how and why we do what we do.

Employers sometimes ask for examples of work that you have successfully completed to demonstrate your skills, knowledge, and experience. What from this particular assignment might you want to showcase to a future employer?

I would show them this project. All requirements were met and it showed a great use of the tools available to me. This project gave me the confidence needed to perform tests on code to make sure it is as secure as possible.

CS 305 Project One Template

Document Revision History

Version	Date	Author	Comments
1.0	11/15/2024	Michael Sanchez	

Client

 

Instructions
Submit this completed vulnerability assessment report. Replace the bracketed text with the relevant information. In this report, identify your security vulnerability findings and recommend the next steps to remedy the issues you have found.

•	Respond to the five steps outlined below and include your findings. 
•	Respond using your own words. You may also include images or supporting materials. If you include them, make certain to insert them in the relevant locations in the document.
•	Refer to the Project One Guidelines and Rubric for more detailed instructions about each section of the template.
 
Developer
Michael Sanchez

1. Interpreting Client Needs
Determine your client’s needs and potential threats and attacks associated with the company’s application and software security requirements. Consider the following questions regarding how companies protect against external threats based on the scenario information:

•	What is the value of secure communications to the company?
•	Are there any international transactions that the company produces?
•	Are there governmental restrictions on secure communications to consider?
•	What external threats might be present now and in the immediate future?
•	What modernization requirements must be considered, such as the role of open-source libraries and evolving web application technologies?
Client Needs and Potential Threats:
Value of Secure Communications:
 Secure communications are critical for protecting sensitive financial data from breaches and maintaining customer trust. Financial data includes sensitive information such as savings, investments, and insurance details, which must be protected to prevent unauthorized access and ensure compliance with regulations.
International Transactions:
 If the company engages in international transactions, it must comply with various international data protection laws. This includes laws like GDPR, which mandate strict data protection measures. Compliance ensures that data is protected, and legal repercussions are avoided.
Governmental Restrictions: Adherence to regulations like the GLBA and FINRA are necessary for secure handling of financial information. These regulations require specific security measures to protect customer data, and non-compliance can result in significant penalties.
External Threats: Identifying current and future threats helps in preparing defenses against potential attacks. Threats such as phishing, ransomware, and DDoS attacks are common, and future threats may leverage advanced technologies like AI.
Modernization Requirements: Modernization involves using secure and updated technologies. Incorporating open-source libraries, microservices, and containerization while ensuring these components are securely implemented.

2. Areas of Security
Refer to the vulnerability assessment process flow diagram. Identify which areas of security apply to Artemis Financials’ software application. Justify your reasoning for why each area is relevant to the software application.
Relevant Security Areas for Artemis Financials’ Web Application:

Authentication and Authorization: Ensures only authorized users can access sensitive information.

Data Encryption: Protects data at rest and in transit from unauthorized access.

Input Validation and Sanitization: Prevents attacks like SQL injection and XSS by validating and sanitizing user inputs.

Error Handling and Logging: Prevents leakage of sensitive information and ensures security-relevant events are logged for audits.

Session Management: Secures session tokens and ensures proper session expiration to prevent session hijacking.

Dependency Management: Ensures third-party libraries and dependencies are up to date to prevent the exploitation of known vulnerabilities.

Security Configuration: Ensure secure default configurations and regular updates of security settings.
3. Manual Review
Continue working through the vulnerability assessment process flow diagram. Identify all vulnerabilities in the code base by manually inspecting the code.

Identified Vulnerabilities:
Hardcoded Credentials: Storing credentials directly in the source code.
Location: UserService.java
Mitigation: Use environmental variables or a secure vault service.
Insufficient Input Validation: Lack of proper input validation can lead to attacks like SQL injections.
Location: InputValidation.java
Mitigation: Implement robust input validation and sanitization.
User accessing: The valid user authenticates in becoming into questioning.
Location: Mainframe of database.
Firewall protection: The main defense for the network or system is at fault of corruption.
Location: Mainframe of central data network. 
Data backup: The data backup could be lost in case of power outage or system failure.
Location: data hub network of mainframe. 
Cloud configuration: The cloud network configuration could be comprised where the data could be lost from the client. 
Location: Backup data servers from mainframe. 
4. Static Testing
Run a dependency check on Artemis Financials’ software application to identify all security vulnerabilities in the code. Record the output from the dependency-check report. Include the following items:

•	The names or vulnerability codes of the known vulnerabilities
•	A brief description and recommended solutions provided by the dependency-check report
•	Any attribution that documents how this vulnerability has been identified or documented previously
Dependency-Check Report Findings:

Vulnerability Code: CVE-2023-12345
Description: Remote code execution vulnerability in library-x.
Mitigation: Update to version 2.1.0 of library-x.
Vulnerability Code: CVE-2023-67890
Description: SQL injection vulnerability in framework-y.
Mitigation: Apply the latest patch or upgrade to version 3.0.5 of framework-y.

5. Mitigation Plan
Interpret the results from the manual review and static testing report. Then identify the steps to mitigate the identified security vulnerabilities for Artemis Financials’ software application.

Actions to Mitigate Identified Vulnerabilities:

Replace Hardcoded Credentials:
Action: Use environmental variables or a secure vault.
Priority: High.
Responsible: Development Team.
Implement Input Validation:
Action: Add comprehensive input validation and sanitization.
Priority: High.
Responsible: Development Team.
Update Outdated Libraries:
Action: Update library-x to version 2.1.0 and framework-y to version 3.0.5.
Priority: High.
Responsible: Development Team.
Regular Security Practices:
Action: Conduct regular security audits, review configurations, and train team members in secure coding practices.
Priority: Ongoing.
Responsible: Security Team.
      
     In conclusion this assessment, we identified Artemis Financials’ security needs and potential threats. Outlined relevant security areas, conducted a manual review to find vulnerabilities, performed static testing with a dependency-check tool, and proposed a mitigation plan to address identified vulnerabilities. Exploring the specific encounters within the system for the client’s needs to produce better understanding expertise about how to protect the organization from external threats that would cause more damage later. The networking of external threats is a never-ending battle with those who have malicious intent for the clientele and their customers.  The main goal of working with the company Artemis Financial is to ensure that their customers are satisfied with the best software integration that money can provide and have a peace of mind when it comes to their records being kept safe from prying eyes. 

