# ldap20:base
## ASIX M06-ASO @edt Curs 2020-2021

Servidor bàsic ldap, amb organització dc=edt,dc=org,
usuaris bàsics pere, marta, anna...
Configuració client ldap.conf:

	BASE    dc=edt,dc=org
	URI     ldap://ldap.edt.org

Descarregar la imatge:
'docker pull andreupasalamar/ldap20:base'


Executar en mode interactiu:
'docker run --name ldap.edt.org -h ldap.edt.org --net 2hisix -p 389:389 -it andreupasalamar/ldap20:base /bin/bash'

Executar en mode detach:
'docker run --name ldap.edt.org -h ldap.edt.org --net 2hisix -p 389:389 -d andreupasalamar/ldap20:base'
