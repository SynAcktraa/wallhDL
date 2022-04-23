# wallhDL

> ### An efficient(kinda) scraper which downloads wallpapers from wallhaven.cc 

## Usage

```sh
$ wallhDL [-p <int> | -t <int>] [-s | -l] [-q <query>]
```

## Arguments

   * `-h` show helptext
   * `-p` downloads from head of the query dump
   * `-t` downloads from tail of the query dump
   * `-q` takes query as a parameter
   * `-s` fetches small size image files
   * `-l` fetches full size image files

## Important

>If you encounter an error similar to this:
```bash
./wallhDL: line 2: $'\r': command not found
./wallhDL: line 10: $'\r': command not found
./wallhDL: line 15: $'\r': command not found
./wallhDL: line 20: $'\r': command not found
./wallhDL: line 21: syntax error near unexpected token `$'{\r''
'/wallhDL: line 21: `help_sec () {
```

>Run this command: `sed -i 's_\r$__g' wallhDL` 