# wgs_aws_newrelic_plugin

## Installer une machine ec2 pour gérer le monitoring depuis l'AMI:

https://aws.amazon.com/marketplace/pp/B00DMMUO0O/

A la création du serveru a l'aide de l'image AMI, déployer Advanced Details, et copier le contenu du fichier newrelic_plugin.yml dans le champ texte, après y avoir renseigné les clefs newrelic et aws.

## Remplacer le code source d'origine par le code source modifié:

Remplacer le contenu du repertoire /home/ubuntu/newrelic_aws/lib par le code présent dans ce repository

## Redémarrer le daemon Newrelic:

Tuer le processus sudo -u ubuntu bash -c bundle exec ./bin/newrelic_aws >> /var/log/newrelic_aws.log 2>&1 il se relancera automatiquement
