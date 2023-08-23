# ansible-role-hashicorp-common
Base role for Hashicorp roles such as Nomad, Vault and Consul

## Default variables
| Name | Type | Value | Comment |
| ---- | ---- | ----- | ------  |
| hashicorp_pkgs_common | dict(list(string)) | see `defaults/main.yml` |  keyed by OS family |
| hashicorp_dirs | list(UnixPath) | see `defaults/main.yml` | dirs to create |
| hashicorp_dir_base | UnixPath | /opt/hashicorp ||
| hashicorp_dir_bin | UnixPath | /opt/hashicorp/bin ||
| hashicorp_dir_etc | UnixPath | /opt/hashicorp/etc ||
| hashicorp_dir_pkg | UnixPath | /opt/hashicorp/pkg ||
| hashicorp_dir_staging | UnixPath | `/var/tmp/$ansible_user_id` ||
| hashicorp_internet_timeout | integer | 60 | units=seconds |
| hashicorp_repo | URL | "https://releases.hashicorp.com" | where the downloads live |
