# Cloudformation
Instructions 
Installez un serveur WordPress (le site de l’entreprise) sur AWS en utilisant :
RDS pour le stockage de la base de données
S3 pour le stockage des médias (via le plugin amazon-web-services)
EC2 et Docker pour le serveur web
ELB pour distribuer les requêtes sur les instances EC2
CloudFormation pour automatiser la création de l’infrastructure
Tous les éléments de votre infrastructure publique devront être répartis sur plusieurs zones de disponibilité (multi-AZ). Vous utiliserez le service ELB pour la répartition des requêtes vers les différentes zones de disponibilité (AZ).
Vous monterez une instance EC2 destinée à héberger l’application intranet sur un sous-réseau privé. Dans le cadre de ce cours, le contenu de l’intranet sera une simple page web HTML.

En local sur votre machine, vous créerez deux machines virtuelles Linux : une pour le serveur de fichiers et une pour le serveur VPN.
Vous établirez une liaison VPN entre votre serveur VPN local et le sous-réseau privé AWS via une instance EC2.
Vous mettrez en place de l’auto-scaling sur les instances EC2 pour augmenter le nombre de machines dès que la charge CPU des serveurs atteint 80% en moyenne sur 5 minutes et vous veillerez à être informé par un mail à chaque fois que l'événement survient.
Vous évaluerez les coûts de votre infrastructure AWS à partir de différentes hypothèses d'usage que vous formulerez.
