### 1- Create a private GKE cluster
-![Screenshot_20230205_032015](https://user-images.githubusercontent.com/116673091/216821447-b0d00e7a-dca3-4d85-9d13-e6d5bb81772b.png)
---
### 2- Deploy Nginx as a deployment using latest Nginx docker image on Docker Hub
```bash 
gcloud components install kubectl
gcloud container clusters get-credentials paula-cluster --zone us-central1 --project paula-iti
kubectl create deployment nginx-deployment --image=nginx:latest
kubectl get deployment
```
- screenshot from terminal ![Screenshot_20230205_034826](https://user-images.githubusercontent.com/116673091/216823147-87b8c7da-0dc7-493e-a9fc-4565b4330ad4.png)
- screenshot from console ![Screenshot_20230205_035046](https://user-images.githubusercontent.com/116673091/216823326-9ba69ede-78ef-47da-9896-7cf3c201aa40.png)
---
### 3- Expose your Nginx deployment using Kubernetes LoadBalancer Service.
```bash 
kubectl expose deployment nginx-deployment --port=80 --target-port=80 --name nginx-lb --type=LoadBalancer
kubectl get services
```
- screenshot from terminal ![Screenshot_20230205_040309](https://user-images.githubusercontent.com/116673091/216824138-4761b461-7eb4-4a15-ab3a-375227c33f34.png)
- screenshot from console ![Screenshot_20230205_040657](https://user-images.githubusercontent.com/116673091/216824264-452ff52e-208b-4d41-829f-6f9477eea5fa.png)
---
### 4- What is the type of GCP Load Balancer that is created for your LB service?
- target pool-based type
- screenshot from console ![Screenshot_20230205_040657](https://user-images.githubusercontent.com/116673091/216824611-bb4ae7e1-67c6-44ae-80c9-f392fb555a19.png)
---
### 5- Use kubectl to view container logs
```bash
kubectl get pods
kubectl logs nginx-deployment-84d8b48bcf-csjn6
```
- screenshot from terminal![Screenshot_20230205_041919](https://user-images.githubusercontent.com/116673091/216824930-99ef66a2-b20a-48ee-a428-7d1352a916b0.png)
---
### 6- Use cloud logging service to view container logs.
- screenshot from console ![Screenshot_20230205_042621](https://user-images.githubusercontent.com/116673091/216825326-50e6dd0b-94f3-4ec8-a06d-8f01e25cb1a0.png)
---
### 7- (Bonus) setup a HTTP load balancer for your deployment using the kubernetes ingress resource (Bonus)``
-yaml file 
```yaml 
apiVersion: networking.k8s.io/v1
kind: Ingress
metadata:
  name: myingress
spec:
  defaultBackend:
    service:
      name: nginx-lb 
      port:
        number: 80
```
- screenshot from console ![Screenshot_20230205_051620](https://user-images.githubusercontent.com/116673091/216827909-e50a7585-8d58-41fe-bcd2-266bfa55f692.png)
- screenshot form acess ip ![Screenshot_20230205_051628](https://user-images.githubusercontent.com/116673091/216827957-fc834d01-001f-4254-9995-2f778e2e49f9.png)
---





