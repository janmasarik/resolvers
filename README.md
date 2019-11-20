# resolvers.txt
List of periodically validated public DNS resolvers.
 
```bash
$ wget https://raw.githubusercontent.com/janmasarik/resolvers/master/resolvers.txt
$ massdns -r resolvers.txt domains_to_resolve.txt
```

## Why?
People need a list of *good* resolvers (e.g. for [massdns](https://github.com/blechschmidt/massdns)). Why spend all that traffic on refreshing a private list? Let's use and improve this one! ᕕ( ᐛ )ᕗ

## How it's done 
Validation is done using [dnsvalidator](https://github.com/vortexau/dnsvalidator/) on https://public-dns.info/nameservers.txt every 24 hours using **Github Actions** that push the fresh results back to this repository. 

## Thanks
- [@vortexau](https://twitter.com/vortexau) and [@codingo_](https://twitter.com/codingo_) for creating [dnsvalidator](https://github.com/vortexau/dnsvalidator)!
- GitHub for *hosting* this on GitHub Actions! :heart:
