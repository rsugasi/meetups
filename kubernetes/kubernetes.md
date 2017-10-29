

#### Nova hardening k8s - Capital One 10/26/2017
```
  Sam Brown, Oteemo
  - slides at goo.gl/p42Shd
  - code at goo.gl/fwwbgB
  - Tigera, Calco, kops
  - egress networkpolicy introduced in 1.8 version
  - Kube API Server
  - Kubelet API - 10250 (Read/Write API)
  - CloudProvider Metadata e.g. In AWS, it's 169.254.169.254
  - curl, tcpdump, nmap are the tools needed
  - cadvisor runs on port 4194 on every pod
  - kubelet exploit has been around since a year now
  - kubectl , kubeadm , kubefed, minikube
```
```
  Simon Kwane 
  - Kubernetes provides User Account and Service Account
  - Kubernetes provides pluggable mechanism for
      - Authentication,
      - Authorization,
      - Admission Control
  - Authentication types
      - x.509 client certificate
      - static token file
      - password file
      - Service Account token
      - Webhook token
      - keystone
      - Open ID
  - Authorization types
      - RBAC (Role Based Access Control)
         - Role and ClusterRole
         - RoleBinding and ClusterRoleBinding
      - ABAC (Asset Based Access Control)
      - Webhook
  - Used OpenID in combination with Dex for the demo
```

#### OWASP Scaling Security for Kubernetes - 12000 Sunrise Valley 10/19/2017
```
  - Ben Pick, nVisium
  - API Server needs to be disabled if not required
  - namespaces is a good way of controlling access to Developers
  - namespaces are a collection of pods and pods a collection of containers
  - never use environment variables since its exposed to all children in the process
```
