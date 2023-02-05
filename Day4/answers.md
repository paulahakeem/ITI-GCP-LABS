### 1- Using gsutil: 
## - Create 3 buckets. 
```bash
gsutil mb gs://<bucketname_must_be_unique>
```
- screenshot from terminal ![Screenshot_20230205_061411](https://user-images.githubusercontent.com/116673091/216831078-4bea949f-33e0-43bc-9a32-13d7ba2bc4d7.png)
- screenshot from console ![Screenshot_20230205_061757](https://user-images.githubusercontent.com/116673091/216831106-83528d99-4417-4056-a750-03d7bfc9ae07.png)
--
## - Enable Versioning for them.
```bash 
 gsutil versioning set on gs://<bucket-name>
 ```
- screenshot from terminal  ![Screenshot_20230205_061922](https://user-images.githubusercontent.com/116673091/216831275-b9b1afbe-98ca-46d5-b746-427f2b3ac5c4.png)
- screenshot from console ![Screenshot_20230205_062359](https://user-images.githubusercontent.com/116673091/216831432-1751b83b-250b-45ff-b7ee-6227b51a87f4.png)
--
## - Upload a file into bucket-1 
```bash
gsutil cp gs:<file-path-in-bucket> gs://<bucket-name>/
```
- screenshot from terminal ![Screenshot_20230205_063501](https://user-images.githubusercontent.com/116673091/216831947-0af39da6-f03c-48b5-a3a7-131c242c64ce.png)
- screenshot from console![Screenshot_20230205_063536](https://user-images.githubusercontent.com/116673091/216832007-ccd7bc21-77e7-4824-9f10-572f5b748228.png)
--
# then copy it from bucket-1 into bucket-2 & bucket-3.
```bash 
gsutil cp gs:<file-path-in-bucket> gs://<bucket-name>/
```
- screenshot from terminal  ![Screenshot_20230205_064221](https://user-images.githubusercontent.com/116673091/216832320-0bf36c78-af5b-47b3-a324-e0a0659aa5f8.png)
## - Delete the file from bucket-1
```bash 
gsutil rm gs:<file-path-in-bucket>
```
- screenshot from terminal  ![Screenshot_20230205_064417](https://user-images.githubusercontent.com/116673091/216832408-a98813ae-a1f1-4cd0-b652-58db4b30a7db.png)
---
### 2.Host a static website on a standard public GCS bucket 
- screenshot from console  ![Screenshot_20230205_071804](https://user-images.githubusercontent.com/116673091/216834122-d6b65216-34b6-4e9f-b9aa-92340f88add2.png)
- screenshot from browser without loadbalancer ![Screenshot_20230205_072740](https://user-images.githubusercontent.com/116673091/216836190-c2359708-01fa-46e8-ab8f-13fc857a8c54.png)
- screenshot from browser after loadbalancer ![Screenshot_20230205_074135](https://user-images.githubusercontent.com/116673091/216836208-2215712c-e5c7-4a12-a446-b656758e275d.png)
- screenshot from loadbalancer conole ![Screenshot_20230205_074847](https://user-images.githubusercontent.com/116673091/216836228-298b76ef-accc-4ede-b09c-443ae3ee73f9.png)


