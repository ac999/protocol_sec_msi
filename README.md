# Security Protocols: Modelling and verification 2021 (teached by Lecturer, Ph.D. Cătălin Bîrjoveanu)
## Done during Master's in Information Security @ Faculty of Computer Science within Alexandru Ioan Cuza University of Iasi

Design a security protocol based on the below specifications and prove its correctness using CL-AtSe tool.
* Agents:
  * A - Client
  * B - Service Delivery Server
  * S -Authentication Server
* Objectives/Goals:
  * establishing a session key between A and B
  * mutual authentication between A and B
* Assumptions and Restrictions:
  * A has a symmetric key shared with S
  * B has a symmetric key shared with S
  * only S can generate session keys
  * do not use timestamps
  * efficiency in the messages structure and their number

The design is based on Example 2 from http://www.avispa-project.org/package/tutorial.pdf.
