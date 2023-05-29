# Codec Special Interest Group

SIG Codec is responsible for the components for structure data encode and decode.

The [charter](charter.md) defines the scope and governance of the Codec Special Interest Group.

## Leadership

### Chairs
The Chairs of the SIG run operations and processes governing the SIG.

* Dong Jiang (**[@dongjiang1989](https://github.com/dongjiang1989)**), Chinamobile

### Technical Leads
The Technical Leads of the SIG establish new subprojects, decommission existing
subprojects, and resolve cross-subproject technical issues and decisions.

* Dong Jiang (**[@dongjiang1989](https://github.com/dongjiang1989)**), Chinamobile
* Zhou Zhenling (**[@zhouzhenling](https://github.com/zhouzhenling)**), Meituan

## Contact
- [Open Community Issues/PRs](https://github.com/kubeservice-stack/Community/blob/main/sig-scheduling)
- GitHub Teams:
    - @kubeservice-stack/sig-codec-reviews - Library Changes and Reviews
	- @kubeservice-stack/sig-codec-bugs - Bug Triage and Troubleshooting
	- @kubeservice-stack/sig-codec-feature-requests - Feature Requests

## Motivation

To reach higher levels of success requires a `comprehensive toolkit` for `coherent distributed programming at scale`. The `Codec Library` is a set of `packages and best practices` that provide a `comprehensive`, `robust` and `trusted` support for building services for organizations of any size.

`Localization support` is also one of it's biggest features.

## Goal

Build a fairly `complete`, `out-of-the-box` Package Collection

- Each package is opposite to each other and can be used as needed
- Reduce external version dependencies, self-shaped ecology
- No business logic, fully open basic capabilities
- No mandatory requirements for specific tools or techniques

## Blueprint

### Self-developed serialization library

Self-developed Codec library, high Performance and high Compatibility.

### High Performance and Scalability
base on 
- Go 1.19.4
- MacPro Apple M2 8G macOS Ventura
- Darwin 192.168.1.7 22.2.0 Darwin Kernel Version 22.2.0: Fri Nov 11 02:06:26 PST 2022; root:xnu-8792.61.2~4/RELEASE_ARM64_T8112 arm64

benchmark Results with
```
goos: darwin
goarch: amd64
pkg: github.com/kubeservice-stack/serialization-benchmarks
cpu: VirtualApple @ 2.50GHz
Benchmark_Bson_Marshal-8         	 2272702	       499.2 ns/op	       110.0 B/serial	     376 B/op	      10 allocs/op
Benchmark_Bson_Unmarshal-8       	 1617357	       716.2 ns/op	       110.0 B/serial	     224 B/op	      19 allocs/op
Benchmark_FastJson_Marshal-8     	 4016576	       296.9 ns/op	       133.8 B/serial	     504 B/op	       6 allocs/op
Benchmark_FastJson_Unmarshal-8   	 1527366	       778.7 ns/op	       133.8 B/serial	    1704 B/op	       9 allocs/op
Benchmark_Gob_Marshal-8          	  467408	      2475 ns/op	       163.6 B/serial	    1616 B/op	      35 allocs/op
Benchmark_Gob_Unmarshal-8        	   95322	     12386 ns/op	       163.6 B/serial	    7688 B/op	     207 allocs/op
Benchmark_JsonIter_Marshal-8     	 1941692	       591.5 ns/op	       148.7 B/serial	     216 B/op	       3 allocs/op
Benchmark_JsonIter_Unmarshal-8   	 1307601	       871.8 ns/op	       148.7 B/serial	     359 B/op	      14 allocs/op
Benchmark_Json_Marshal-8         	 1406618	       850.8 ns/op	       148.6 B/serial	     208 B/op	       2 allocs/op
Benchmark_Json_Unmarshal-8       	  494430	      2153 ns/op	       148.6 B/serial	     399 B/op	       9 allocs/op
Benchmark_xxxPack_Marshal-8      	 3624224	       312.8 ns/op	       119.0 B/serial	     344 B/op	       6 allocs/op
Benchmark_xxxPack_Unmarshal-8    	 2070897	       574.7 ns/op	       119.0 B/serial	     112 B/op	       3 allocs/op
Benchmark_Msgpack_Marshal-8      	 2961548	       401.9 ns/op	        92.00 B/serial	     264 B/op	       4 allocs/op
Benchmark_Msgpack_Unmarshal-8    	 2209035	       536.9 ns/op	        92.00 B/serial	     160 B/op	       4 allocs/op
PASS
ok  	github.com/kubeservice-stack/serialization-benchmarks	23.928s
```

### Muti language support

support `java`, `golang`, `rust`, `c/c++`

## Subprojects

TODO