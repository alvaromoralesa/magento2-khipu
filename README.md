# Magento 2 Khipu Plugin

khipu payment gateway Magento 2 plugin.

You can sign up for khipu account at <https://khipu.com>

## Development

Plugin:

1. Clone current project into some directory.
2. Create a branch for your changes. In ex: EP-19-magento2---actualizar-plugin-para-.
3. Push the branch with it's changes.

Testing:

1. Have magento2 and php previously installed.
2. Make sure Magento is already running correctly on your system.
2. Install Composer locally on magento2 directory: https://getcomposer.org/download/.
3. Run the following command to integrate library and get latest changes from your development branch:

    ```bash
    php composer.phar require khipu/magento2-khipu:dev-EP-19-magento2---actualizar-plugin-para-
    ```

__Note:__ Please make sure you are using the same php executable instance as Magento, to avoid issues related to system-level dependencies.

## Install via Composer

You can install Magento 2 khipu plugin via [Composer](http://getcomposer.org/). Run the following command in your terminal:

1. Go to your Magento 2 root folder.

2. Enter following commands to install plugin:

    ```bash
    composer require khipu/magento2-khipu
    ```
   Wait while dependencies are updated.

3. Enter following commands to enable plugin:

    ```bash
    php bin/magento module:enable Khipu_Payment --clear-static-content
    php bin/magento setup:upgrade
    ```

4. Enable and configure Khipu plugin in Magento Admin under `Stores / Configuration / Sales / Payment Methods / Khipu`.
