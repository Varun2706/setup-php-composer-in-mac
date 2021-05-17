# setup-php-composer-in-mac
Step by step process to ready development environment in MAC for PHP based opensource application

To proceed with Composer configuration on Mac, we need to have below dependencies

1.	First we need to install HomeBrew package manger to install packages to their own directory and then symlinks their files into  /user/local.

'ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"'

2.	Check the brew version and confirm if upgrade required

'brew update'

3.	Install Php: There is a inbuilt php configured with mac OS, which can be validated by below command.

'brew tap homebrew/php'

Specific Php version can be install with below commands

'brew install php@7.3'
'brew services start php@7.3'


4.	Install mcrypt 

'brew install mcrypt php70-mcrypt'

5.	 Install Ansible :   required for cloud configuration

'brew install ansible'


6.	Install composer

'brew install composer'

Above command will install latest and if it need to downgrade for project needs, we can be do samewith below commands

'composer self-update 1.10.17'


7. Check all software version

'php -v'
'ansible --version'
'composer --version'
