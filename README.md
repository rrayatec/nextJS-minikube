## 1. Inicializar Docker
#
## 2. Inicializar minikube
`minikube start`
#
## 3. Ubicar el proyecto Origen con los Archivos
`Dockerfile`

`Service.yaml`

`Deployment.yaml`
#
## 4. Empaquetando el proyecto
`docker build -t website-2 .`

`docker run -p 3000:3000 website`

`docker tag website rrayad/next-sample`

`docker push rrayad/next-sample`
#
## 5 Verificar el namespace Defaul en minikube
#
## 6 crear el servicio y deployment
`kubectl apply -f Service.yaml`

`kubectl apply -f Deployment.yaml`
#
## 7. CLuster Minikube
`kubectl get pods --watch     `

`kubectl cluster-info  `      

`kubectl get svc      `   

`kubectl get po      `

`kubectl exec nextjs-app -it -- /bin/sh`    

`minikube service nextjs-app --url`

`minikube delete  `
