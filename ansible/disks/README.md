# Create a new partition

The ansible playbook creates a new partition, formats it, and mounts it.

Example:

```
ansible-playbook partition.yml --extra-vars "blk_dev=nvme0n1 dev=nvme0n1p1 fstype=ext4 path=/home/user/work" 
```

