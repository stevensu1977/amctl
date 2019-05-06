# amctl
This is tools for AWS AppMesh , like istioctl , can be generate config, enable autoinject

## TODO List
1. genrate app mesh config (process)
2. genrate manual/auto inject like istioctl
3. install aws-appmesh-inject to k8s cluster
4. create demo appmesh use istio bookinfo app


## Resource
*   AWS Go SDK
*   K8S clieng-go
*   github.com/spf13/cobra


```bash
	amctl generate -f service.yaml
	amctl create-demo -t autoinject|manualinject -n namespace
	amctl k8s-autoinject enable|disable  -n namespace (if not installed , install frist)
 	amctl inject -t auto|manual -f <k8s deployment>.yaml