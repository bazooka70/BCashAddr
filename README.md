# BCashAddr
C# implementation of the cashaddr and copay Bitcoin Cash address formats

## References:

https://github.com/bitcoincashjs/cashaddrjs/ 

https://github.com/bitcoincashjs/bchaddrjs/

## Usage:

```
BchAddrData bchAddr = BchAddr.DecodeAddress("CTH8H8Zj6DSnXFBKQeDG28ogAS92iS16Bp");
var legacy = bchAddr.AsLegacyAddress; // 1BpEi6DfDAUFd7GtittLSdBeYJvcoaVggu
var bitpay = bchAddr.AsBitpayAddress; // CTH8H8Zj6DSnXFBKQeDG28ogAS92iS16Bp
var cashaddr = bchAddr.AsCashaddrAddress; // bitcoincash:qpm2qsznhks23z7629mms6s4cwef74vcwvy22gdx6a
var cashaddrNoPrefix = bchAddr.AsCashaddrAddressNoPrefix; // qpm2qsznhks23z7629mms6s4cwef74vcwvy22gdx6a

Console.WriteLine(
  $"legacy: {legacy}\r\n" +
  $"bitpay: {bitpay}\r\n" +
  $"cashaddr: {cashaddr}\r\n" +
  $"cashaddrNoPrefix: {cashaddrNoPrefix}");
 
```

## Prerequisite:

NBitcoin: https://github.com/MetacoSA/NBitcoin

## See also:

[Bitcoin Cash Address Converter (online)](https://cashaddr.bitcoincash.org/)
