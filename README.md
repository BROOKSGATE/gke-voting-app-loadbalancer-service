# gke-voting-app-loadbalancer-service
gke-voting-app-loadbalancer-service

 65  gcloud container clusters get-credentials dev-prod-cluster --zone northamerica-northeast1-a --project celestial-gist-401022
   66  history
   67  gcloud container clusters get-credentials dev-prod-cluster --zone northamerica-northeast1-a --project celestial-gist-401022
   68  git clone https://github.com/BROOKSGATE/gke-voting-app-loadbalancer-service.git
   69  ls
   70  cd gke-voting-app-loadbalancer-service/
   71  ls
   72  kubectl create ns votingapp-prod
   73  kubectl get ns
   74  kubectl apply -f . -n votingapp-prod
   75  kubectl get all
   76  kubectl get all -n votingapp-prod
   77  kubectl delete svc result-service -n votingapp-prod
   78  kubectl delete svc voting-service -n votingapp-prod
   79  kubectl delete svc voting-service -n votingapp-dev
   80  kubectl delete svc result-service -n votingapp-dev
