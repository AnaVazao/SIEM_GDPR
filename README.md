# GDPR-compliant open-source SIEM

This work aims to implement the open-source SIEM prototype and create a tool for analyzing and detecting threats in real-time that, at the same time, want to guarantee a performance according to GDPR compliance.

The following image is the result of documental research and the implementation of some practical scenarios, it intends to contribute to a SIEM solution where it is possible to pseudonymize the logs without losing the ability to identify threats and attacks.

![fig4b](https://user-images.githubusercontent.com/130701154/231868018-65ff943b-f0c7-423b-b749-2c200cb0ebb0.png)

# Table -  List of fields to pseudonymize
Depending on the beat type, personal data maps to distinct fields. The table illustrates the SIEM fields that may contain personal data.

![imag1](https://user-images.githubusercontent.com/130701154/232053760-ce632691-ff27-4b3b-a7fb-a9d33e354b3e.JPG)


# Algorithm  - Log pseudonymization
Through a test environment for Windows and Linux operating systems, a survey was carried out of the fields to pseudonymize for each Beat, which allowed the creation of the algorithm illustrated in the following image.

![Capturar_1](https://user-images.githubusercontent.com/130701154/231874963-05969c78-5cf9-48b0-b66d-2b4b1dc67cca.PNG)

The following link illustrates the algorithm in the server Logstash configuration file for the pipeline:

* https://github.com/AnaVazao/SIEM_GDPR/blob/main/prototype/Server_Logstash/beats.conf


The following link illustrates the algorithm in the server Logstash configuration file for the pipeline in scenario Metrics:

* https://github.com/AnaVazao/SIEM_GDPR/blob/main/Pipeline_Metricas/beats_VF.conf


# Video
Video illustrating an attack executed on a machine,  the situation anomalous it is identifying, and it's possible to look for the key to identifying the anonymized data. 


https://user-images.githubusercontent.com/130701154/232077023-f736cac3-3978-41e1-ac3e-21451cba904e.mp4

   
#
# To cite this work, please use:

Ana Paula Vazão, Leonel Santos, Rogério Luís de C. Costa, Carlos Rabadão. 2023. Implementing and evaluating a GDPR-compliant open-source SIEM solution. To appear.
