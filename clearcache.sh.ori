#!/bin/bash

echo "Purging cache for homelaber.com.br"

curl -X DELETE "https://api.cloudflare.com/client/v4/zones/d38f5ec0396fbe7d2eba3ae4d8bd5c65/purge_cache" \
-H "X-Auth-Email: homelaber@gmail.com" \
-H "X-Auth-Key: 4ab08cd1214c91d1cd74d454490e313034c9b" \
-H "Content-Type:application/json" \
--data '{"purge_everything":true}'

echo "CloudFlare cache has been cleared"
