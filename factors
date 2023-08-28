#!/usr/bin/python3

import sys

def factorize(n):
    for i in range(2, n):
        if n % i == 0:
            return i, n // i
    return None, None

def main(file_path):
    with open(file_path, 'r') as file:
        for line in file:
            n = int(line.strip())
            p, q = factorize(n)
            if p is not None and q is not None:
                print("{}={}*{}".format(n, p, q))

if __name__ == "__main__":
    if len(sys.argv) != 2:
        print("Usage: factors <file>")
        sys.exit(1)

    file_path = sys.argv[1]
    main(file_path)
