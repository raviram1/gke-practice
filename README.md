# gke-practice

  111  kubectl get nodes
  112  kubectl version
  113  gcloud container clusters get-credentials <cluster-name> --zone <zone_name> --project <project-name>
  117  kubectl create deployment ghost-deploy --replicas=3 --image=ghost --port=80 --dry-run=client -o yaml > deployment.yaml
  118  ls -lrt
  119  cat deployment.yaml
  120  kubectl get pods
  121  kubectl apply -f deployment.yaml
  122  kubectl get pods -w
  123  kubectl get pods
  124  kubectl get all
  125  kubectl get deployment ghost-deploy
  126  kubectl describe deployment ghost-deploy
  127  kubectl get svc
  128  kubectl get pod
  129  kubectl describe pod
  131  kubectl get namespaces
  135  kubectl expose deploy ghost-deploy --type=LoadBalancer --port=80 --target-port=2368 --dry-run=client -o yaml > service.yaml
  136  cat service.yaml
  138  kubectl get svc
  139  kubcetl apply -f service.yaml
  142  kubectl get svc
  145  cp deployment.yaml deployment1.yaml
  154  kubcetl apply -f deployment1.yaml
  157  kubectl get deploy
  158  kubectl get pods
  159  ls -lrt
  160  cp service.yaml service1.yaml
  161  vi service
  162  vi service1.yaml
  164  kubectl apply -f service1.yaml
  165  kubectl get svc
  166  kubectl delete all --help
  167  kubectl get all -l app=ghost-deploy1
  170  kubectl get all
  179  kubectl describe deploy ghost-deploy1
  180  kubectl delete all -l app=ghost-deploy1
