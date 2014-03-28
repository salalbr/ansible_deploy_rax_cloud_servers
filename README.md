Name: ansible_deploy_rax_cloud_servers

Synopsis:
Creates a Rackspace Public Cloud instance according to variables define in 'group_vars/all.yml'.

Example:
# ansible-playbook play_build_cloud_server.yml -l local

PLAY [Build a Cloud Server] *************************************************** 

TASK: [Server build request] ************************************************** 
changed: [127.0.0.1]

TASK: [Add the instances we created (by public IP) to the group 'raxhosts'] *** 
ok: [127.0.0.1] => (item={u'rax_progress': 0, u'rax_links': [{u'href': u'https://iad.servers.api.rackspacecloud.com/v2/<ID>/servers/<GUIID>', u'rel': u'self'}, {u'href': u'https://iad.servers.api.rackspacecloud.com/<ID>/servers/<GUID>', u'rel': u'bookmark'}], u'id': u'<GUID>', u'rax_accessipv6': u'', u'rax_human_id': u'<SERVERNAME>', u'rax_os-ext-sts_task_state': u'scheduling', u'accessIPv4': u'', u'rax_os-ext-sts_vm_state': u'building', u'rax_flavor': {u'id': u'performance1-2', u'links': [{u'href': u'https://iad.servers.api.rackspacecloud.com/<ID>/flavors/performance1-2', u'rel': u'bookmark'}]}, u'rax_accessipv4': u'', u'rax_id': u'<GUID>', u'rax_created': u'2014-03-28T07:02:29Z', u'rax_os-ext-sts_power_state': 0, u'rax_hostid': u'', u'rax_name_attr': u'name', u'rax_adminpass': u'<password>', u'rax_key_name': None, u'status': u'BUILD', u'rax_name': u'<SERVERNAME>', u'rax_metadata': {u'group': u'<SERVERGROUP>'}, u'rax_networks': {}, u'rax_addresses': {}, u'rax_image': {u'id': u'<GUID>', u'links': [{u'href': u'https://iad.servers.api.rackspacecloud.com/<ID>/images/<GUID>', u'rel': u'bookmark'}]}, u'rax_user_id': u'<GUID>', u'rax_updated': u'2014-03-28T07:02:29Z', u'rax_config_drive': u'', u'rax_os-dcf_diskconfig': u'MANUAL', u'rax_status': u'BUILD', u'name': u'<SERVERNAME>', u'rax_tenant_id': u'<ID>'})
