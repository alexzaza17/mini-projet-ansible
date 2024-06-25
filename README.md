#Fankem
## Alex Junior
### Eazytraining 18th DevOps Bootcamp
#### Period: march-april-may
Application

Il est question ici pour nous de mettre en place un code Ansible qui nous permettra de configurer une machine cliente a distance c est a dire installer docker en utilisant Apache a l aide d un role. Nous avons tout d abord creer le fichierr:
- Le dossier goup_vars qui contient le fichier prod.yml qui permettra ansible de definir l adresse de la machine sur laquelle on voudra fiare la cobfiguration et demander a Ansible d accepter la connexion a distance
- Le dossier files/secrets contient le fichier credentials.vault qui permettra de securiser la connexion
- Le dossier role qui contient le dossier apache_docker qui va etre appeler dans lorsqu on va lance la commande ansible playbook avec le fichier deploy.yml. le dossier apache_docker contient le tasks qui lui a son tour contient deux fichiers a savoir main.yml et le pre-tasks.yml
- Le fichier deploy.yml qui sera lance dans la commande notre Ansible playbook pour executer la configuration
- Le host.yml qui contient les adresses ip de la machine cliente a configurer lui aussi sera lance dans notre commande Ansible playbook  
