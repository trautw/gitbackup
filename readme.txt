mkdir $HOME/.gitbackup
cd $HOME/.gitbackup
git clone git@github.com:trautw/gitbackup || git clone https://github.com/trautw/gitbackup

# In $HOME/.ssh/config
#Host archive
#  Hostname dhcp-christophsair2.sinner-schrader.de
#  Port 9022
#  User git
#  IdentityFile ~/.ssh/archive
#
# Check:
# ssh archive 2>/dev/null | grep gitbackup
# expect:
#  R  	gitbackup

mkdir .gitbackup
cd .gitbackup
git clone archive:gitbackup
