# Follow these steps for deployment:

# Step 1: Run the setup script

```
chmod 777 setup.sh
./setup.sh
```

# Step 2: Create a cluster

```
Kind create cluster
```

# Step 3: login to docker 

```
docker login
```

# Step 4: Create namespace for deployment:

```
kubectl create ns oai-tutorial
```

# Step 5: Update helm dependencies:

```
cd charts/oai-5g-core/oai-5g-basic
helm dependency update
```

# Step 6: Deploy command

```
helm spray --namespace oai-tutorial .
```
