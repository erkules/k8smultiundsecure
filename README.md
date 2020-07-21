# Vortragsnotizen

In https://github.com/erkules/k8sworkshop gibt es viel mehr Bsp. :)

Idee: 

Wir wollen wollen schauen wie wir K8s Multi-tenant-fähig und sicherer bekommen.

# Topics

* User an Namespaces binden
* Networkpolicies
* Biske ResourceQuota
* PodPriorities
* PSP

# User an Namespace binden

Er Erkan (hessisch ausprechen) wird admin in Namespace erkan

erkanBekommtEinZuhauseRBAC.yaml

# Networkpolicies

#kubectl apply -f erkan-ns.yml
kubectl apply -f service.yml
kubectl apply -f allepodsimNamespaceErreichensich.yml

# ResourceQuota

kubectl delete -f deployment.yml
deployment.yml anpassen
kubectl apply -f resourcequota.yaml
# Dann PodPriorities mit mega Memory

ResourceQuota deleten :)

--enable-admission-plugins=PodSecurityPolicy


