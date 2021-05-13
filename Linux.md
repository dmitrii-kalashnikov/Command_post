#### Getting the Size of a Directory
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
sudo du -sh /var

Output
85G	/var

~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
#### File search ( views.py -the file we are looking for )
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
find ./ -name “views.py”
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### File search ( all files with views in the name )
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
find ./ -name “views.*”
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### File search
 1. rin search in this and all nested directories
 1. i insensitive - large and small letters
 1. n numbers strings
 1. --include= in which files are we looking for
 1. dot means in the current directory
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
grep -rin –include=”*.py” “charfield” .
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### Best file search ( It skips binaries and reads gitignore files and won't look in them )
`Highlighting results`
1. sudo apt update
1. sudo apt install snapd
1.  sudo snap install ripgrep --classic
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
rg -i “target” .
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### All startup
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
systemctl list-dependencies multi-user.target
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### See open ports
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
sudo netstat -pnltu
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### Copy some file from Server to local mashine
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
scp -i "insert key file here" -r "insert ec2 instance here" "your local directory"
scp -i amazon.pem -r ec2-user@ec2-##-##-##:/source/dir /destination/dir
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
