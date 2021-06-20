# Read 11: Authentication:

## What is OAuth:

**What is OAuth?**

- A protocol allows authenticated access to their assets without sharing their passwords. Instead of share the users their passwords, this protocol works like an agent between the users and their information. In authentication parlance, this is known as secure, third-party, user-agent, delegated authorization.

**Give an example of what using OAuth would look like.**

- When you for example, log onto any website that offers the opportuinty to log using another website, like, Netlify and Heroku logging onti using GitHub.

**How does OAuth work? What are the steps that it takes to authenticate the user?**

- The first website connects to the second website on behalf of the user, using OAuth, providing the user’s verified identity.

- The second site generates a one-time token and a one-time secret unique to the transaction and parties involved.

- The first site gives this token and secret to the initiating user’s client software.

- The client’s software presents the request token and secret to their authorization provider (which may or may not be the second site).

- If not already authenticated to the authorization provider, the client may be asked to authenticate. After authentication, the client is asked to approve the authorization transaction to the second website.

- The user approves (or their software silently approves) a particular transaction type at the first website.

- The user is given an approved access token (notice it’s no longer a request token).

- The user gives the approved access token to the first website.

- The first website gives the access token to the second website as proof of authentication on behalf of the user.

- The second website lets the first website access their site on behalf of the user.

- The user sees a successfully completed transaction occurring.

**What is OpenID?**

- It is security technologies for humans logging into machines.

---------------------------------------------------------------------

## Authorization and Authentication flows:

**What is the difference between authorization and authentication?**

- Authentication is the process of verifying who a user is, while authorization is the process of verifying what they have access to.

**What is Authorization Code Flow?**

- Regular web apps are server-side apps where the source code is not publicly exposed, they can use the Authorization Code Flow ,which exchanges an Authorization Code for a token.

**What is Authorization Code Flow with Proof Key for Code Exchange (PKCE)?**

- Public clients (e.g., native and single-page applications) request Access Tokens, some additional security concerns are posed that are not mitigated by the Authorization Code Flow alone.

**What is Implicit Flow with Form Post?**

- Intended for Public Clients, or applications which are unable to securely store Client Secrets.

**What is Client Credentials Flow?**

- With machine-to-machine (M2M) applications, such as CLIs, daemons, or services running on your back-end, the system authenticates and authorizes the app rather than a user.

**What is Device Authorization Flow?**

- Input-constrained devices that connect to the internet, rather than authenticate the user directly, the device asks the user to go to a link on their computer or smartphone and authorize the device.

**What is Resource Owner Password Flow?**

- Though we do not recommend it, highly-trusted applications can use the Resource Owner Password Flow, which requests that users provide credentials (username and password), typically using an interactive form.

---------------------------------------------------------------------

### Things I want to know more about:

- About authintication and authorization.
- About OpenID protocol and Auth2.
