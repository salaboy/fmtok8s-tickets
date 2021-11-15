# From Monolith To K8s :: Tickets Parent Chart

Parent chart for installing Tickets Sale flow for the Conference Platform application.

## Build and Release

This repository depends on the following charts to be released: 
- [Tickets Service](https://github.com/salaboy/fmtok8s-tickets-service/)
- [Queue Service](https://github.com/salaboy/fmtok8s-queue-service/)
- [Payments Service](https://github.com/salaboy/fmtok8s-payments-service/)


```
cd charts/fmtok8s-tickets
helm dependency build
helm package .
```

Copy tar to http://github.com/salaboy/helm and push