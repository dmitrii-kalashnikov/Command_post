
#### File search (views.py -the file we are looking for)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
find ./ -name “views.py”
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### File search (all files with views in the name)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
find ./ -name “views.*”
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### File search ( -rin search in this and all nested directories, I insensitive - large and small letters, n numbers strings, --include= in which files are we looking for,dot means in the current directory  )
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
grep -rin –include=”*.py” “charfield” .
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### Best file search (It skips binaries and reads gitignore files and won't look in them)
##### Highlighting results
##### sudo apt update
##### sudo apt install snapd
##### sudo snap install ripgrep --classic
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
