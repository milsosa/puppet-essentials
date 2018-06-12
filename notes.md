# Puppet Setup Notes

## PuppetLabs repos
- yum.puppetlabs.com # RedHat / CentOS
- apt.puppetlabs.com # Ubuntu

## Install puppetlabs rpm repository

- rpm -ihv http://yum.puppetlabs.com/puppetlabs-release-pc1-el-7.noarch.rpm
- rpm -q puppet-agent # See installed package
- update /etc/profile.d/puppet-agent.sh to add /opt/puppetlabs/puppet/bin to PATH env

## Install puppetlabs apt repository

- wget http://apt.puppetlabs.com/puppetlabs-release-pc1-xenial.deb
- apt-get -y update
- apt-get -y puppet-agent

## Puppet directories/paths
- /opt/puppetlabs # Facter
- /etc/puppetlabs/[code/[environments]]
- /etc/puppetlabs/puppet
- /etc/puppetlabs/puppetserver
- /etc/sysconfig/puppet
- /etc/sysconfig/puppetserver