havlak%cc: havlak%.cc
	g++ -O3 -o havlak$*cc havlak$*.cc

havlak%: havlak%.go
	go build havlak$*.go

%.time: %
	./xtime ./$*

havlak%.prof: havlak%
	./havlak$* -cpuprofile=$@

havlak%.mprof: havlak%
	./havlak$* -memprofile=$@
