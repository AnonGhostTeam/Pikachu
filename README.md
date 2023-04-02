# Pikachu

Pikachu is a free and Open source tool available on GitHub. We can perform a denial of service attack using this tool. It’s a framework written in .NET Core. This tool provides many base classes and extensions to use with your daily work. This tool allows a single machine to take down another machine’s web server it uses perfectly legitimate HTTP traffic. It makes a full TCP connection and then requires only a few hundred requests at long-term and regular intervals. As a result, the tool doesn’t need to use a lot of traffic to exhaust the available connections on a server. 

Attack Vector exploited: HTTP Keep Alive + NoCache

## Uses of Pikachu:

Pikachu uses perfectly legitimate HTTP traffic.

Denial of service attack can be executed with the help of Pikachu by generating heavy traffic of botnets.

Pikachu sends multiple requests to the target as a result generates heavy traffic botnets.

Pikachu is an open-source tool, so you can download it from GitHub free of cost.

Pikachu can be used to perform ddos attacks on any webserver.


 USAGE: python3 pikachu.py <url> [OPTIONS]

     OPTIONS:
        Flag           Description                     Default
        -u, --useragents   File with user-agents to use                     (default: randomly generated)
        -w, --workers      Number of concurrent workers                     (default: 50)
        -s, --sockets      Number of concurrent sockets                     (default: 30)
        -m, --method       HTTP Method to use 'get' or 'post'  or 'random'  (default: get)
        -d, --debug        Enable Debug Mode [more verbose output]          (default: False)
        -n, --nosslcheck   Do not verify SSL Certificate                    (default: True)
        -h, --help         Shows this help


## Utilities
* util/pikachu.py - Fetches user-agent lists from http://www.useragentstring.com/pages/useragentstring.php subpages (ex: python3 pikachu.py "http://www.useragentstring.com/pages/useragentstring.php?name=All") *REQUIRES BEAUTIFULSOUP4*
* res/lists/useragents - Text lists (one per line) of User-Agent strings (from http://www.useragentstring.com)

## To-do
* Change from getopt to argparse
* Change from string.format() to printf-like

## License
This software is distributed under the GNU General Public License version 3 (GPLv3).

