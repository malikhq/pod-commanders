# Assignment Two:
Read about the of types of ApplicationSets Generators and create one example for your team
• Team Pod Container -- Matrix Generator
• Team Cluster Ninja -- Merge generator 
• Team Kube-Masters -- Pull Request Generator

# Solution
# Get the base64-encoded client cert
kubectl config view --raw -o jsonpath='{.users[?(@.name=="minikube")].user.client-certificate-data}'

# Get the base64-encoded client key
kubectl config view --raw -o jsonpath='{.users[?(@.name=="minikube")].user.client-key-data}'
