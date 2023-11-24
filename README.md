---
marp: false
---

# Github Documents

- github + plantuml + archimate + marp
---

## Install
- [VSCode](https://code.visualstudio.com/)
- VSCode extension
    - plantuml
    ![Plantuml](./img/vscode_extension_plantuml.png)
    - marp
    ![MARP](./img/vscode_extension_marp.png)
---

# PlantUML
- [plantuml website](https://plantuml.com/ko/archimate-diagram)

---
- plantuml code path
    - [diagrams/src/](./diagrams/src/)
    ![plantuml code path](./img/plantuml_code_path.png)

- 이미지 생성 
    1. Right click on "diagrams" folder
    2. Left click on "Export Workspace Diagrams"
---

- Archimate Diagram List

![plantuml_archimate_list](./diagrams/out/plantuml_archimate_list.png)

---
- Sample
![Archimate](./diagrams/out/archimate.png)

---
- FIDO Image Sample
![FIDO width:600px](./img/D0_SecureVault.png)

---
- FIDO Plantuml Sample(image version)
![FIDO](./diagrams/out/FIDO.png) 

---
- FIDO Plantuml Sample(code version)
```plantuml
@startuml

node "CrossCert FIDO Secure Vault" as TCCFido <<$archimate/technology-device>> #TECHNOLOGY 

node "FIDO Authentication Service" as TCCFidoAuth <<$archimate/technology-device>> #TECHNOLOGY 
node "Fraud Detection Service" as TCCFidoDetection <<$archimate/technology-device>> #TECHNOLOGY 
node "Know Your Customer\n(T.B.D)" as TCCKYC <<$archimate/technology-device>> #TECHNOLOGY 
node "Out of Band Authentication\n(High Security Authentication)" as TCCOBA <<$archimate/technology-device>> #TECHNOLOGY 

left to right direction
TCCFido --> TCCFidoAuth
TCCFido --> TCCFidoDetection
TCCFido --> TCCKYC
TCCFido --> TCCOBA
@enduml
```
