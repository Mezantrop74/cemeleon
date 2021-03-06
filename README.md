# Cemelon

**The tool collects address used in the bitcoin blockchain!**

## Usage of cemelon

~~~
Usage of ./cemelon:
  -e int
        The block number on which program finished collecting the addresses including this number (default -1)
  -m int
        The number of addresses stored in the card to prevent re-entry of addresses (default 262144)
  -n int
        The number of threads downloading data (default 1)
  -o string
        Output data file base name (default "cemelon.txt")
  -r    Not to collect the first address in the block
  -s int
        The block number at which to start collecting addresses (default -1)
  -z    Not to collect all addresses
~~~

## Dependencies

Install go packages:

```bash
go get github.com/vasilyukvasiliy/blockchain
```

## Scripts

 * **top100bitcoin-richest.sh** - Allows you to collect top 10,000 richest Bitcoin and Bitcoin Cash addresses

## Example of the execution log

```log
#######################################################
#                                                     #
#   #####                                             #
#  #     # ###### #    # ###### #       ####  #    #  #
#  #       #      ##  ## #      #      #    # ##   #  #
#  #       #####  # ## # #####  #      #    # # #  #  #
#  #       #      #    # #      #      #    # #  # #  #
#  #     # #      #    # #      #      #    # #   ##  #
#   #####  ###### #    # ###### ######  ####  #    #  #
#                                                     #
#  The MIT License (MIT)                              #
#  Copyright (с) 2017-2018 Vasiliy Vasilyuk               #
#  Email: vasilyukvasiliy@gmail.com                   #
#######################################################
#            Github: https://git.io/vNIKR             #
#######################################################


cemelon -s 300000 -e 300010 -n 2
Mon, 01 Jan 2018 10:31:48 UTC | Block index:  300000
Mon, 01 Jan 2018 10:31:48 UTC | Block index:  300005
Mon, 01 Jan 2018 10:31:49 UTC | Block index:  300006
Mon, 01 Jan 2018 10:31:50 UTC | Block index:  300007
Mon, 01 Jan 2018 10:31:50 UTC | Block index:  300001
Mon, 01 Jan 2018 10:31:53 UTC | Block index:  300008
Mon, 01 Jan 2018 10:31:54 UTC | Block index:  300009
Mon, 01 Jan 2018 10:31:56 UTC | Block index:  300010
```


## License

The MIT License ([MIT](https://git.io/vNI0r))