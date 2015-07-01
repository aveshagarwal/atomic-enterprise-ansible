# atomic-enterprise-ansible RPM Build instructions
We use tito to make building and tracking revisions easy.

For more information on tito, please see the [Tito home page](http://rm-rf.ca/tito "Tito home page").


## Build atomic-enterprise-ansible-bin
- Change into atomic-enterprise-ansible/bin
```
cd atomic-enterprise-ansible/bin
```
- Build a test package (no tagging needed)
```
tito build --test --rpm
```
- Tag a new build (bumps version number and adds log entries)
```
tito tag
```
- Follow the on screen tito instructions to push the tags
- Build a new package based on the latest tag information
```
tito build --rpm
```


## Build atomic-enterprise-ansible-inventory
- Change into atomic-enterprise-ansible/inventory
```
cd atomic-enterprise-ansible/inventory
```
- Build a test package (no tagging needed)
```
tito build --test --rpm
```
- Tag a new build (bumps version number and adds log entries)
```
tito tag
```
- Follow the on screen tito instructions to push the tags
- Build a new package based on the latest tag information
```
tito build --rpm
```
