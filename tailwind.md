```sh
$ doas kldload linux64
$ doas pkg install -yr FreeBSD linux_base-rl9
$ doas service linux onestart
$ curl -#LO https://github.com/tailwindlabs/tailwindcss/releases/download/v4.0.13/tailwindcss-linux-arm64
$ chmod +x tailwindcss-linux-arm64
$ brandelf -t Linux tailwindcss-linux-arm64
$ ./tailwindcss-linux-arm64 -h
≈ tailwindcss v4.0.13

Usage:
  tailwindcss [--input input.css] [--output output.css] [--watch] [options…]

Options:
  -i, --input ··········· Input file
  -o, --output ·········· Output file [default: `-`]
  -w, --watch ··········· Watch for changes and rebuild as needed
  -m, --minify ·········· Optimize and minify the output
      --optimize ········ Optimize the output without minifying
      --cwd ············· The current working directory [default: `.`]
  -h, --help ············ Display usage information
```

This will work for amd64 as well, just use s/arm64/x64/ for the above.




### Latest with daisy
https://git.sr.ht/~dch/cacao/commit/e3397d8f#assets/css/app.css
