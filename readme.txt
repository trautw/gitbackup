mkdir $HOME/.gitbackup
cd $HOME/.gitbackup
git clone https://github.com/trautw/gitbackup.git --depth 1

# In $HOME/.ssh/config
Host archive
  Hostname archive.szz.chtw.de
  Port 9022
  User git
  IdentityFile ~/.ssh/archive
  ForwardX11 no
  StrictHostKeyChecking no
  UserKnownHostsFile=/dev/null
  LogLevel ERROR

# Check:
# ssh archive 2>/dev/null | grep gitbackup
# expect:
#  R  	gitbackup

