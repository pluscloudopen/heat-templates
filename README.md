# Heat Templates
These are Heat template examples to use with OpenStack on the pluscloud open - the data sovereign open source cloud offered by plusserver. They should run on any OpenStack cloud with small adjustments.

Take a look at the image names and instance flavors. They should be available on any SCS compliant CSP, but everywhere else they will likely differ.

They don't claim to be perfect, but they are intended to serve as a good starting point. And you're welcome to provide feedback by opening an issue here on github.

# Templates

- just-one-instance - simple template to start with
- instance-using-user-data - in addition to the first template it will install a nginx
- instance-with-docker - instance with Docker CE
- ghost-cms - installs an instance with nginx, nodejs and Ghost CMS

# For further reading

* [Template Guide](https://docs.openstack.org/heat/latest/template_guide/index.html)
* [Offical OpenStack Heat Documentation](https://docs.openstack.org/heat/latest/)
* [OpenStack Resource Types](https://docs.openstack.org/heat/latest/template_guide/openstack.html)
