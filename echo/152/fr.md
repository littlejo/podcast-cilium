**Aperçu de KCLI**  
KCLI est un outil conçu pour offrir une expérience utilisateur unifiée lors de l’utilisation de différentes plateformes de virtualisation (Libvirt, vSphere, AWS, Azure, GCP, IBM Cloud, OpenStack, etc.) et de clusters Kubernetes (kubeadm, OpenShift, OKD, k3s, et plus). Il est très polyvalent, permettant de gérer des machines virtuelles (VM) et des clusters Kubernetes, d’automatiser la création des plans de contrôle et d’intégrer des technologies comme HyperShift pour des plans de contrôle hébergés.

### Fonctionnalités principales :
- **Gestion unifiée** : Gérez des VMs et des clusters Kubernetes sur plusieurs plateformes, telles que AWS, GCP, Azure, et OpenShift.
- **Automatisation des clusters** : Automatisation de la configuration des plans de contrôle, des nœuds de travail et d'autres composants, avec la prise en charge de kubeadm et d'OpenShift.
- **HyperShift** : Permet de déployer des plans de contrôle hébergés, similaire à EKS, facilitant l'extension et la gestion des clusters Kubernetes.
- **Paramètres prédéfinis** : Vous pouvez personnaliser les configurations telles que le nombre de plans de contrôle, les ressources des nœuds et l’installation d’applications supplémentaires (ex. : stockage local, OpenShift Data Foundation, Multicluster Engine).
- **Intégration avec Cilium et les politiques réseau** : KCLI prend en charge Cilium comme solution réseau, permettant des fonctionnalités avancées de mise en réseau et de sécurité pour les environnements Kubernetes.

### Exemple d’utilisation :
Dans la démo, l'intervenant utilise une instance GCP avec 100 Go de RAM et 64 CPU pour montrer la création d'un cluster OpenShift. Il montre également l’installation de composants supplémentaires comme le stockage local, Cilium et HyperShift pour gérer les plans de contrôle hébergés.

### Flux de travail :
- **Création de VMs** : Utilisez KCLI pour créer des VMs pour les plans de contrôle et les nœuds de travail.
- **Configuration du cluster** : Définissez les paramètres du cluster via un fichier de paramètres ("params"), y compris le nombre de nœuds et les applications supplémentaires.
- **Surveillance** : KCLI fournit diverses commandes pour surveiller et gérer les VMs, les clusters et les opérateurs Kubernetes.

### Outils supplémentaires :
- **Accès console** : Accès direct via SSH et console série pour le dépannage.
- **Mise à l’échelle** : Mettez facilement à l’échelle les nœuds de travail et ajustez dynamiquement les ressources du cluster.
- **Extensibilité** : KCLI est hautement configurable, permettant aux utilisateurs de personnaliser presque tous les aspects de la création de VMs et de clusters, du stockage à la mise en réseau.

Vous pouvez regarder la vidéo complète ici : [https://www.youtube.com/watch?v=Mt5YyO0pRZ8](https://www.youtube.com/watch?v=Mt5YyO0pRZ8)
