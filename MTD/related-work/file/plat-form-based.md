## Dynamic PlatForm Techqniues

 Dynamic platform techniques (DPT) change platform properties to stop attacking process. Tempoeral changes (e.g., virtual machine rotation) and diversity (e.g., multiple variants execution) are widely used as DPT techniques for system protection. DPT techqniues, which have been discussed above, so we focus on machine-level/OS-level DPT techniques, which cincludes migration-based techniques, server-swithcing techniques, and self-cleaning techniques.
- Migration-based techniques, such as Talent, leverge OS-level virtualization to createa a virtual execution environment for migrating a running application across different platforms and preserving the state of the appication. DPT could also be achieved by switching between different implementations of servers. 

- Saidane et al. propse the deployment of redundant servers with diverse software (e.g., Apatche and IIS) in a web system. Redundancy improves system availability, and diversificaiton increase the difficulty of vulnerability explitation. 
 
- Self-cleaning techniques change current platform instance without diverfication, such as reimaging the OS. SCIT achieves self-cleansing by decommissing a server that has been exposed to the Internet for a predetermined period of time, and launching a pristine copy of the server.

- Ideas of DPT are also used in works on aseessing software reliability. For instance, Zhang and Liu designed and deployed diver-serivers based replicas of virutal machines (Heter-device), to compare run-time behavior of drivers from different vendors. Replcias in a Heter-device load heterogeneous drivers for identical virutal devices. 
  - The behavior of these derivers are compared to capture inconsistencies as evidence of un-trustworthiness.
