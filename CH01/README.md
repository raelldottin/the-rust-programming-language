# The Rust Programming Language
# Steve Klabnik, Carol Nichols, Contributions from the Rust Community
# This material may be protected by copyright. The Rust Programming Language

##  Installation
```console
$ curl --proto '=https' --tlsv1.2 https://sh.rustup.rs -sSf | sh”

```
The rustup command can used to install and manage rust installations.
The curl command sownloads a script and the sh command runs the script which installs the rustup tool and rust.


```console
$ xcode-select --install
```
On macos, install the C compiler by installing xcode command line tools.


## Troubleshooting
```console
$ rustc --version
rustc x.y.z (abcabcabc yyyy-mm-dd
```
The rustc command will display the version number if Rust is installed correctly.

# Updating
```console
$ rustup update
```
This command will update Rust if it was installed via rustup.

# Uninstalling
```console
$ rustup self uninstall
```
This command will uninstall Rust and the rustup script

# Local Documentation
```console
$ rustup doc
```
This command will open the local documentation in your web browser.


