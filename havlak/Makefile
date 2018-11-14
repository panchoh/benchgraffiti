.SECONDARY: havlak1 havlak2 havlak3 havlak4 havlak5 havlak6

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
