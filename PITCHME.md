# Docker for Windows Developers

---

![](http://maritime-connector.com/ships_uploads/maersk_mc_kinney_moller-9619907-container_ship-8-168317.jpg)

---

### What is Container Technology 
- But it works on my machine 
- Better utilization of resources
- Security without the cost of VMs 
- Ease of life 
- Developers rule the world

---

### What is Docker
- A specific container technology developed by Docker Inc
- Not the only container tech (but the biggest)
- Docker Inc have other products, Swarm, Docker Hub, Docker Cloud 
- The Cloud Native Computing Foundation (https://www.cncf.io/)

---

### Why now 
- It is mature
- Microsoft is embracing Docker tech
- It works on Windows (somewhat)
- .net Core is getting ready for prime time
- Clients are asking for it
- We can provide better DevOps without vendor lock
- You can work with more projects on your machine (with out conflicts) - hey node.js :) 

---

### Why is it relevant for us
- Because you will be part of projects that will rely on it
- Clients will ask questions about it
- Ease of life

---

### What else is in the docker ecosystem 
- Orchestrators (Kubernetes, Mesos Marathon)
- Container Registeries 
- CI products (VSTS and others)
- New ways of logging
- New ways to build apps (12-factor)

---

### Things to avoid
- Windows Containers
- Don't invent it yourself
- Be careful with new initiatives (docker eco-system is like NPM)

---

### What is Docker for Windows
- Installs the docker tools on windows 
- A windows service that runs in the background and manages a VM
- Relies on Hyper-V to run a Linux VM where the containers run
- Enables easy sharing of disk volumes with containers 
- Enables easy access to minikube (developer version of kubernetes)

---

![](https://i1.wp.com/blog.docker.com/wp-content/uploads/2013/08/KuDr42X_ITXghJhSInDZekNEF0jLt3NeVxtRye3tqco.png?ssl=1)

---

![](https://docs.docker.com/engine/images/architecture.svg)

---

![](https://success.docker.com/api/images/Docker_Reference_Architecture-_Designing_Scalable,_Portable_Docker_Container_Networks%2F%2Fimages%2Fcnm.png)