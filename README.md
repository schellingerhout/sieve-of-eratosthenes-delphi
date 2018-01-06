# Sieve-of-Eratosthenes-Delphi
A simple implementation of the Sieve of Erastothenos for finding primes. 

Very fast but memory intensive... can calculate primes up to Max(UInt32). This is the straight forward implementation, optimized as I could find, but the segmented method may allow faster implementation over multiple threads. Fork and contribute if you'd like

For details see https://schellingerhout.github.io/algorithms/sieve-of-eratosthenes/

usage

``` pascal
var
  LMaxValue: UInt32; // Cardinal
  LPrimes: ArrayOfUInt32;
begin
  LMaxValue := 1000000; // all primes up to LMaxValue returned
  LPrimes := TSieveOfEratosthenes.GetPrimes(LMaxValue)
end;
```

There is still quite a bit of optimization to be done. Feel free to fork and issue pull requests for improvements.
