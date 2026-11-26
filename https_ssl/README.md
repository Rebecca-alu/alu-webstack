# HTTPS SSL

This project sets up HTTPS for my website using HAProxy on my load balancer (lb-01).

## Files
- `0-world_wide_web` - Bash script that shows the DNS record type and IP of the subdomains www, lb-01, web-01 and web-02
- `1-haproxy_ssl_termination` - HAProxy config that accepts HTTPS on port 443 and passes the traffic to web-01 and web-02
- `2-redirect_http_to_https` - HAProxy config that also redirects HTTP to HTTPS with a 301
