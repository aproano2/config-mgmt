# Create a new partition

The ansible playbook creates a new partition, formats it, and mounts it.

Example:

```
ansible-playbook -K -i inventory partition.yml --extra-vars "blk_dev=/dev/nvme0n1 dev=/dev/nvme0n1p1 fstype=ext4 path=/home/user/work"
ansible-playbook -K -i inventory delete_partition.yml --extra-vars "blk_dev=/dev/nvme0n1 dev=/dev/nvme0n1p1 number=1 path=/home/user/work" 
```

