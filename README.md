# perllib for Dada Mail 

This repository holds the Perl Library that is distributed by default with Dada Mail. 

We distribute a Perl Library (henceforce called, "perllib") with the distribution to make installation of Dada Mail very, very easy, as it is meant to be installed by non-devs. 

There are many disadvantages to this. 

One problem is that this perllib is not well-maintained. Many of the modules are out of date, and knowing which ones need to be updated is a task in of itself. We're hoping putting this in a distribution will help with any future updates of the modules that need to be updated and get code that we don't actually hack on out of the distribution itself.  

Another problem is that there's already CPAN. If you ARE a developer, having a creaky perllib being bundled with the application you're installing may not be optimal. 

The necessary CPAN Perl modules Dada Mail requires can be installed via the Bundle::DadaMailXXL module ala, 

```sh
cpanm Bundle::DadaMailXXL
```
There currently isn't a public build script bundled with the Dada Mail distro. When that's created, one goal is to give you the choice of adding this perllib to the distro, installing Bundle::DadaMailXXL or to do nothing. 

# TODO

This entire perllib needs to be recreated. How? Probably figure out what all the Pure Perl modules are, and make a Bundle::DadaMailPurePerl out of that, then install those locally ala, ,

```
cpanm --force --local-lib ~/perllib Bundle::DadaMailPurePerl
```

clean that up a bit and then THAT's our new perlib to bundle with the Dada Mail distribution. 

# See Also

* Dada Mail 
https://dadamailproject.con 

* The Dada Mail Repository 
https://github.com/justingit/dada-mail/

* Bundle::DadaMail
https://github.com/justingit/Bundle-DadaMail

* Bundle::DadaMail on CPAN 
https://metacpan.org/pod/Bundle::DadaMail

* Bundle::DadaMailXXL
https://github.com/justingit/Bundle-DadaMailXXL

* Bundle::DadaMailXXL on CPAN 
https://metacpan.org/pod/Bundle::DadaMailXXL


