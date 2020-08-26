# Tesis acerca de observabilidad. 

Aplicación de la Observabilidad como mecanismo de prevención inteligente de fallas de sistemas distribuidos.

Este documento se mantendra en lenguaje Espanol.

## Objetivos iniciales:

- Plantear el problema
- Empezar a desarrollar el entorno de pruebas.
- Definir que son observables en una plataforma de microservicios distribuidos, por ejemplo Kubernetes como entorno donde una aplicación o sistema requiere monitoreo para mantener su estado de estabilidad.
- Identificar que metodologias/modelos son aplicados para observar sistemas.


## Proposición para el entorno de pruebas:

Para el entorno de pruebas, vamos a desplegar Kubernetes en un entorno virtual, no utilizaremos minikube ya que necesitamos simular un plano de control aislado con nodos que puedan ser modificados para poder agregar condiciones que creen inestablidad en el sistema distribuido.

Se quiere también crear varios microservicios que se comuniquen a través del protocolo gRCP, esta aplicación se moniteara con Prometheus para evaluar las conficiones del sistema.

## Entorno de integración end-to-end, interacción minima, propuesta:

1 - desplegar infraestructura como codigo, (validación monitoreable)
2 - automatizar despliegue de certificados y la rotación automatica (observable)
3 - desplegar cluster de Kubernetes desde código
4 - desplegar microservicios
5 - validar microservicios
6 - smoke test
7 - promote (promover updates desde Jenkins)
8 - Aplicar observabilidad al sistema

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


Documentos de acceso público, pero queda prohibida cualquier reproducción o distribucuión, copia o uso no autorizado.
