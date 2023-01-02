# How to get terraform to recognize third party provider

Third-party plugins can be manually installed into the user plugins directory, located at

<tabs>
<tab title="Windows">

`${HOME}/.terraform.d/plugins/registry.terraform.io/`

</tab>
<tab title="Other OSs">

`~/.terraform.d/plugins`

</tab>
</tabs>

Plugins come with executables that have to be placed in the plugin directory.

## Compile executables with Go

In order to build the required executables, install Go first. Then clone this repository and run the following commands inside the cloned repository.

$ export GO111MODULE=on
$ go install github.com/Telmate/terraform-provider-proxmox/cmd/terraform-provider-proxmox
Then create the executables. They are placed in the bin folder inside the repository.

$ cd terraform-provider-proxmox
$ make
Copy executables to plugin directory (Terraform <0.13)
You need to copy these executables to the ~/.terraform.d directory which will also need to have a plugins directory created.

$ mkdir -p ~/.terraform.d/plugins
$ cp -f bin/terraform-provider-proxmox_v2.0.0 ~/.terraform.d/plugins