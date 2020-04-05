# RLEf_ck
RLE-fied Brainfck converter

Suppose [Brainfck] isn't esoteric enough for your esolang requirements. However, you also happen to be experienced in Brainfck. You notice that there are exactly eight commands in Brainfck. So you decide to encode it in binary with the following table:
|Char|Encode|
|>   |000   |
|<   |010   |
|+   |001   |
|-   |011   |
|[   |100   |
|]   |101   |
|.   |110   |
|,   |111   |
Your code is the following "Hello World" program:
```bf
++++++++[>++++[>++>+++>+++>+<<<<-]>+>+>->>+[<]<-]>>.>---.+++++++..+++.>>.<-.<.+++.------.--------.>>+.>++.
```
The result is the following:
```
010010010010010010010010100000010010010010100000010010000010010010000010010010000010001001001001011101000010000010000011000000010100001101001011101000000110000011011011110010010010010010010010110110010010010110000000110001011110001110010010010110011011011011011011110011011011011011011011011110000000010110000010010110
```

However, suppose this still isn't esoteric enough for your purposes. What can you do?

Run-length encode the program.
```
[0] 1 1 2 1 2 1 2 1 2 1 2 1 2 1 2 1 1 1 6 1 2 1 2 1 2 1 1 1 6 1 2 1 5 1 2 1 2 1 5 1 2 1 2 1 5 1 3 1 2 1 2 1 2 1 1 3 1 1 4 1 5 1 5 2 7 1 1 1 4 2 1 1 2 1 1 3 1 1 6 2 5 2 1 2 1 4 2 1 2 1 2 1 2 1 2 1 2 1 2 1 1 2 1 2 2 1 2 1 2 1 1 2 7 2 3 1 1 4 3 3 2 1 2 1 2 1 1 2 2 2 1 2 1 2 1 2 1 2 1 4 2 2 1 2 1 2 1 2 1 2 1 2 1 2 1 4 8 1 1 2 5 1 2 1 1 2 1
```
_Notes: The `[0]` at the beginning means the first character is a `0`. It isn't necessary to state which character each run is of because there are only two characters and they must alternate._

**Congratulations, you've written your first RLEf*ck program!**

Converters can be found for both conversions [here](hhtps://ezliang.github.io/RLEf_ck/converter.html)
