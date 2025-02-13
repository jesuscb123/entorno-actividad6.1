# entorno-actividad6.1

### 1. Crea el diagrama de uso haciendo uso de platuml, representado los actores y casos de uso que identifiques en los requisitos.

En canva:
![image](https://github.com/user-attachments/assets/2e5647cc-dd75-4ed6-87b8-cede01dddef7)

Con plantUML:

@startuml
actor Cliente

Cliente --> (Validarse en el sistema)

(Validarse en el sistema) --> (Sacar dinero)

(Validarse en el sistema) --> (Hacer transferencia)

(Validarse en el sistema) --> (Realizar ingreso)

(Sacar dinero) --> (Verificar saldo suficiente)

(Sacar dinero) --> (Verificar límite diario)

(Sacar dinero) -down-> (Avisar saldo insuficiente)

(Sacar dinero) -down-> (Avisar límite diario)

@enduml

![image](https://github.com/user-attachments/assets/2d1e0e3e-3e94-4fa6-b89d-a3826f1e605b)

### 2. Describe, haciendo uso de la plantilla, al menos el caso de uso "Sacar dinero", con las interacciones que tiene entre el actor y el caso de uso.

Para que el usuario pueda realizar alguna operación, deberá autentificarse previamente. Cuando el usuario quiera realizar alguna acción, comprobará si dispone de saldo disponible para realizar dicha operación. Por ejemplo, si desea sacar dinero, el cajero comprobará si tiene saldo disponible para sacar la cantidad deseada.

### 3. Responde a las siguiente preguntas:¿Para qué me sirve tener/realizar un diagrama de casos de uso modelando el sistema que se representa? ¿Qué aporta?

Sirve para ayudar al programador a realizar el código del sistema, debido a que tienes de manera gráfica y estructurada, como se va a utilizar el sistema y ayuda a implementar el código mucho más rápido y claro.

Aporta una estructura más clara y guiada para realizar el código.
