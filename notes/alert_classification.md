Alert ID: SOC-002
Alert Type: Unauthorized API Access Attempt
Endpoint: /api/Products
HTTP Status Code: 401 Unauthorized
Severity Level: Low
Description:
An unauthenticated request was made to a protected API endpoint.
Access was correctly denied by the server.

Potential Impact:
Repeated attempts may indicate reconnaissance activity.

Recommended Action:
Continue monitoring and ensure proper authentication enforcement.


Alert ID: SOC-002
Alert Type: Public API Endpoint Accessible Without Authentication
Endpoint: /api/Products/<id>/reviews
HTTP Status Code: 200 OK
Severity Level: Medium
Description:
A product reviews API endpoint was accessible without authentication
and returned data successfully.

Potential Impact:
If sensitive or excessive data is exposed, attackers could harvest
information or abuse the endpoint for enumeration or scraping.

Recommended Action:
Review access control requirements, limit exposed data, and implement
rate limiting or authentication if necessary.


Alert ID: SOC-003
Alert Type: User Identity Endpoint Accessed Without Active Session
Endpoint: /rest/user/whoami
HTTP Status Code: 304 Not Modified
Severity Level: Informational
Description:
The user identity endpoint was accessed without an active authenticated
session, resulting in no content being returned.

Potential Impact:
Minimal risk. However, repeated probing of identity endpoints may
indicate reconnaissance behavior.

Recommended Action:
Continue monitoring access attempts and ensure session management
controls are functioning correctly.




