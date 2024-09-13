Le sujet de la vidéo est la flexibilité offerte par EKS (Amazon Elastic Kubernetes Service) pour utiliser un autre CNI (Container Network Interface) comme **Cilium**. Le changement principal abordé est la possibilité de créer des clusters EKS sans les add-ons réseau par défaut d'AWS (AWS VPC CNI, kube-proxy et CoreDNS), permettant ainsi aux utilisateurs d'installer un CNI tiers comme Cilium.

### Points clés :
1. **Flexibilité du CNI** : AWS permet désormais aux utilisateurs de créer des clusters EKS sans les add-ons réseau par défaut, leur permettant ainsi d'installer leur propre CNI, comme Cilium.
   
2. **Suppression des add-ons par défaut** : En désactivant AWS VPC CNI et kube-proxy lors de la création du cluster, les utilisateurs peuvent installer un CNI différent comme Cilium, qui utilise eBPF pour remplacer kube-proxy.

3. **Avantages de Cilium sur EKS** : Cilium, en tant que CNI, offre des fonctionnalités réseau avancées comme le remplacement de kube-proxy avec eBPF pour une performance optimisée et une meilleure gestion des politiques réseau.

4. **Gestion des groupes de nœuds** : Après l'installation de Cilium, les utilisateurs peuvent ajouter des groupes de nœuds pour rendre le cluster pleinement opérationnel.

5. **ENI (Elastic Network Interface)** : EKS recommande d'utiliser le mode ENI, qui permet aux pods de recevoir des adresses IP directement depuis le VPC, supprimant ainsi le besoin de tunneling et améliorant les performances réseau.

Cette nouvelle flexibilité dans EKS permet aux utilisateurs de personnaliser l'infrastructure réseau de leur cluster en choisissant le CNI le plus adapté, comme Cilium, tout en optimisant les performances et la sécurité réseau.

Regardez la vidéo complète ici : [https://www.youtube.com/watch?v=DnzwxDxgkvk](https://www.youtube.com/watch?v=DnzwxDxgkvk)
