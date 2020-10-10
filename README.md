# CloudFrameworkTests API-TEST

It allows to run CloudFrameworkTests previously defined in your corporate ERP
* [Designing-API-Tests-from-CloudFramework](https://www.notion.so/cloudframework/Designing-API-Tests-from-CloudFramework-afc8d166610f4b8e98742b98c504053f)

## Pre-requistes for MAC

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


## INSTALLING

```
git clone https://github.com/CloudFramework-io/cloudframework-api-test.git
cd cloudframework-api-test 
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
alias cftest="php vendor/cloudframework-io/appengine-php-core-7.3/runtest.php"
```

### Execute
Now using the alias to start execute

```
cftest erp/{your-org}
```

To clean-up local data cache
```
cftest clean
```

To download the last version of CloudFrameworkTests
```
cftest update
```
