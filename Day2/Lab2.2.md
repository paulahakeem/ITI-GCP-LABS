1. Create a VM with public ip :
![first isnt](https://user-images.githubusercontent.com/116673091/216274978-7ae62565-ee6a-410e-a883-7ecaaa619103.png)
- ssh from console 
![first ssh](https://user-images.githubusercontent.com/116673091/216275252-7d635d77-6066-489d-8255-a281f789fa19.png)
- ssh using cli 
![second ssh](https://user-images.githubusercontent.com/116673091/216275509-f35a5af1-559c-47b7-8072-2887d1c5809e.png)
- Enforce SSH into this VM to be IAP protected.
 ![iam ssh](https://user-images.githubusercontent.com/116673091/216276293-10fe4dc8-141e-494d-a7be-7a958a9b2682.png)
2. Create a VM without public ip then:
![privavte vm](https://user-images.githubusercontent.com/116673091/216277218-c95517d7-f8c3-45c8-bf7c-6144888eaff4.png)
- SSH into this vm. update system packages (is it possible?) no doesnt possible
![private vm](https://user-images.githubusercontent.com/116673091/216276763-b74c006d-12cd-43c2-97d2-df2542cb9a32.png)
3. Create a VM with public ip then:
– SSH into this vm 
– Update system packages.
![Screenshot_20230202_105636](https://user-images.githubusercontent.com/116673091/216278215-0fc4a98b-f2e5-49b9-8286-57ff8dd11dcb.png)
– Setup Nginx Web Server and test your setup.
![Screenshot_20230202_110015](https://user-images.githubusercontent.com/116673091/216278460-8600be2b-e798-43ed-811d-2b1e7a1b2a6a.png)
– Create a custom image from this VM named “custom-img-nginx
![Screenshot_20230125_060024](https://user-images.githubusercontent.com/116673091/216278970-7629c837-9e8a-4005-a640-f97014898d2f.png)
4. Create MIG (min 3 and max 5) of a template using the custom image “custom-img-nginx”.
![Screenshot_20230202_110624](https://user-images.githubusercontent.com/116673091/216279889-6f48b466-7d29-49df-b43b-22e1a3ad73a4.png)
![Screenshot_20230125_061024](https://user-images.githubusercontent.com/116673091/216281726-b03c89c9-af77-414c-a071-4c72f5771236.png)
![Screenshot_20230125_061944](https://user-images.githubusercontent.com/116673091/216281731-bb1b417b-cd57-4d8f-9da3-e02e476836f0.png)
![Screenshot_20230125_062042](https://user-images.githubusercontent.com/116673091/216281739-eac6a9b7-5aba-43b9-938c-3311b08a6ae8.png)
