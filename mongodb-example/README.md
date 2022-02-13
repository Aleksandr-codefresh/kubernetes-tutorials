To be able to run mongo express with mongo DB create and apply Secret manifest:
```
apiVersion: v1
kind: Secret
metadata:
  name: mongodb-secret
type: Opaque
data:
  mongo-root-username: base64 encoded
  mongo-root-password: base64 encoded
```

### How to encode:
```
echo -n 'username' | base64
```
### How to decode:
```
echo dXNlcm5hbWU= | base64 --decode
```

## How to navigate from browser?
```
minikube service mongo-express-service
```