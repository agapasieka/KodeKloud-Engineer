# Solution

1. Create manifest file for pod
    ```
    apiVersion: v1
    kind: Pod
    metadata:
      name: pod-httpd
      labels:
        app: httpd_app
    spec:
      containers:
      - name: httpd-container
        image: httpd:latest
        command: ["sleep", "infinity"]
    ```
2. Deploy pod
   ```
   kubectl create -f pod.yaml
   ```
