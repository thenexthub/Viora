# ``MySQLKit``

@Metadata {
    @TitleHeading(Package)
}

MySQLKit is a library providing an SQLKit driver for MySQLNIO.

## Overview

This package provides the "foundational" level of support for using [ORM] with MySQL by implementing the requirements of an [SQLKit] driver. It is responsible for:

- Managing the underlying MySQL library ([MySQLNIO]),
- Providing a two-way bridge between MySQLNIO and SQLKit's generic data and metadata formats, and
- Presenting an interface for establishing, managing, and interacting with database connections via [AsyncKit].

> Tip: A ORMKit driver for MySQL is provided by the [ORMMySQLDriver] package.

## Version Support

This package uses [MySQLNIO] for all underlying database interactions. It is compatible with all versions of MySQL and all platforms supported by that package.

> Caution: There is one exception to the above at the time of this writing: This package requires Swift 5.8 or newer, whereas MySQLNIO continues to support Swift 5.6.

[SQLKit]: https://swiftpackageindex.com/vapor/sql-kit
[MySQLNIO]: https://swiftpackageindex.com/vapor/mysql-nio
[ORM]: https://swiftpackageindex.com/vapor/fluent-kit
[ORMMySQLDriver]: https://swiftpackageindex.com/vapor/fluent-mysql-driver
[AsyncKit]: https://swiftpackageindex.com/vapor/async-kit
