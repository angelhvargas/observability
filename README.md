# Tesis acerca de observabilidad. 

APLICACIÓN DE LA OBSERVABILIDAD COMO MECANISMO DE PREVENCIÓN DE FALLAS EN APLICACIONES DESPLEGADAS EN UN SISTEMA DISTRIBUIDO DE MICROSERVICIOS.

Este documento se mantendra en lenguaje Espanol.

## Objetivos iniciales:

~ - Plantear el problema~
- Disenar el entorno de pruebas
- Definir los objetivos clave para el monitoreo del sistema.
- Desarrollar el entorno de pruebas.
- Definir cuales son los observables en la plataforma de microservicios distribuidos, por ejemplo Kubernetes será la elección como plataforma para manejar nuestros containers. 
- Identificar que metodologias/modelos son aplicados para observar sistemas.

Notas:
1. Kubernetes será desplegado on-prem (no Cloud) para obtener dominio sobre el plano de control. En K8s vamos a desplegar un grupo de microservicios que puedan ser inicialmente monitoreados en combinación con los componentes del plano de control.

## Proposición para el entorno de pruebas:

Para el entorno de pruebas, vamos a desplegar Kubernetes en un entorno virtual, no utilizaremos minikube ya que necesitamos simular un plano de control aislado con nodos que puedan ser modificados para poder agregar condiciones que creen inestablidad en el sistema distribuido.

Se quiere también crear varios microservicios que se comuniquen a través del protocolo gRCP, esta aplicación se moniteara con Prometheus para evaluar las conficiones del sistema.

## Entorno de integración end-to-end, interacción minima, propuesta:

1. desplegar infraestructura como codigo, (validación monitoreable)
2. automatizar despliegue de certificados y la rotación automatica (observable)
3. desplegar cluster de Kubernetes desde código
4. desplegar microservicios
5. validar microservicios
6. Smoke test
7. promote (promover updates desde Jenkins)
8. Aplicar observabilidad al sistema

## Tecnologías a utilizar:

- IBM Cloud
- Vagrant
- Microservicios
- Artifactory
- Vault
- Kubernetes
- Docker
- Golang
- Jenkins
- Ansible

Documentos de acceso público, pero queda prohibida cualquier reproducción o distribucuión, copia o uso no autorizado.
