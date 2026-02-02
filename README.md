# mulesoft

MuleSoft Catalyst pillars can be broken into 6paths :
1. Busines outcomes:
    - Business outcomes : contains information about how to identify and measure outcomes and align them to KPIs and stakeholders
2. Technolgy Delivery: path to operate MuleSoft’s Anypoint Platform
    - Anypoint Platform  : 
    - Projects
3. Org enablement
   - Center for Enablement (C4E) :  enables organizations to maximize their results through best practices, reuse, and self-service
   - Internal support : helps customers build support models for projects involving Anypoint Platform
   - Training : shows customers how to use enablement resources to provide training and certification
  


API-Led Connectivity:
1. System APIs
2. process APIs
3. experience APIs

<img width="653" height="318" alt="image" src="https://github.com/user-attachments/assets/e5a191b1-09f3-4277-93d8-1ac0fd0dbbc6" />


DevOps is a movement with a set of practices that aim to increase collaboration between IT operations and development teams.


**Mule Event**: Mule Message + Variables + error info

**Mule Message**: Payload + Attributes



**RAML (RESTful API Modeling Language)** is a YAML-based language used for designing, describing, and documenting RESTful APIs (1:09). It promotes a design-first approach for consistency and reusability, allowing developers to define API contracts before implementation.

MuleSoft prefers RAML due to its:

- Deep integration with the Anypoint Platform : 
      RAML seamlessly works with MuleSoft's tools like Design Center, API Manager, Studio, and Exchange for end-to-end API lifecycle management.
- Support for reusable components: 
      Features like resource types (2:47) and traits (19:28) allow developers to define common patterns and apply them across multiple APIs, reducing code duplication.
- Rapid development: 
      RAML enables quick generation of documentation, mock services, and client SDKs, facilitating parallel development and testing.
- Consistency and governance: 
    It helps enforce standards, making APIs more predictable and manageable in large enterprise environments.


RAML is central to MuleSoft's API-led connectivity strategy, providing a standardized, reusable contract for effective API development and management.

**Traits**:
- they are resource types
- resource --> from resource as a whole (method, request, and response)
- traits --> extract patther from only for method (request and response)
- used for more than one method

**Mule 4:**
Mule 4 are mavenised projects (pom.xml : is a file where you mention all proj related info and depnedecy and download and mention in the pom.xml) here the pom.xml is updatede automatically when you drag or import anything.

Mule structure
      1. Payload
      2. attributes
      3. variables
      4, error

Files important for a mule 4 proj
      - pom.xml
      - src/main/mule
      - /src/main/resources
      - mule-artifact.json

Each Mule app xml has -
      - Message flow - Graphical representation
      - Global elements - contains all the config details
      - configuration aml - contains all the xml version of graphical representation

Flow, SubFlow and PrivateFlow:

- Flow :
        - atlease one single flow
        - 3 parts:  Source, process, error handling
  
  <img width="448" height="428" alt="image" src="https://github.com/user-attachments/assets/bd0502c2-1bee-4aec-9bc2-663cb540fed6" />
        
- SubFlow:
        - cannot be independent and needs to be refrenced by flow
        - when you dont have Source and error handling part but only have process filters
        - Error handling is being handled by calling flow or private flows.
  

- Private Flow:
        - cannot be independent and needs to be refrenced by flow
        - when you dont have Source but only have process and error handling filters
  
  <img width="472" height="386" alt="image" src="https://github.com/user-attachments/assets/fb10f986-d43c-4571-bc53-563d771cc2c2" />
