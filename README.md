## WordPress+Nginx+PHP-FPM Deployment

- Requires Ansible 1.2 or newer
- Expects CentOS/RHEL 6.x hosts

These playbooks deploy a simple all-in-one configuration of the popular
WordPress blogging platform and CMS, frontend by the Nginx web server and the
PHP-FPM process manager. To use, copy the `hosts.example` file to `hosts` and 
edit the `hosts` inventory file to include the names or URLs of the servers
you want to deploy.

Then run the playbook, like this:

	ansible-playbook -i my_hosts site.yml

The playbooks will configure MySQL, WordPress, Nginx, and PHP-FPM. When the run
is complete, you can hit access server to begin the WordPress configuration.
