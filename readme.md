# loadprofile - a simple linux profile loader

### Manage your profile in git and let it load by the profile loader

## Usage
loadprofile supports the following dir tree:
```
+$HOME/
 + profile/
   + profile.d/
     + 001_java_env.sh
     + 002_go_env.sh
   + DOTssh/
     + mykey.id_rsa
   + DOTpg/
     + ...
```

* Folders/files DOTabc below $HOME/profile/ are linked to your home directory.
* Snippets form $HOME/profile/profile.d/ are loaded on login.

## Installation

* Download loadprofile
```
mkdir -p $HOME/bin && \
curl -o $HOME/bin/loadprofile https://raw.githubusercontent.com/cbuschka/loadprofile/master/loadprofile && \
chmod +x $HOME/bin/loadprofile
```

* Add loadprofile to your .bash_profile or .profile
```
source $HOME/bin/loadprofile
```

* Create a folder profile in your $HOME
```
mkdir -p $HOME/profile && chmod 700 $HOME/profile
```

* Add DOT folders/files and mixins

## License

[MIT](license)
