## [bitcoin_wallet][origin_url] project with gradle for android studio

Hello, I tried to build [bitcoin_wallet][origin_url] project without maven using eclipse but it was giving `--core-library` error for `dx - dalvic`.
[See This][stack_url]

So I decided moving to android studio and succeeded to build and here I am sharing .
Gradle version of [bitcoin_wallet][origin_url]

* Don't forget to replace last line of your dx file in `build_tools` directory with 

```sh
exec java $javaOpts -jar "$jarpath" --core-library "$@"
```

[origin_url]: https://github.com/schildbach/bitcoin-wallet "Original Bitcoin Project"
[stack_url]:http://stackoverflow.com/q/28622254/1602333 "Stackoverflow Question"
