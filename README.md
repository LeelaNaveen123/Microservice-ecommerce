# Microservice-ecommerce


  1  yum update -y
    2  cd /var/lib/jenkins/workspace/pipeline1
    3  ls'
    4  ls
    5  git branch
    6  git checkout master
    7  ls
    8  cd charts/
    9  ls
   10  cd ..
   11  cd pipeline1
   12  ls
   13   tree
   14  sudo dnf install maven -y
   15  whoami
   16  id jenkins
   17  ls -ld /var/lib/jenkins
   18  ls -ld /var/lib/jenkins/workspace
   19  ls -ld /var/lib/jenkins/workspace/pipeline1
   20  ls -ld /var/lib/jenkins/workspace/pipeline1/services
   21  ls -ld /var/lib/jenkins/workspace/pipeline1/services/api-gateway
   22  find /var/lib/jenkins/workspace/pipeline1 -maxdepth 3 -printf "%u %g %p\n" | head -50
   23  sudo chown -R jenkins:jenkins /var/lib/jenkins/workspace/pipeline1
   24  find /var/lib/jenkins/workspace/pipeline1 -printf "%u %g %p\n" | grep services | head
   25  sudo dnf install -y nodejs
   26  node -v
   27  npm -v
   28  sudo systemctl restart jenkins
   29  which npm
   30  cat /etc/os-release
   31  sudo dnf install -y libatomic
   32  ls -l /usr/lib64/libatomic.so*
   33  which node
   34  node -v
   35  ldd $(which node)
   36  sudo dnf install docker -y
   37  cd /var/lib/jenkins/workspace/pipeline1
   38  ls
   39  kubectl get po
   40  kubectl delete po --all
   41  kubectl get po
   42  kubectl delete po --all
   43  kubectl get po
   44  kubectl describe pod product-microservice-7c46bc8b6c-gczpn
   45  kubectl describe pod user-microservice-595768bf5c-sdws6
   46  kubectl get po
   47  cat charts/microservice/values/api-gateway.yaml
   48  docker images
   49  cat charts/microservice/values/product-service.yaml 
   50  cat charts/microservice/values/user-service.yaml 
   51  x
   52  kubectl get po
   53  helm uninstall product
   54  helm uninstall user
   55  kubectl get po
   56  kubectl get pods -o wide
   57  kubectl get nodes
   58  kubectl create namespace monitoring
   59  kubectl get ns
   60  helm repo add prometheus-community https://prometheus-community.github.io/helm-charts
   61  cd /var/lib/jenkins/workspace/pipeline1
   62  ls
   63  eksctl scale nodegroup   --cluster techitfactory-cluster   --name default   --nodes 3
   64  kubectl get nodes
   65  eksctl scale nodegroup   --cluster techitfactory-cluster   --name default   --nodes 3
   66  kubectl get nodes -L node.kubernetes.io/instance-type
   67  cd /var/lib/jenkins/workspace/pipeline1
   68  ls
   69  kubectl get nodes
   70  aws eks update-nodegroup-config   --cluster-name techitfactory-cluster   --nodegroup-name <nodegroup-name>   --scaling-config minSize=2,maxSize=4,desiredSize=3
   71  aws eks list-nodegroups --cluster-name techitfactory-cluster
   72  aws eks update-nodegroup-config   --cluster-name techitfactory-cluster   --nodegroup-name default-20260701135341736000000001   --scaling-config minSize=2,maxSize=4,desiredSize=3
   73  kubectl get nodes
   74  aws eks list-updates   --cluster-name techitfactory-cluster   --nodegroup-name default-20260701135341736000000001
   75  kubectl get nodes -w
   76  kubectl get nodes
   77  kubectl get pods -n monitoring
   78  helm status monitoring -n monitoring
   79  kubectl get nodes -o wide
   80  kubectl describe pod monitoring-grafana-5fd5797456-2ps9d -n monitoring
   81  kubectl get po
   82  cd /var/lib/jenkins/workspace/pipeline1
   83  ls
   84  kubectl get nodes
   85  kubectl get po
   86  ping google.com
   87  cd /var/lib/jenkins/workspace/pipeline1
   88  ls
   89  kubectl get po
   90  kubectl describe pod api-gateway-microservice-7cdf557b79-rlxmk
   91  kubectl get nodes
   92  kubectl describe node ip-10-0-1-137.ec2.internal | grep -A10 "Capacity"
   93  ps -ef | grep kubelet
   94  kubectl get pods -A -o wide
   95  kubectl get node ip-10-0-1-137.ec2.internal -o jsonpath='{.status.capacity.pods}{"\n"}'
   96  helm list
   97  kubectl get node ip-10-0-1-137.ec2.internal -o yaml | grep -i pods
   98  kubectl describe daemonset aws-node -n kube-system
   99  aws eks list-nodegroups --cluster-name techitfactory-cluster
  100  aws eks describe-nodegroup   --cluster-name techitfactory-cluster   --nodegroup-name default-20260701135341736000000001
  101  ping google.com
  102  cd /var/lib/jenkins/workspace/pipeline1
  103  ls
  104  kubectl get po
  105  kubectl get po -n monitoring
  106  ls -R
  107  kubectl get cluster
  108  eksctl get cluster
  109  aws eks list-clusters --region us-east-1
  110  aws eks update-kubeconfig --region us-east-1 --name techitfactory-cluster
  111  kubectl get nodes
  112  sudo mkdir -p /var/lib/jenkins/.kube
  113  sudo cp /root/.kube/config /var/lib/jenkins/.kube/config
  114  sudo chown -R jenkins:jenkins /var/lib/jenkins/.kube
  115  sudo systemctl restart jenkins
  116  sudo mkdir -p /var/lib/jenkins/.kube
  117  sudo cp /root/.kube/config /var/lib/jenkins/.kube/config
  118  sudo chown -R jenkins:jenkins /var/lib/jenkins/.kube
  119  sudo -u jenkins kubectl get nodes
  120  aws sts get-caller-identity
  121  sudo -u jenkins aws sts get-caller-identity
  122  sudo su - jenkins
  123  aws configure
  124  which aws
  125  sudo systemctl restart jenkins
  126  echo $KUBECONFIG
  127  sudo -u jenkins aws eks update-kubeconfig ...
  128  sudo -u jenkins aws eks update-kubeconfig   --region us-east-1   --name techitfactory-cluster
  129  sudo -u jenkins kubectl get nodes
  130  sudo -u jenkins aws sts get-caller-identity
  131  kubectl edit configmap aws-auth -n kube-system
  132  sudo -u jenkins kubectl get nodes
  133  curl -v http://ad251331b84b84361ac0d2d5e72abeb8-1387099725.us-east-1.elb.amazonaws.com
  134  curl -i http://ad251331b84b84361ac0d2d5e72abeb8-1387099725.us-east-1.elb.amazonaws.com/
  135  ls
  136  git status
  137  git add .
  138  git status
  139  git commit -m "Add complete microservices project with Kubernetes, Helm, Jenkins, Prometheus and Grafana"
  140  git remote -v
  141  git branch
  142  git add .
  143  git commit -m "Add complete microservices project with Jenkins, Kubernetes, Helm, Prometheus and Grafana"
  144  git push -u origin main
  145  history
