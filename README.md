# Specify Web Portal Ansible playbook

## Instructions

1) Get the database export archive from Specify.

2) Move the solr directory and flds.json into the files directory.

3) Make any necessary changes from PortalInstanceSetting.json in files/settings.json.

4) Remove all the fields from <fields> in files/schema.xml and copy and paste the fields from SolrFldSchema.xml.

5) Make sure the server is setup in /etc/ansible/hosts.

6) Make sure the public key is on the hosts.

7) Run:
`ansible-playbook playbook.yml`
