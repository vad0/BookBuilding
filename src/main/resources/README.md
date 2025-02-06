We receive price updates from an exchange and want to find situations when best bid price intersects best ask price.
Bid = order for buying an asset.
Ask = order for selling an asset.
If bid price > ask price, then we can buy low (at ask price) and sell high (at bid price).

The data looks as follows.
Price update: {"T":int time, "B":[[int price>0, int size>=0],...], "A":[[price,size],...]}
Top of book {"T":int time, "B":[price,size],"A": [price,size]}

The program has two arguments: path of input file and path of output file. It reads input file similar to input.json, and writes an output file similar to output.json.