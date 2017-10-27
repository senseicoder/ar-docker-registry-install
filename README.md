# Usage

roles:
  - ar-docker-registry-install

note: docker doit être déjà installé, et la registry doit être installée avant que les autres machines Docker ne soient installées (elles vont récupérer le certificat auto-généré).

Dépose dans le certificat et sa clef dans 
* pathcrt: /etc/docker/certs.d/registry.crt
* pathkey: /etc/docker/certs.d/registry.key

# variables à surcharger

* docker_registry_img_name: registry
* docker_registry_img_tag: 2
* docker_registry_img_load_dir: /etc/docker/images
* pathphpscript_cleanupsrcdocker: /docker_list_srccleanup.php

# Todo
