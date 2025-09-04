# Bash FizzBuzz One-Liner

## Overview

This is a concise Bash script that prints the classic FizzBuzz sequence from 1 to 100.  
It outputs:

- "FizzBuzz" for numbers divisible by 15  
- "Buzz" for numbers divisible by 5  
- "Fizz" for numbers divisible by 3  
- The number itself if none of the above conditions are met

## Script


- #!/usr/bin/bash
  for n in {1..100}; do
  ((( n % 15 == 0 )) && echo 'FizzBuzz') ||
  ((( n % 5 == 0 )) && echo 'Buzz') ||
  ((( n % 3 == 0 )) && echo 'Fizz') ||
  echo $n
  done


## Usage

1. Save the script in a file, e.g., `fizzbuzz.sh`  
2. Give execute permissions: `chmod +x fizzbuzz.sh`  
3. Run it: `./fizzbuzz.sh`

## Requirements

- A Unix-like system with Bash shell (version supporting arithmetic evaluation)

## Author

- [Suguro](https://github.com/L1vStr34m)

## License

MIT License
