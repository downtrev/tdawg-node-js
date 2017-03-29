#comment, this is a comment
Build image run: 
  docker build -t hello-node:v2 .

Update image:
  kubectl set image deployment/hello-node hello-node=hello-node:v2
  
Run app:
  minikube service hello-node
  
Cleanup:
  kubectl delete service hello-node
  kubectl delete deployment hello-node

Stop minikube:
  minikube stop
  
#comment, this is a comment
