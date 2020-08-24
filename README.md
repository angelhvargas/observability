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

Documentos de acceso público, pero queda prohibida cualquier reproducción o distribucuión, copia o uso no autorizado.
