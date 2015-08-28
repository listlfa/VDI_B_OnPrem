#**Repo DEPRECATED by https://github.com/listlfa/VDI_OnPrem_B01_PuppEnv/**

# VDI_B_OnPrem
b vdi 01 - total environment

##Steps

###Prepare Puppet

####Puppet Config
1. Confirm Puppet is _old_ enough, eg <=3.6, by `puppet -V`
2. Confirm modulepath has "C:/ProgramData/PuppetLabs/code/environments/production/modules" by `puppet config print modulepath`
    1. Fix with something like `puppet config set modulepath "C:/ProgramData/PuppetLabs/puppet/etc/modules;C:/usr/share/puppet/modules;C:/ProgramData/PuppetLabs/code/environments/production/modules"`
2. Confirm ordering is "manifest" by `puppet config print ordering`
  1. Fix with `puppet config set ordering manifest`

####Puppet Modules
1. Install AD module (includes dependancies)
  1. `puppet module install jriviere-windows_ad`
2. 



