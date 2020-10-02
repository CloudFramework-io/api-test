# api-test

It allows to run CloudFrameworkTests previously defined in your corporate ERP

```
git clone https://github.com/CloudFramework-io/cloudframework-api-test.git
cd cloudframework-api-test 
```

## Pre-requistes

### Brew
If you do not have Brew installed then install it.
```
/usr/bin/ruby -e "$(curl -fsSL https://raw.githubusercontent.com/Homebrew/install/master/install)"
```

###  php7.3 & Composer
If you do not have php and or composer

```$shell
brew install php@7.3 composer
composer --version   (latest with this doc: 1.10.8)
```

## Run tests

### Install CloudFramework Libraries
```
# First time
composer install

# next times
composer update
```

### Create the following alias
```
alias cftest="php vendor/cloudframework-io/appengine-php-core-7.3/runscript.php"
```

### Execute
Now using the alias to start execute

```
cftest _test/erp/{your-org}
```

To clean-up local data cache
```
cftest _test/clean
```
