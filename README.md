# polar-cookieParser

Clone of Express/Connect cookieParser that filters cookies by domain.

RFC 6265 defines no order for cookie parsing, web browsers can choose to send them in any order they please, and there is no way to tell which one is coming from where ([see Github's notes on the issue](https://github.com/blog/1466-yummy-cookies-across-domains)), so using cookies across domains can be complicated. This prevents complications by 

1. tying cookies explicitly to a domain using the cookie key, and
2. avoiding parsing any cookie that does not use this key.
