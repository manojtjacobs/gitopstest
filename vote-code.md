
## variables
$azureContainerRegistry="mtjacr001"


git clone https://github.com/Azure-Samples/azure-voting-app-redis.git
cd azure-voting-app-redis/azure-vote/
az acr build --image azure-vote-front:v1 --registry $azureContainerRegistry --file Dockerfile .