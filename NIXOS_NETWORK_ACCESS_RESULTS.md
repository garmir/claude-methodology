=== NIXOS-ENTER NETWORK ENDPOINT TESTING ===
Timestamp: Sun 21 Sep 22:36:11 BST 2025

## Primary NixOS Target (192.168.0.15)
this derivation will be built:
  /nix/store/qbs2ndlkxc1nlcyf4ynhjd34lsnp330x-nixos-install-tools-25.11pre-git.drv
building '/nix/store/qbs2ndlkxc1nlcyf4ynhjd34lsnp330x-nixos-install-tools-25.11pre-git.drv'...
created 7 symlinks in user environment
unshare: mount /proc failed: Operation not permitted

## Network Gateway (192.168.0.1)
unshare: mount /proc failed: Operation not permitted

## NFS Export Tests
clnt_create: RPC: Unable to receive

## NFS Mount Test (192.168.0.15)
this path will be fetched (0.00 MiB download, 0.01 MiB unpacked):
  /nix/store/pz1syacgxmf4q2p3dwmzzg6ag9d8bixa-nfs-utils-2.7.1-dev
copying path '/nix/store/pz1syacgxmf4q2p3dwmzzg6ag9d8bixa-nfs-utils-2.7.1-dev' from 'https://cache.nixos.org'...
clnt_create: RPC: Unable to receive

## Mount Test Results Summary
### WebDAV Mount (Pi-hole)
this path will be fetched (0.13 MiB download, 0.38 MiB unpacked):
  /nix/store/q7s8anpx8qy5f9p4cmg817lqmmd3dq1v-davfs2-1.7.1
copying path '/nix/store/q7s8anpx8qy5f9p4cmg817lqmmd3dq1v-davfs2-1.7.1' from 'https://cache.nixos.org'...
mount: /tmp/webdav-mounts/pihole: must be superuser to use mount.
       dmesg(1) may have more information after failed mount system call.

### NixOS Store Mount (NFS)
mount: /tmp/nixos-store-mounts/target: must be superuser to use mount.
       dmesg(1) may have more information after failed mount system call.

## Sudo-Based Access Attempts
### Sudo nixos-enter (192.168.0.15)
Place your finger on the fingerprint reader
Verification timed out
[sudo] password for a: /nix/store/x46bj1d2vw7s7niqxlawlydyf36wdrr5-nixos-install-tools-25.11pre-git/bin/nixos-enter: '/net/192.168.0.15' is not a NixOS installation

### Sudo NFS Mount (NixOS Store)
[sudo] password for a: mount: /mnt/nixos-remote: fsconfig() failed: NFS: mount program didn't pass remote address.
       dmesg(1) may have more information after failed mount system call.

## Summary Status: Sun 21 Sep 22:38:21 BST 2025
