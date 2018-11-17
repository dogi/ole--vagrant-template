How to create vagrant boxes

```sh
vagrant cloud auth login
vagrant destroy -f
rm template.log

vagrant up |& tee template.log
vagrant halt
vagrant package --output ole-0.5.4.box
```

upload the new box to https://app.vagrantup.com/ole/boxes/stretch64
