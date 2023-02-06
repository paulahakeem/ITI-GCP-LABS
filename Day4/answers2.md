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
# try to pull the image
- screenshot from terminal ![Screenshot_20230206_060245](https://user-images.githubusercontent.com/116673091/216881191-b3a49f38-7383-4486-8e64-aab417be23b8.png)
---
### 2- Using Cloud Functions
# - Create a Function that runs whenever a file is uploaded to a cloud storage bucket
- screenshot from console ![Screenshot_20230206_064607](https://user-images.githubusercontent.com/116673091/216885737-70fafa3f-a929-4974-a5b2-af3cd10982ba.png)
---
### 3- Using Cloud Run:
- Build and Run any sample app (pulled from GCR) ![Screenshot_20230206_065621](https://user-images.githubusercontent.com/116673091/216887055-d9c90634-6e0d-4c5d-9cb4-9bdac1343059.png)
### 4- Using App Engine:
iam used this link https://cloud.google.com/appengine/docs/standard/python3/building-app/writing-web-service
run commands 
```bash
git clone https://github.com/GoogleCloudPlatform/python-docs-samples.git
cd python-docs-samples/appengine/standard_python37/
gcloud app deploy
gcloud app browse
```
- screenshot from terminal ![Screenshot_20230206_072139](https://user-images.githubusercontent.com/116673091/216890049-155b632e-cefe-407a-ac62-7daa1f9b2828.png)
- screenshot from browser ![Screenshot_20230206_072249](https://user-images.githubusercontent.com/116673091/216890213-1e475768-3035-4ce1-8a0e-f3788b94624d.png)
----


