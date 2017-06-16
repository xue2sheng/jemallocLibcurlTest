# Jemalloc Libcurl Test

Dummy performance test on jemalloc / libcurl

See [Jemalloc heap profiling](https://github.com/jemalloc/jemalloc/wiki/Use-Case:-Heap-Profiling) and [Curl example](https://curl.haxx.se/libcurl/c/htmltitle.html)

## Print heap every 10 mega

	export MALLOC_CONF="prof:true,prof_prefix:jeprof.out,lg_prof_interval:10485760"
