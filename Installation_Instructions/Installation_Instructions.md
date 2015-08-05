#How to Install OroCRM Amazon Integration






![Installation](img/package_manager.png)

3. Re-enter your OroCRM credentials to verify your permissions
![Installation](img/installed_packages.png)
5. The **Available Packages** screen opens. You can find all the packages available for installation here. In this example we are looking for **eltrino/orocrm-amazon-bundle**. After you find it, click **Install** to initiate installation process.
![Installation](img/install.png)
![Installation](img/notification.png)
![Installation](img/success.png)

###Installation via Composer

Add as dependency in composer:

```composer require eltrino/orocrm-amazon-bundle:1.0.2```

For this bundle to function properly, clear cache by issuing the following command:

```php app/console cache:clear --no-warmup```

Then execute a platform update:

```php app/console oro:platform:update --force --timeout=0```


######Amazon Transport Configuration

For the proper transport configuration please refer to [Amazon MWS Developer Guide](https://images-na.ssl-images-amazon.com/images/G/02/mwsportal/doc/en_US/bde/MWSDeveloperGuide._V327338421_.pdf). You can find proper configuration for Endpoints and Marketplace IDs in this manual.