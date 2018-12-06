

# Coding style and naming standards
- [Coding style and naming standards](#coding-style-and-naming-standards)
    - [Coding style](#coding-style)
        - [PHP](#php)
        - [Visual Basic](#visual-basic)
    - [Naming standards](#naming-standards)
        - [Database structure](#database-structure)
            - [Database name](#database-name)
            - [Table names](#table-names)
            - [Column names](#column-names)

The purpose of this document, is to describe all coding style and namiong agreements we make along the way.  
This is for our own benefit, as well as potential future employees.

## Coding style

### PHP
All PHP code should follow the guidelines defined in [PSR-1](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-1-basic-coding-standard.md) and [PSR-2](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-2-coding-style-guide.md).

Logging should be done using the [PSR-3](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-3-logger-interface.md) interfaces, or Inkpro's own [logging library](https://github.com/InkproDK/php-bigbrother) \(`composer require inkpro/bigbrother`\).

Namespacing and file structure should follow the guildelines defined in [PSR-4](https://github.com/php-fig/fig-standards/blob/master/accepted/PSR-4-autoloader.md) for easy autoloading.

Code should be documented using comments in the [phpDocumenter style](http://manual.phpdoc.org/HTMLSmartyConverter/HandS/phpDocumentor/tutorial_phpDocumentor.quickstart.pkg.html). Make sure the code is as readable as possible, and comment as much as neccesary.

### Visual Basic
On the way!

## Naming standards

### Database structure
#### Database name
Names of databases must be declared using **UpperCamelCase** (or abbreviations, ie. "WMS").

#### Table names
Table names should as a general rule be prefixed with the modulename in **UpperCamelCase**, followed by an underscore and the tablename in **UpperCamelCase**. I.e. `PriceSpider_CrawlErrors`.

#### Column names
Column names should always be defined in **UpperCamelCase**.