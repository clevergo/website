---
title: "Benchmark"
linkTitle: "Benchmark"
weight: 2
date: 2020-04-08T10:44:52+08:00
---

* Date: 2020/04/05
* Go: 1.14
* [Source](https://github.com/razonyang/go-http-routing-benchmark)

**Lower is better!**

![Benchmark](/img/benchmark.png)

| | Version |
| ---: | --- |
| CleverGo | v1.9.0 |
| Echo | v4.1.16 |
| Gin | v1.6.2 |
| HttpRouter | v1.3.0 |

```text
BenchmarkEcho_Param                     16917187                71.2 ns/op             0 B/op          0 allocs/op
BenchmarkGin_Param                       5957187               210 ns/op              32 B/op          1 allocs/op
BenchmarkHttpRouter_Param               11565042                93.0 ns/op            32 B/op          1 allocs/op
BenchmarkCleverGo_Param                 18139321                65.6 ns/op             0 B/op          0 allocs/op
BenchmarkEcho_Param5                     7405576               165 ns/op               0 B/op          0 allocs/op
BenchmarkGin_Param5                      5316942               211 ns/op              32 B/op          1 allocs/op
BenchmarkHttpRouter_Param5               4284582               272 ns/op             160 B/op          1 allocs/op
BenchmarkCleverGo_Param5                11253404               105 ns/op               0 B/op          0 allocs/op
BenchmarkEcho_Param20                    2382092               511 ns/op               0 B/op          0 allocs/op
BenchmarkGin_Param20                     2697861               438 ns/op              32 B/op          1 allocs/op
BenchmarkHttpRouter_Param20              1312308               910 ns/op             640 B/op          1 allocs/op
BenchmarkCleverGo_Param20                4401469               270 ns/op               0 B/op          0 allocs/op
BenchmarkEcho_ParamWrite                 7462525               166 ns/op               8 B/op          1 allocs/op
BenchmarkGin_ParamWrite                  5503063               224 ns/op              32 B/op          1 allocs/op
BenchmarkHttpRouter_ParamWrite           9790910               124 ns/op              32 B/op          1 allocs/op
BenchmarkCleverGo_ParamWrite            12461090                98.7 ns/op             0 B/op          0 allocs/op
BenchmarkEcho_GithubStatic              12125133                98.0 ns/op             0 B/op          0 allocs/op
BenchmarkGin_GithubStatic                6702390               178 ns/op              32 B/op          1 allocs/op
BenchmarkHttpRouter_GithubStatic        31478012                38.1 ns/op             0 B/op          0 allocs/op
BenchmarkCleverGo_GithubStatic          18279379                63.8 ns/op             0 B/op          0 allocs/op
BenchmarkEcho_GithubParam                6818716               177 ns/op               0 B/op          0 allocs/op
BenchmarkGin_GithubParam                 5673768               217 ns/op              32 B/op          1 allocs/op
BenchmarkHttpRouter_GithubParam          5217598               230 ns/op              96 B/op          1 allocs/op
BenchmarkCleverGo_GithubParam            9384177               122 ns/op               0 B/op          0 allocs/op
BenchmarkEcho_GithubAll                    34786             34050 ns/op               0 B/op          0 allocs/op
BenchmarkGin_GithubAll                     26689             45883 ns/op            6496 B/op        203 allocs/op
BenchmarkHttpRouter_GithubAll              26613             43546 ns/op           13792 B/op        167 allocs/op
BenchmarkCleverGo_GithubAll                48681             24564 ns/op               0 B/op          0 allocs/op
BenchmarkEcho_GPlusStatic               18314020                66.9 ns/op             0 B/op          0 allocs/op
BenchmarkGin_GPlusStatic                 7336438               165 ns/op              32 B/op          1 allocs/op
BenchmarkHttpRouter_GPlusStatic         50243390                23.3 ns/op             0 B/op          0 allocs/op
BenchmarkCleverGo_GPlusStatic           24276782                48.1 ns/op             0 B/op          0 allocs/op
BenchmarkEcho_GPlusParam                12441846                97.5 ns/op             0 B/op          0 allocs/op
BenchmarkGin_GPlusParam                  6299746               195 ns/op              32 B/op          1 allocs/op
BenchmarkHttpRouter_GPlusParam           7702280               151 ns/op              64 B/op          1 allocs/op
BenchmarkCleverGo_GPlusParam            13458559                92.2 ns/op             0 B/op          0 allocs/op
BenchmarkEcho_GPlus2Params               7924144               152 ns/op               0 B/op          0 allocs/op
BenchmarkGin_GPlus2Params                5417515               222 ns/op              32 B/op          1 allocs/op
BenchmarkHttpRouter_GPlus2Params         6396112               179 ns/op              64 B/op          1 allocs/op
BenchmarkCleverGo_GPlus2Params          10868599               109 ns/op               0 B/op          0 allocs/op
BenchmarkEcho_GPlusAll                    747770              1561 ns/op               0 B/op          0 allocs/op
BenchmarkGin_GPlusAll                     660558              2500 ns/op             416 B/op         13 allocs/op
BenchmarkHttpRouter_GPlusAll              609037              2017 ns/op             640 B/op         11 allocs/op
BenchmarkCleverGo_GPlusAll                944690              1224 ns/op               0 B/op          0 allocs/op
BenchmarkEcho_ParseStatic               17630368                69.1 ns/op             0 B/op          0 allocs/op
BenchmarkGin_ParseStatic                 7404474               166 ns/op              32 B/op          1 allocs/op
BenchmarkHttpRouter_ParseStatic         50948972                22.8 ns/op             0 B/op          0 allocs/op
BenchmarkCleverGo_ParseStatic           23951481                47.8 ns/op             0 B/op          0 allocs/op
BenchmarkEcho_ParseParam                14224027                82.4 ns/op             0 B/op          0 allocs/op
BenchmarkGin_ParseParam                  6667672               186 ns/op              32 B/op          1 allocs/op
BenchmarkHttpRouter_ParseParam           8803288               144 ns/op              64 B/op          1 allocs/op
BenchmarkCleverGo_ParseParam            14893399                79.9 ns/op             0 B/op          0 allocs/op
BenchmarkEcho_Parse2Params               9941707               113 ns/op               0 B/op          0 allocs/op
BenchmarkGin_Parse2Params                5996330               211 ns/op              32 B/op          1 allocs/op
BenchmarkHttpRouter_Parse2Params         7428163               159 ns/op              64 B/op          1 allocs/op
BenchmarkCleverGo_Parse2Params          13746112                90.4 ns/op             0 B/op          0 allocs/op
BenchmarkEcho_ParseAll                    433760              2672 ns/op               0 B/op          0 allocs/op
BenchmarkGin_ParseAll                     246598              5553 ns/op             832 B/op         26 allocs/op
BenchmarkHttpRouter_ParseAll              461934              2782 ns/op             640 B/op         16 allocs/op
BenchmarkCleverGo_ParseAll                554302              2046 ns/op               0 B/op          0 allocs/op
BenchmarkEcho_StaticAll                    49604             24031 ns/op               0 B/op          0 allocs/op
BenchmarkGin_StaticAll                     32766             36923 ns/op            5024 B/op        157 allocs/op
BenchmarkHttpRouter_StaticAll             111400             10195 ns/op               0 B/op          0 allocs/op
BenchmarkCleverGo_StaticAll                75066             15577 ns/op               0 B/op          0 allocs/op
```