# Policy Service Endpoints
Unlike the queries at the root level of this repository, these queries use:
`https://api.cloud.ox.security/api/policy-service` as their endpoint.
Additionally, for authorization they use the [Bearer Token](#getting-your-ox-token) presented by your
logged-in OX Dashboard. 

##### Getting your OX Token

Login to the [OX Dashboard](https://app.ox.security) and bring up your browser's
Developer Tools (usually `ctrl-shift-I` or `cmd-opt-I` depending on your
platform).

From there, go to the "Network" tab and filter the traffic for
`api.cloud.ox.security` (refresh the page if necessary) and from the Request
Headers, pull the Authorization Bearer Token (it'll start with "ey", base64
encoding for "{" which all JWTs start with).
