# Deploy the NGINX Ingress namespace
kubectl apply -f ingress-nginx-namespace.yaml



# Deploy the standard Apache server
kubectl apply -f apache-deployment.yaml

# Create services for standard Apache server
kubectl apply -f apache-service.yaml



# Deploy your custom Apache server
kubectl apply -f custom-apache-deployment.yaml

# Create services for custom Apache server
kubectl apply -f custom-apache-service.yaml




# Create the Ingress resource
kubectl apply -f apache-ingress.yaml


# Deploy the NGINX Ingress controller
kubectl apply -f nginx-ingress-controller.yaml

