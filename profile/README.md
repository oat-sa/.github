# TAO Days

![TAO Days](https://media-exp2.licdn.com/dms/image/sync/C4E34AQELxUJsWXoQJQ/ugc-proxy-shrink_800/0/1652276248497?e=1656320400&v=beta&t=P1k3UrHLYrxUkIDS7iATqo8wKTWUcMxeIVbGdKrjwnU)
***[ > > > Save your seat](https://hubs.ly/Q01b0RT-0)***

# What is TAO?

![TAO Logo](https://github.com/oat-sa/taohub-developer-guide/raw/master/resources/tao-logo.png)

![GitHub](https://img.shields.io/github/license/oat-sa/package-tao.svg)
![GitHub release](https://img.shields.io/github/release/oat-sa/package-tao.svg)

>TAO is an Open Source e-Testing platform that empowers you to build, deliver, and share innovative and engaging assessments online – in any language or subject matter.

TAO ("Computer-Based Testing" or *Testing Assisté par Ordinateur* in French), was created by the University of Luxembourg and is now maintained primarily by [Open Assessment Technologies (OAT)](http://www.taotesting.com/).

TAO is the first commercial-grade Open Source assessment development software on the market. It is QTI and LTI standards-based, and operates under audit-proof transparency. Developers can access the source code for their own test-creating or administering purposes, opening the user to a wide range of potential customizations. Complete ownership of test design has never been this easy; without the restrictions and high costs of proprietary testing, all assessments can easily be displayed with the educational institution's signature details. Furthermore, TAO is fully compatible with just about all of your favorite commercial add-ons.

## Installation

For a detailed documentation of the installation process please visit our Administrator Guide:

- [Prerequisites](https://www.taotesting.com/user-guide/installation-and-upgrade/prerequisites/)
- [Centos, Redhat and Fedora](https://www.taotesting.com/user-guide/installation-and-upgrade/centos-redhat-and-fedora/)
- [MacOS](https://www.taotesting.com/user-guide/installation-and-upgrade/macos/)
- [Ubuntu and Debian](https://www.taotesting.com/user-guide/installation-and-upgrade/ubuntu-and-debian/)
- [Windows](https://www.taotesting.com/user-guide/installation-and-upgrade/windows/)
- [Web Installer](https://www.taotesting.com/user-guide/installation-and-upgrade/web-installer/)

## Other TAO Resources

- [Administrator Guide](https://www.taotesting.com/user-guide/managing-tao/introduction-to-managing-tao/)
- [User Guide](https://www.taotesting.com/user-guide/)
- [Technical Articles](https://github.com/oat-sa/taohub-articles)
- [User Forum](https://www.taotesting.com/forum/)
- [OAT website](https://www.taotesting.com)

## Quickstart

Clone repository

    git clone https://github.com/oat-sa/package-tao.git

Install via composer missing library and extensions.

    composer install

Add rw to www-data

    sudo chown -R www-data package-tao
