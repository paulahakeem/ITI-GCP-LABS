### 1. From Cloud console, create a VPC named “auto-vpc” with auto-mode enabled,-How many subnets created? 
- 35 subnet 
![Screenshot_20230202_093027](https://user-images.githubusercontent.com/116673091/216268913-a2e37b69-da6b-4bf0-af1d-756339c69e89.png)
---
### 2. From Cloud console, create a VPC named “custom-vpc” with auto-mode disabled and create two subnets. 
 ![215321029-e5905c12-615a-4b43-a534-5aa9b2c9dddf](https://user-images.githubusercontent.com/116673091/216269825-b629bca6-f77f-48c1-8312-922563df6515.png)
---
### 3. Using gcloud tool list all available VPCs 
![00000](https://user-images.githubusercontent.com/116673091/216270221-c3cfcd3c-c8a2-4ac2-b87a-3f6bcce78958.png)
- list subnets of each VPC.
![ssssss](https://user-images.githubusercontent.com/116673091/216270746-00d7661d-91eb-48dd-a543-36d08c0b2953.png)
![Screenshot_20230125_032351](https://user-images.githubusercontent.com/116673091/216270873-1e6a863a-5fe7-4da2-945f-799689d6c168.png)
---
### 4. Block internet access from you VPC using firewall rules.
![000](https://user-images.githubusercontent.com/116673091/216271863-971ca4bb-8fbf-4681-b281-24f54efd7185.png)

---
### 5. Create a firewall rule to allow incoming SSH requests from internet to all instances in your vpc.
![010](https://user-images.githubusercontent.com/116673091/216272380-42bf4f89-9d29-4d10-9937-ca9a1d8e91ea.png)

---
### 6. Modify the previous firewall rule to allow only ssh requests coming through Google’s IAP servers.
![Screenshot_20230125_041235](https://user-images.githubusercontent.com/116673091/216273792-c29ec051-085c-4fdf-8e9a-c5c42179eaa9.png)
