### 1- Using gcloud & Docker
# Configure Docker & gcloud to work with GCR of your project
```bash 
gcloud auth configure-docker
```
- screenshot fro terminal ![Screenshot_20230206_025202](https://user-images.githubusercontent.com/116673091/216872726-664c8298-3742-4c19-a231-61b5c1ce431b.png)
# Push Nginx docker (private) image to GCR 
Dockerfile && conf file
![Screenshot_20230206_055455](https://user-images.githubusercontent.com/116673091/216880367-75e2e165-0184-4ff3-81b9-fbcbace23a6a.png)
![Screenshot_20230206_055451](https://user-images.githubusercontent.com/116673091/216880351-aa92b033-5fa1-4d01-a2e5-c0025d22558c.png)
- screenshot from console ![Screenshot_20230206_055908](https://user-images.githubusercontent.com/116673091/216880798-5fb8e1ca-82a3-4252-a227-3cc565a66f80.png)
# Pull this image into a k8s setup or on a VM
- screenshot from terminal ![Screenshot_20230206_060245](https://user-images.githubusercontent.com/116673091/216881191-b3a49f38-7383-4486-8e64-aab417be23b8.png)
---
