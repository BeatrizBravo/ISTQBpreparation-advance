#### **Content:**
<a id="x"></a>

* [Introduction](#2)
* [Risk Identification](#3)
* [Risk Assessment](#4)
* [Risk Mitigation](#5)
* [Prioritizing the Tests](#6)
<br>

<a id="2"></a>

# Introduction
Test Managers often have overall **responsibility** for establishing and managing a risk-based test strategy. They will usually request the involvement of a Test Analyst to ensure the risk-based approach is implemented correctly.<br>

**Test Analysts should be actively involved in the following risk-based testing tasks:**
* Risk identification 
* Risk assessment / prioritization
* Risk mitigation
* 
<br>

These tasks are performed iteratively throughout the SDLC to deal with emerging risks, changing priorities and to regularly evaluate and communicate risk status. In Agile software development, the three tasks are often combined in a so-called risk session with focus on either an iteration or a release.<br>

Test Analysts should work within the riskbased test framework established for the project by the Test Manager. They should contribute their knowledge of the business domain risks that are inherent in the project such as risks related to safety, business and economic concerns, and political factors, among others.
<br>


[Back to content](#x)

---

<br>

<a id="3"></a>

# Risk Identification
By calling on the broadest possible sample of stakeholders, the risk identification process is most likely to detect the largest possible number of significant risks.
Test Analysts often possess unique knowledge regarding the particular business domain of the system under test. This means they are particularly well suited to the following tasks:
* Conducting expert interviews with the domain experts and users Conducting independent assessments 
* Using risk templates
* Participating in risk workshops
* Participating in brainstorming sessions with potential and current users 
* Defining testing checklists
* Calling on past experience with similar systems or projects
<br>

In particular, Test Analysts should work closely with the users and other domain experts (e.g., requirement engineers, business analysts) to determine the areas of business risk that should be addressed during testing. <br>

In Agile software development, this close relationship with stakeholders enables risk identification to be conducted on a regular basis, such as during iteration planning meetings.

Sample risks that might be identified in a project include:
* Issues with functional correctness, e.g., incorrect calculations 
* Usability issues, e.g., insufficient keyboard shortcuts
* Portability issues, e.g., inability to install an application on particular platforms
<br>

[Back to content](#x)

---

<br>

<a id="4"></a>

# Risk Assessment 
While risk identification is about identifying as many pertinent risks as possible, risk assessment is the study of these identified risks. Specifically, categorizing each risk and determining its risk level.<br>

Determining the risk level typically involves assessing, for each risk item, the risk **_likelihood_** and the risk **_impact_**. The risk likelihood is usually interpreted as the likelihood that the potential problem can exist in the system under test and will be observed when the system is in production. Technical Test Analysts should contribute to finding and understanding the potential likelihood for each risk item whereas Test Analysts contribute to understanding the potential business impact of the problem should it occur (in Agile software development this role-based distinction may be less strong).<br>

The risk impact is often interpreted as the severity of the effect on the users, customers, or other stakeholders. In other words, it arises from business risk. Test Analysts should contribute to identifying and assessing the potential business domain or user impact for each risk item. <br>


Factors influencing business risk include the following:
* Frequency of use of the affected feature
* Business loss Financial damage
* Ecological or social losses or liability 
* Civil or criminal legal sanctions 
* Safety concerns Fines, loss of license
* Lack of reasonable workarounds if people cannot work any more 
* Visibility of the feature
* Visibility of failure leading to negative publicity and potential image damage 
* Loss of customers

Given the available risk information, Test Analysts need to **establish the levels of business risk** according to the guidelines provided by a Test Manager. These could be classified using an ordinal scale (actual numeric or low/medium/high), or traffic signal colors. Once the risk **likelihood** and risk impact have been assigned, Test Managers use these values to determine the risk level for each risk item. That risk level is then used to prioritize the risk mitigation activities.

| **Priority Level** | **Description**   |
|---------------------|-------------------|
| **1**               | Must have         |
| **2**               | Should have       |
| **3**               | Could have        |
| **4**               | Would have        |



<br>

[Back to content](#x)

---

<br>

<a id="5"></a>

# Risk Mitigation
During the project, Test Analysts should seek to do the following:
* **Reduce** product risk by designing effective test cases that demonstrate unambiguously whether tests pass or fail, and by **participating** in **reviews** of software work products such as requirements, designs, and user documentation
* **Implement** appropriate risk mitigation activities identified in the test **strategy** and **test plan** (e.g., test a particularly high risk business process using particular test techniques)
* **Re-evaluate** known **risks** based on additional information gathered as the project unfolds, adjusting risk likelihood, risk impact, or both, as appropriate Identify new risks from information obtained during testing.

When one is talking about a product risk, then testing makes an essential contribution to mitigating such risks.
**By finding defects,** testers reduce risk by providing awareness of the defects and opportunities to deal with the defects before release. 
If the testers **find no defects,** testing then reduces risk by providing **evidence that**, under certain conditions (i.e., the conditions tested), the system operates correctly. 
Test Analysts help to determine risk mitigation options by investigating opportunities for gathering accurate test data, creating and testing realistic user scenarios and conducting or overseeing usability studies, among others.
<br>

[Back to content](#x)

---

<br>

<a id="6"></a>

# Prioritizing the Tests
The **level of risk is also used to prioritize tests.** A Test Analyst might determine that there is a high risk in the area of transactional accuracy in an accounting system. As a result, to mitigate the risk, the tester may work with other business domain experts to gather a strong set of sample data that can be processed and verified for accuracy. Similarly, a Test Analyst might determine that usability issues are a significant risk for a new test object. Rather than wait for a user acceptance test to discover any issues, the Test Analyst might prioritize an early usability test based on a prototype to help identify and resolve usability design problems early before the user acceptance test. This prioritization must be considered as early as possible in the planning stages so that the schedule can accommodate the necessary testing at the necessary time.<br>

In some cases, all of the **highest risk tests are run** before any lower-risk tests, and tests are run in strict risk order (called “**depth-first**”); 
in other cases, a sampling approach is used to **select a sample** of tests across all the **identified risk areas** using risk level **to weight** the selection while at the same time ensuring coverage of every risk at least once (called “**breadth-first**”). 
Whether risk-based testing proceeds depth-first or breadth-first, it is possible that the **time allocated** for testing might be consumed without all tests being run. 
Risk-based testing allows testers to **report to management in terms of the remaining level of risk at this point**, and allows management to decide whether to extend testing or to transfer the remaining risk onto the users, customers, help desk/technical support, and/or operational staff.<br>


<br>

[Back to content](#x)
<br>

<a id="6"></a>

# ADJUSTING TESTING FOR FUTURE TEST CYCLES

Risk assessment is **not** a one-time activity **performed before the start of test implementation**; it is a continuous process. 
Each future planned test cycle should be subjected to new risk analysis to take into account such factors as:

* Any new or significantly changed product risks 
* Unstable or failure-prone areas discovered during the testing 
* Risks from fixed defects 
* Typical defects found during testing Under-tested areas (low requirements coverage)
<br>

[Back to content](#x)
<br>

<a id="6"></a>

# Questions to review

- Test Analysts often have overall responsibility for establishing and managing a risk-based test strategy. They will usually request the involvement of a Test Manager  to ensure the risk-based approach is implemented correctly. = false. El Test Manager es el encargado de asegurar que el enfoque basado en riesgos se implemente correctamente. Sin embargo, los Test Analysts juegan un papel crucial al identificar y evaluar los riesgos, pero no tienen la responsabilidad primaria de gestionar la estrategia de pruebas basada en riesgos.
<br>
**Test Manager**: Responsable de establecer y gestionar la estrategia de pruebas basada en riesgos.<br>
**Test Analyst**: Responsable de identificar y evaluar los riesgos, pero no de gestionar la estrategia general.

- Test Analysts should be actively involved in the following risk-based testing tasks: <br>
Risk identification, Risk assessment & Risk mitigation. <br>
These tasks are performed **only** **once** throughout the SDLC to deal with emerging risks, changing priorities and to regularly evaluate and communicate risk status.<br>
= False. En la gestión de riesgos las actividades _se repiten_ a lo largo de todo el ciclo de vida, lo que refleja cómo un enfoque iterativo mejora la adaptación y el control de los riesgos. Esta comprensión clave del proceso dinámico fortalece tu habilidad para aplicar estrategias de pruebas basadas en riesgos efectivamente.

- In Agile software development, the three Risk-Based tasks are often combined in a so-called risk session with focus on either an iteration or a release. = true.  En Agile las tareas de gestión de riesgos se integran en sesiones colaborativas centradas en iteraciones o entregas, facilitando una evaluación rápida y continua que mejora la respuesta ante los riesgos. Esta práctica refleja cómo Agile promueve la adaptación constante, un concepto clave para manejar riesgos eficazmente.
- Test analyst is often involved in project risks more than product risks. =  False. El analista de pruebas se enfoca principalmente en los riesgos relacionados con el producto y su calidad, lo cual es clave para diseñar pruebas efectivas que detecten fallos antes de la entrega. Este entendimiento mejora tu capacidad para abordar riesgos específicos del producto de manera adecuada.
- By calling on the broadest possible sample of stakeholders, the risk assessment process is most likely to detect the largest possible number of significant risks. - false. Involucrar a demasiados interesados puede dispersar el enfoque y dificultar identificar los riesgos más significativos, lo que muestra una comprensión clave sobre cómo optimizar el proceso de evaluación de riesgos.
- Test Analysts often possess unique knowledge regarding the particular business domain of the system under test. This means they are particularly well suited to the following tasks:
a- Conducting expert interviews with the domain experts and users.<br>
b- Using risk templates.<br>
c- Calling on past experience with similar systems or projects.<br>
d- All of the Above.<br> [x]

-   It is the study of the identified risks. Specifically, categorizing each risk and determining its risk level. = Risk Assessment = While risk identification is about identifying as many pertinent risks as possible, risk assessment is the study of these identified risks. Specifically, categorizing each risk and determining its risk level.
- Risk Assessment involves: the risk likelihood and risk impact.  lo que permite priorizar y gestionar los riesgos de manera efectiva.
- The risk likelihood is usually interpreted as the likelihood that the potential problem can exist in the system _after_ is has been released. = False. The risk likelihood is usually interpreted as the likelihood that the potential problem can exist in _the system under test_ and will be observed when the system is in _production_.
- The risk impact is often interpreted as the severity of the effect on the users, customers, or other stakeholders. = true =  el impacto del riesgo refleja cuánto puede **afectar** **negativamente** a los usuarios o interesados, lo cual es fundamental para priorizar acciones y gestionar riesgos eficazmente.
- Once the risk likelihood and risk impact **have been assigned**, Test Analysts use these values to determine the risk level for each risk item. That risk level is then used to prioritize the risk mitigation activities. = false. Test Managers use these values to determine the risk level for each risk item.  Identificar y gestionar los riesgos del proyecto es fundamental para **planificar y controlar las actividades de prueba,** asegurando que se prioricen los esfuerzos donde más impacto pueden tener. 
- Test Analysts can Reduce product risk During the project by:<br>
a- **Designing** effective test cases that **demonstrate** unambiguously whether tests pass or fail.<br>
b- **Participating** in **reviews** of software work products such as requirements, designs, and user documentation.<br>
c- [x] All of the above.<br> 
- Implement appropriate risk mitigation activities identified in the test execution. = false. Implement appropriate risk mitigation activities identified in the test strategy and test plan.
- During the project, Test Analysts should seek to do the following:
a- Identify new risks from information obtained during testing.
b- Re-evaluate known risks based on additional information gathered as the project unfolds, adjusting risk likelihood, risk impact, or both.
c- Reduce product risk by designing effective test cases that demonstrate unambiguously whether tests pass or fail.
d- All of the Above. [x] 
- Test Analysts help to determine risk mitigation options by:
a- investigating opportunities for gathering accurate test data.
b- creating and testing realistic user scenarios.
c- conducting usability studies among others.
d- All of the Above. [x] 
- We can use the level of risk to prioritize tests. = True.  El nivel de riesgo para priorizar pruebas permite centrar esfuerzos en áreas más críticas, optimizando recursos y mejorando la efectividad del testing.
- The Test Analyst must wait for a user acceptance test to discover any usability issues. = false. Test Analyst might determine that usability issues are a significant risk for a new test object. Rather than wait for a user acceptance test to discover any issues.
- The Test Analyst might prioritize an early usability test based on a prototype to help identify and resolve usability design problems early before the user acceptance test. = true
- Prioritization must be considered as early as possible in the **execution** stage. = false. This prioritization must be considered as early as possible in the planning stages so that the schedule can accommodate the necessary testing at the necessary time.
- We Run Tests in strict risk order called : depth- first
- “breadth-first” is : a sampling approach is used to select a sample of tests across all the identified risk areas using risk level to weight the selection while at the same time ensuring coverage of every risk at least once
- Whether risk-based testing proceeds depth-first or breadth-first, it is possible that the time allocated for testing might be consumed without all tests being run. true. en las pruebas basadas en riesgo, el tiempo disponible puede agotarse antes de ejecutar todas las pruebas planificadas, lo que refleja la realidad de priorizar pruebas según riesgo para optimizar recursos y resultados.


















