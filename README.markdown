## Usage Note

Because of browser [security limitations](http://en.wikipedia.org/wiki/Same_origin_policy), you can't just up-and-use Giles directly from Github's server, sigh.

Two options:

1. `git clone git://github.com/rentzsch/giles.git` and run it locally off your file system.

2. Copy Giles to your DBSlayer server and have DBSlayer vend it like so:

		dbslayer -c /etc/mysql/my.cnf -s slayer -b /path/to/giles

	Then access Giles at

		http://slayer.example.com/index.html

In the future there's a low probability I'll fork DBSlayer and add JSONP support, but this in general seems like a bad idea since DBSlayer should never be exposed to the public Net.