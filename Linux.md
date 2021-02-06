
#### File search (views.py -the file we are looking for)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Find ./ -name “views.py”
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### File search (all files with views in the name)
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Find ./ -name “views.*”
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### File search ( -rin search in this and all nested directories, I insensitive - large and small letters, n numbers strings, --include= in which files are we looking for,dot means in the current directory  )
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Grep -rin –include=”*.py” “charfield” .
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### Best file search (It skips binaries and reads gitignore files and won't look in them)
##### Highlighting results
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
Rg -I “charfield” .
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### All startup
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
systemctl list-dependencies multi-user.target
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~

#### See open ports
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
sudo netstat -pnltu
~~~~~~~~~~~~~~~~~~~~~~~~~~~~~~
