# boxbilling

Manage billing and client records for an online services business from a self-hosted PHP application. BoxBilling supports invoicing, incoming payments, and client communication for hosting and other online businesses.

## Features

- Automate invoices for services sold through the application.
- Record incoming payments through configured payment gateways.
- Manage client accounts and related communication.
- Integrate with server management software and payment gateways.
- Store application data in MySQL.

## Installation

BoxBilling requires:

- PHP 8.0
- MySQL 8 or a compatible database
- A web server such as Apache, nginx, Lighttpd, or LSWS
- PHP extensions: `pdo_mysql`, `curl`, `zlib`, `gettext`, and `openssl`

To install from source:

```sh
git clone https://github.com/boxbilling/boxbilling.git boxbilling
cd boxbilling
composer install --no-dev --optimize-autoloader
```

Create an empty MySQL database and record its name, username, and password. Configure your web server to use the BoxBilling directory as the site's public directory, then open the site in a browser and follow the installation screen.

For a production installation, download the latest release from the [GitHub releases page](https://github.com/boxbilling/boxbilling/releases/latest). Release archives include the Composer dependencies and can be uploaded to a web server without running Composer there.

Example web server configurations are available for [nginx](https://github.com/boxbilling/boxbilling/blob/master/data/nginx.conf) and [Lighttpd](https://github.com/boxbilling/boxbilling/blob/master/data/lighttpd.conf).

## Usage

For local testing, start PHP's built-in web server from the project directory:

```sh
php -S 127.0.0.1:8080 -t .
```

Open [http://127.0.0.1:8080](http://127.0.0.1:8080) in a browser to continue the web-based setup and use the application.

**Review the security and maintenance status before deploying this software to production.**

## License

This project is licensed under the Apache License 2.0. It is based on [boxbilling/boxbilling](https://github.com/boxbilling/boxbilling), which is also released under Apache-2.0. Preserve the original license and attribution notices when redistributing the project.

