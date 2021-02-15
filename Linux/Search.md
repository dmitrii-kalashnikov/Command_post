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

#### Поиск файлов и поиск по содержимому файлов
- find / -name file1 - найти файлы и директории с именем file1. Поиск начать с корня (/)
- find / -user user1 - найти файл и директорию принадлежащие пользователю user1. Поиск начать с корня (/)
- find /home/user1 -name "*.bin" - Найти все файлы и директории, имена которых оканчиваются на ‘. bin’. Поиск начать с ‘/ home/user1’
- find /usr/bin -type f -atime +100 - найти все файлы в ‘/usr/bin’, время последнего обращения к которым более 100 дней
- find /usr/bin -type f -mtime -10 - найти все файлы в ‘/usr/bin’, созданные или изменённые в течении последних 10 дней
- find / -name *.rpm -exec chmod 755 '{}' \; - найти все фалы и директории, имена которых оканчиваются на ‘.rpm’, и изменить права доступа к ним
- find / -xdev -name "*.rpm" - найти все фалы и директории, имена которых оканчиваются на ‘.rpm’, игнорируя съёмные носители, такие как
cdrom,
floppy и т.п.
- locate "*.ps" - найти все файлы, содержащие в имени ‘.ps’. Предварительно рекомендуется выполнить команду ‘updatedb’
- whereis halt -	показывает размещение бинарных файлов, исходных кодов и руководств, относящихся к файлу ‘halt’
- which halt - отображает полный путь к файлу ‘halt’
