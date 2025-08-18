### Definition

- The **`.well-known`** standard (RFC 8615) defines a **standardized directory** located at:
    
    `https://example.com/.well-known/`
    
- Purpose: Stores **metadata, configurations, and security-related files** in a **centralized and predictable location**.
    
- Maintained by: **IANA** (Internet Assigned Numbers Authority).
    

---

### 📖 Why Important?

- Provides **consistent access** for:
    
    - Browsers
        
    - Applications
        
    - Security tools
        
- Helps in **automatic discovery** of security policies, authentication configs, and service metadata.
    

---

### 🔑 Common Examples (IANA Registry)

|URI Suffix|Purpose|Status|Reference|
|---|---|---|---|
|`security.txt`|Contact info for reporting vulnerabilities|Permanent|RFC 9116|
|`change-password`|Standard URL for password change page|Provisional|[Spec](https://w3c.github.io/webappsec-change-password-url/#the-change-password-well-known-uri)|
|`openid-configuration`|OpenID Connect metadata & endpoints|Permanent|[OpenID Spec](http://openid.net/specs/openid-connect-discovery-1_0.html)|
|`assetlinks.json`|Verifies ownership of apps/domains|Permanent|[Google Spec](https://github.com/google/digitalassetlinks/blob/master/well-known/specification.md)|
|`mta-sts.txt`|SMTP MTA-STS policy for email security|Permanent|RFC 8461|

---

### 🛡️ Web Recon & Pentesting Usage

During **web reconnaissance**, `.well-known` paths can leak **critical configuration details**.

#### Example: `openid-configuration`

- Path:
    
    `https://example.com/.well-known/openid-configuration`
    
- Returns **JSON metadata** about OpenID Connect & OAuth 2.0 provider.
    

**Sample JSON Output:**

`{   "issuer": "https://example.com",   "authorization_endpoint": "https://example.com/oauth2/authorize",   "token_endpoint": "https://example.com/oauth2/token",   "userinfo_endpoint": "https://example.com/oauth2/userinfo",   "jwks_uri": "https://example.com/oauth2/jwks",   "response_types_supported": ["code", "token", "id_token"],   "scopes_supported": ["openid", "profile", "email"] }`

#### Security Insights:

- **Authorization endpoint** → Entry point for authentication requests.
    
- **Token endpoint** → Location where tokens are issued.
    
- **Userinfo endpoint** → API to fetch user details.
    
- **JWKS URI** → Public cryptographic keys used for JWT verification.
    
- **Supported scopes & response types** → Helps in understanding allowed permissions.
    
- **Algorithms supported** → Reveals crypto details (e.g., `RS256`).