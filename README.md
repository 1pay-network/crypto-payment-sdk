# 1PAY.network - Crypto Payment SDK

Website: [1pay.network](https://1pay.network)

Documents: [1pay.network/documents](https://1pay.network/documents)

This repository is a complete example of setting up Crypto Payment for a website using 1PAY.network

```html
<!DOCTYPE html>
<html>
  <head>
  <title>Example</title>
  </head>
  <body>
  <script src="https://1pay.network/onepay.js?recipient=0x8d70EC40AAd376aa6fD08e4CFD363EaC0AB2c174&network=ethereum,arbitrum,optimism,bsc&token=usdt,usdc,dai"></script>
  <script>
    const onepaySuccess = (PaymentResponse) => {
      console.log(PaymentResponse)
      // (optional)
      // here you can send PaymentResponse to your server
      // then use API Re-check Transaction of 1PAY to verify payment
      // this will improve the security of the payment process
    }
    onepay(0.1, 'usdt', 'example payment')
  </script>
  </body>
</html>
```