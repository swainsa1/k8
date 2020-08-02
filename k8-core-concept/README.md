# Introduction to K8s

## Why k8s 
   - Opensource for automating deployment :wq
   - Conductor of an orchestra
## Key feature 
   - Service Discovery / Load Balancing 
   - Storage Orchestration
   - Automate Rollout and rollbacks
   - Self Healing
   - Secret and configuration mgmt 
   - Horizontal Scaling
## The big picture
   - Master
    node .... node 
    pod ......pod
   - Containers are inside pod 
   -  Containers are inside pod 
   -Pod is like a space suit and human is the container 
## Building blocks
    * Pod  
    ** Container
   - Service
   - Deployment 
   - ReplicaSet
### Master Node 
   - etcd store :  Everything the master node needs to track
   - Controller Manager : Manages the request and schedules 
     this helps to manage all the incoming request 
### scheduler : When it comes to life or go away 
### API Server
### kubectl : sends the yaml/json request through api server 
#### K8 Nodes 
     - Node[Pod[container]]
     - Kubelet
     - Container Runtime 
     - Kube-Proxy
     
#### Container benefits 
    - Accelrate developer onboarding 
    - Eliminate App conflicts 
    - Environment consistency 
    - Ship software faster

#### K8 benefits 
    -  Orchestrate containers 
    - Zero downtime deployment 
    - Self healing 
    - Scale container 
##### Why k8s for developers 
    - Emulates prod locally 
    - End to end testing 
    - Ensure application scability 
    - Secret and configuration works properly
    - Performance testing
    - Diffrent deployment testing
      - Canary or A/B 

    - Help DEvOps to solve problem 

#####
Kubectl basic commands 
  - cluster-info
  - get all : Retrieves information about pods,deployments services and more
  - run [container name] -- image=[image-name]
  - ```port-foreward [pod] [port] ```: FOrward a port to allow external access
  - expose : Expose a port for a deployment/pod
  - create : create a new resource
  - apply : modify a resource
###### Options
   --dry-run : Give it a trial run without really starting the pod 
   --validate=true : Validate yaml files for synatical error 
   -  By default --validate= true 
  
  


## 
Kubernetes with docker desktop 
- To enable docker desktop with kubectl goto docker -> preference ->Enable kubernete
- Issue : If you see that kubernets is hanging while starting with an error "Keubernetes Starting"

- There was a suggestion to remove the pki folder ```rm -rf  ~/Library/Group\ Containers/group.com.docker/pki```




	 
	
  



