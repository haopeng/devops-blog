---
title: Scaling my kubernetes deployment
date: 2019-02-02
tags: ["kubernetes", "code"]
---
Scaling my Kubernetes deployment

<!--more-->

'''sh
    $kubectl scale deployments/kubernetes-bootcamp --replicas=4
'''

Now check whether it is scaled up:
'''sh
    $kubectl get deployments
NAME             READY   UP-TO-DATE   AVAILABLE   AGE
webhook-server   1/1     1            1           16s

$kubectl get pods -o wide
NAME                READY   STATUS      RESTARTS   AGE    IP           NODE       NOMINATED NODE   READINESS GATES
pod-with-defaults   0/1     Completed   0          7h2m   172.17.0.3   minikube   <none>           <none>
'''
