# infoblox_ansible

Why is my output sometimes replaced with ********?

Ansible replaces any string marked no_log, including passwords, with ******** in Ansible output. This is done by design, to protect your sensitive data. Most users are happy to have their passwords redacted. However, Ansible replaces every string that matches your password with ********. If you use a common word for your password, this can be a problem. For example, if you choose Admin as your password, Ansible will replace every instance of the word Admin with ******** in your output. This may make your output harder to read. To avoid this problem, select a secure password that will not occur elsewhere in your Ansible output.
