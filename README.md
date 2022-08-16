About qemu
==========

Home: https://qemu.org

Package license: GPL-2.0-only

Feedstock license: [BSD-3-Clause](https://github.com/conda-forge/ucb-bar-qemu-feedstock/blob/master/LICENSE.txt)

Summary: QEMU is a generic and open source machine & userspace emulator and virtualizer.

Development: https://github.com/qemu/qemu

Documentation: https://www.qemu.org/support/

QEMU is capable of emulating a complete machine in software without any need for hardware
virtualization support. By using dynamic translation, it achieves very good performance. QEMU
can also integrate with the Xen and KVM hypervisors to provide emulated hardware while allowing
the hypervisor to manage the CPU. With hypervisor support, QEMU can achieve near native
performance for CPUs. When QEMU emulates CPUs directly it is capable of running operating
systems made for one machine (e.g. an ARMv7 board) on a different machine (e.g. an x86_64 PC
board).

QEMU is also capable of providing userspace API virtualization for Linux and BSD kernel
interfaces. This allows binaries compiled against one architecture ABI (e.g. the Linux PPC64
ABI) to be run on a host using a different architecture ABI (e.g. the Linux x86_64 ABI). This
does not involve any hardware emulation, simply CPU and syscall emulation.

QEMU aims to fit into a variety of use cases. It can be invoked directly by users wishing to
have full control over its behaviour and settings. It also aims to facilitate integration into
higher level management layers, by providing a stable command line interface and monitor API. It
is commonly invoked indirectly via the libvirt library when using open source applications such
as oVirt, OpenStack and virt-manager.

QEMU as a whole is released under the GNU General Public License, version 2. For full licensing
details, consult the LICENSE file.


Current build status
====================


<table>
</table>

Current release info
====================

| Name | Downloads | Version | Platforms |
| --- | --- | --- | --- |
| [![Conda Recipe](https://img.shields.io/badge/recipe-qemu-green.svg)](https://anaconda.org/ucb-bar/qemu) | [![Conda Downloads](https://img.shields.io/conda/dn/ucb-bar/qemu.svg)](https://anaconda.org/ucb-bar/qemu) | [![Conda Version](https://img.shields.io/conda/vn/ucb-bar/qemu.svg)](https://anaconda.org/ucb-bar/qemu) | [![Conda Platforms](https://img.shields.io/conda/pn/ucb-bar/qemu.svg)](https://anaconda.org/ucb-bar/qemu) |

Installing qemu
===============

Installing `qemu` from the `ucb-bar` channel can be achieved by adding `ucb-bar` to your channels with:

```
conda config --add channels ucb-bar
conda config --set channel_priority strict
```

Once the `ucb-bar` channel has been enabled, `qemu` can be installed with `conda`:

```
conda install qemu
```

or with `mamba`:

```
mamba install qemu
```

It is possible to list all of the versions of `qemu` available on your platform with `conda`:

```
conda search qemu --channel ucb-bar
```

or with `mamba`:

```
mamba search qemu --channel ucb-bar
```

Alternatively, `mamba repoquery` may provide more information:

```
# Search all versions available on your platform:
mamba repoquery search qemu --channel ucb-bar

# List packages depending on `qemu`:
mamba repoquery whoneeds qemu --channel ucb-bar

# List dependencies of `qemu`:
mamba repoquery depends qemu --channel ucb-bar
```




Updating qemu-feedstock
=======================

If you would like to improve the qemu recipe or build a new
package version, please fork this repository and submit a PR. Upon submission,
your changes will be run on the appropriate platforms to give the reviewer an
opportunity to confirm that the changes result in a successful build. Once
merged, the recipe will be re-built and uploaded automatically to the
`ucb-bar` channel, whereupon the built conda packages will be available for
everybody to install and use from the `ucb-bar` channel.
Note that all branches in the conda-forge/qemu-feedstock are
immediately built and any created packages are uploaded, so PRs should be based
on branches in forks and branches in the main repository should only be used to
build distinct package versions.

In order to produce a uniquely identifiable distribution:
 * If the version of a package **is not** being increased, please add or increase
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string).
 * If the version of a package **is** being increased, please remember to return
   the [``build/number``](https://docs.conda.io/projects/conda-build/en/latest/resources/define-metadata.html#build-number-and-string)
   back to 0.

Feedstock Maintainers
=====================

* [@timsnyder](https://github.com/timsnyder/)

