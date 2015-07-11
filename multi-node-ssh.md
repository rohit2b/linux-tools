Command to execute same command across multiple nodes over ssh

For example, this will execute 'cat /etc/hosts' across the following node hostnames:
* hostname-1
* hostname-2
* hostname-3
* hostname-4

''' bash
for COUNT in 1 2 3 4
do
	ssh -i gce-key hostname-$COUNT "cat /etc/hosts"
done
'''
