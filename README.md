# cubeSQL Python2 Cleint

Simple Python 2.x JSON client for the [cubeSQL](http://www.sqlabs.com/cubesql.php) database server.

## Usage example

See `Examples/simple.py` for a simple example.

```py
import cubesql

cube = cubesql.CubeSQL( 'localhost', "loginname", "password" )
cube.use( "test" )

cube.execute( "INSERT INTO Log VALUES ( DATETIME( 'now', 'localtime' ), '127.0.0.1' , 'request...' );" );

d = cube.select( "SELECT * FROM Log;" );
print( d )
```

## Donate

- [Patreon](https://www.patreon.com/andreas_pfeil)
- [PayPal](https://www.paypal.com/paypalme/PfeilAndreas/10.00EUR)

## Contributors

- [Andreas Pfeil](https://github.com/andreaspfeil)

## Acknowledgments

- [sqlabs](https://sqlabs.com)
- [cubeSQL](https://sqlabs.com/cubesql)
- [Marco Bambini](https://github.com/marcobambini)

## See also

- [cubeSQL for Python3](https://github.com/andreaspfeil/CubeSQL.Python3)
- [cubeSQL für .NET](https://github.com/andreaspfeil/CubeSQL.NET)

## License

BEER license / MIT license