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
