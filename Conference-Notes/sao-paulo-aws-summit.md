# 04-08-2022 São Paulo AWS Summit (by @marciok)

- EC2 global view to see where your resources are allocated and consuming computing.
- Step functions to automate internal processes, combine manual and automated tasks ex: User validation, onboardings etc..
- Diversify when using spot instances, use different regions and sizes.
- Spot instances are good for jobs type of processes, we can integrate on with SidekiqWorkers
- EKS helps manage K8S machines, making easier to keep your cluster healthy 
- [Single table design with DynamoDB can help scale and improve performance](https://aws.amazon.com/blogs/compute/creating-a-single-table-design-with-amazon-dynamodb/)
- NewRelic can aggregate and filter logs for a good price
- Try chaos engineer, what if a third party data provider fails? 
- [Well Architected Framework](https://docs.aws.amazon.com/wellarchitected/latest/framework/welcome.html)
- Use MongoDB TTL for documents that are not useful anymore
- MongoDB `$facet` operator do not use indexes after the first match
- 'every ms counts', make sure to use lean and clean functions/code.
- [Porpuse-built DB stragegy](#IMG_1352). We don't need to *exclusevely* work with just one kind of DB. 
- Use caching alongside asynchronous functions (jobs, in our case).
- Things will fails eventually, so make sure to have a fallback strategy in hand.

---

Pictures 


![IMG_1342](https://user-images.githubusercontent.com/311156/182886755-1ebe8283-be1a-428f-99f4-fb6c9bb018e8.jpeg)
![IMG_1343](https://user-images.githubusercontent.com/311156/182886778-ea703798-5abd-4b97-acd4-658e2d7d2c58.jpeg)
![IMG_1344](https://user-images.githubusercontent.com/311156/182886786-c550d64f-c0a8-45c9-81d4-7e8c3d04e5f4.jpeg)
![IMG_1347](https://user-images.githubusercontent.com/311156/182886791-18c555ae-2ee4-49dc-906e-45a300f56a13.jpeg)
![IMG_1349](https://user-images.githubusercontent.com/311156/182886794-21065744-f0cc-451b-a216-57462f3fdbc7.jpeg)
![IMG_1350](https://user-images.githubusercontent.com/311156/182886797-beb4a249-0f4c-446e-91ac-1e94bc6e9f0a.jpeg)
![IMG_1351](https://user-images.githubusercontent.com/311156/182886800-da6fbfc8-51c7-4899-988d-a56950927f64.jpeg)
![IMG_1353](https://user-images.githubusercontent.com/311156/182886802-f949768a-1315-4e81-93cb-0e33fc4bc660.jpeg)
![IMG_1354](https://user-images.githubusercontent.com/311156/182886805-c9873303-ae14-4e70-83c6-cd1b7255f10d.jpeg)
![IMG_1355](https://user-images.githubusercontent.com/311156/182886813-66795635-151e-4a54-8b11-79028b871173.jpeg)
![IMG_1356](https://user-images.githubusercontent.com/311156/182886823-77eca03a-e736-4be9-965a-4682a9453f8b.jpeg)
![IMG_1352](https://user-images.githubusercontent.com/311156/182886828-6fb54cbc-3f07-41cd-a7db-e60b91c37496.jpeg)
![IMG_1346](https://user-images.githubusercontent.com/311156/182886833-b1528b2a-d1e3-459d-979e-5d777127df60.jpeg)
