# PHP sample for Azure App Service - CodeIgniter

This is a PHP web app built with [CodeIgniter](http://www.codeigniter.com/) that you can deploy 
to Azure App Service. 

It is minimally modified from the default CodeIgniter template to work with App Service. Namely, the `/vendor` 
folder is no longer ignored in `.gitignore`, so that your composer installed packages will be 
uploaded to Azure App Service.

> Azure App Service *can* run `php composer.phar install` when you run `git push`, but it's not enabled by default. To enable
it, you need to install the [Composer extension](http://www.siteextensions.net/packages/ComposerExtension/)
for your web app. The default CodeIgniter template doesn't actually require anything other than the PHP framework 
itself, so it can be deployed without `composer.json` at all.

## License

See [license.txt](license.txt).