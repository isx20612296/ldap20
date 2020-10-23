# ldap20:acl

isx20612296@edt 
ASIX M06-ASO

access to * by * read
access to * by * write
access to * 
	by self write 
	by * read

access to *
        by * read
        by self write

access to attrs=homePhone by * read
access to * by * write

access to * by * write
access to attrs=homePhone by * read

access to attrs=homePhone
	by dn.exact="cn=Anna Pou,ou=usuaris,dc=edt,dc=org" write
	by * read
access to * by * write

access to attrs=homePhone
	by dn.exact="cn=AnnaPou,ou=usuaris,dc=edt,dc=org" write
access to attrs=homePhone
	by * read
access to * by * write

access to attrs=homePhone
	by dn.exact="cn=Anna Pou,ou=usuaris,dc=edt,dc=org"
	by dn.exact="cn=Admin System,ou=usuaris,dc=edt,dc=org"
	by * read
access to *
	by dn.exact="cn=Admin System,ou=usuaris,dc=edt,dc=org" write
	by self write
	by * read

access to attrs=userPassword
	by self write
access to * by * read
