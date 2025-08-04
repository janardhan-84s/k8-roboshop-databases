## Using Volume concept we can create databases for our roboshop applications and also mentioning our components in statefulset resource ##

1. Generally we are having a resource in k8 called " Deployment" .
  For this resource it is mainly used for stateless applications

2. But actually there is a resource called " Statefulset" especially developed 
   for stateful applications

3. Actually our roboshop project is stateful application.
   But we can treated our application as Stateful to explore this resource

4. We are also implementing Horizontal Auto scaling because it doesn't have single point 
   of failure.
   1. Horizontal scaling :  is a controller that automatically adjusts the number of pod replicas in a deployment, StatefulSet, or other scalable resource based on observed metrics like CPU or memory usage.

5. We had done with scaling the PODS based on CPU utilization
   using below conditions we are setting up the Scaling
   1. Make sure metric server is running
   2. Mentioning resources, request and limits

6. We had implementing Horizontal scaling for below components
    1. Catalogue
    2. shipping
    3. cart
    4. Frontend
    5. Payment
    6. user

7. This is the naming reference of Horizontal scaling

      kind: HorizontalPodAutoscaler