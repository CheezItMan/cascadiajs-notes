# Node Can do Quic

@trivikram

Github @trivikr

NodeJS core contributor

What do you call a can opener which doesn't work, a can't opener.




Why http2 is required, and why http3 is required and when is it coming.

http 1.0

- Building extensibility
  - get mypage.html http/1.0
    - User-agent
    - Provides response code

http 1.1

- Standardized protocol
  - too many damm headers
  - Issues:
    - 3 roundtrips per request
      - TCP Sync 
      - TCP syn - Ack
      - TCP Ack
      - TCP Client Hello
      - TLS Server Hello
      - TLS finished
      - HTTP request
      - HTTP response
    - Multiple TCP+ TLS connections created for concurrent requests
      - Request a bunch of stuff at the same time

http 2.0

How it works
- You can request multiple resources in one http request
- Benefits
  - Multiplexing and concurrency (different requests on same connection)
  - Prioritized stuff
  - Compression

Why Http 3?

TCP head-of-line blocking

http3 over quic
- When setting up multiple streams they are treated independently, so if one packet is lost only streams from the same resource gets repeated, rather than all.
- Use UDP instead, and adds TCP congestion control over UDP so that it can stream different resources independently.
- Also reduces roundtrips


What will benefit

- Jasper at 10am will talk about it.
- Self-driving cars
