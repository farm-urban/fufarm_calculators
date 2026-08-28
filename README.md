# fufarm_calculators
For calculating hydroponic growing parameters

## QR Codes
* [PNG](https://github.com/farm-urban/fufarm_calculators/blob/7e7f781496ba4582c1b6f0e8204d03c86dbdb156/ec_farmurban_qr_qrcodemonkey.png)
* [SVG](https://github.com/farm-urban/fufarm_calculators/blob/7e7f781496ba4582c1b6f0e8204d03c86dbdb156/ec_farmurban_qr_qrcodemonkey.svg)

## Setup
1. Point A record on DNS for subdomain at server (currently ***platform1-katapault*** running Caddy.

2. Serve from Caddy with snippet in: `/etc/caddy/Caddyfile`
    ```
    ec.farmurban.co.uk {
        root * /opt/platforms/fufarm_calculators
        try_files {path} /ec-calculator.html
        file_server
    }
    ```
