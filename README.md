# Linux Infrastructure File Services (NFS & Samba)

This repository documents the setup of a centralized file server using NFS and Samba on Debian.

## Architecture
- **Server:** `172.20.10.3` (Main)
- **Client:** `172.20.10.4` (Clone 1)
- **Shared Directory:** `/home/netadmin/NFSdrive`

## Features
- **NFS:** Exported with `no_root_squash` for administrative access.
- **Samba:** Public (guest access) and Private (authenticated) shares.
- **Samba User:** `sambauser` added to the `smbshare` group.

## Verification
- NFS mounts successfully on the client.
- Samba private share requires authentication.
