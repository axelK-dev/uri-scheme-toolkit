## 🚀 Start Here

Welcome to the URI Scheme Toolkit! This lightweight, mobile-friendly dashboard is designed to help you:

- Understand how URLs and URI schemes work
- Trigger actions on your phone or browser
- Learn how these concepts connect to cybersecurity and DevOps
- Discover free resources to build your skills

---

## 🎓 Free Learning Resources

These platforms offer free courses and certifications to help you build skills in cybersecurity, DevOps, and more:

- [LinkedIn Learning](https://www.linkedin.com/learning) *(Free with many library cards)*
- [Cisco Networking Academy](https://www.netacad.com/)
- [FreeCodeCamp](https://www.freecodecamp.org/)
- [MIT OpenCourseWare](https://ocw.mit.edu/)
- [Khan Academy](https://www.khanacademy.org/computing)

---
## 🧭 Curiosity Pathways

Choose a path to start exploring:

- **🔐 I want to learn cybersecurity basics**
- **🧰 I want to build tools with Markdown and URI schemes**
- **🌐 I want to understand how the internet works**
- **📱 I want to make my own mobile app**
  
---

URI Building
🌐 What You Might Encounter in a Browser Address Bar
Here’s a breakdown of the types of inputs and what they mean:

| **Type**               | **Example**                                  | **Purpose**                                                                 |
|------------------------|----------------------------------------------|------------------------------------------------------------------------------|
| Domain Name           | `example.com`                               | Human-readable name mapped to an IP address via DNS.                        |
| IP Address            | `192.168.1.1`                               | Direct access to a server or device (often local).                          |
| Protocol              | `https://`, `ftp://`, `ws://`               | Defines how data is transferred (HTTP, FTP, WebSocket).                     |
| Port Number           | `:8080`, `:3306`                            | Specifies a service running on a specific port (e.g., web server, database).|
| Path                  | `/products/item123`                         | Points to a resource or endpoint on the server.                             |
________________________________
🧠 Database Access via URL
While you don’t directly access a database from the browser, you often trigger a backend query via:

REST API endpoints:

https://api.example.com/users?id=42
→ This hits a backend route that queries a database.

GraphQL endpoints:

https://api.example.com/graphql
→ The query is sent in the request body, not the URL.

Web apps with query strings:

https://app.example.com/search?term=books&category=fiction
→ The frontend parses this and sends a request to the backend.
________________________________________
📊 URL Components Table

| **Component**                | **Example**                                      | **Purpose / Notes**                                                                 |
|------------------------------|---------------------------------------------------|--------------------------------------------------------------------------------------|
| Protocol                    | `https://`, `http://`, `ftp://`, `ws://`          | Defines how data is transferred (secure, file, WebSocket, etc.)                     |
| Subdomain                   | `api.example.com`, `db.example.com`               | Often used to separate services (e.g., API, database access)                        |
| Domain Name                 | `example.com`                                     | Human-readable name mapped to an IP address via DNS                                  |
| IP Address                  | `192.168.1.1`, `8.8.8.8`                          | Direct access to a server or device (often used in local or admin access)           |
| Port Number                 | `:80`, `:443`, `:3306`                            | Specifies the service port (e.g., web server, database, custom app)                 |
| Path                        | `/users`, `/products/item123`                     | Points to a resource or endpoint on the server                                       |
| Query String                | `?id=123&sort=asc`                                | Sends parameters to the server (often used in database queries via APIs)            |
| Fragment                    | `#section2`                                       | Refers to a part of the page (handled by the browser, not the server)               |
| Authentication Info         | `user:pass@example.com`                           | Rarely used now; sends credentials in the URL (not secure)                           |
| Encoded Characters          | `%20`, `%2F`                                      | URL encoding for special characters (e.g., spaces, slashes)                          |
| Custom Schemes              | `mailto:`, `tel:`, `geo:`                         | Triggers apps or services (email, phone, maps)                                       |
| Environment Variables (in dev) | `localhost:3000?env=dev`                        | Used in development to simulate different configurations                              |
________________________________________
🧠 For Database Access:

You’ll often see query strings used to pass parameters to backend services that query a database.

The actual database access happens server-side, but the URL can trigger it.
________________________________________
✅ Why Trying Them Out Helps

Hands-on learning: 
You’ll see how query strings affect search results or how paths map to resources.

Debugging intuition: You’ll start to recognize malformed URLs or missing parameters.

Security awareness: You’ll notice how sensitive data should (or shouldn’t) be passed in URLs.

Database interaction: You’ll understand how frontend URLs trigger backend queries.
________________________________________
🧪 Safe Things to Try
Here are some examples you can experiment with:

| **Type**          | **Example to Try**                                | **What It Does**                     |
|--------------------|---------------------------------------------------|---------------------------------------|
| Basic URL          | `https://example.com`                            | Loads homepage                       |
| Path               | `https://example.com/products`                   | Loads product list                   |
| Query String       | `https://example.com/search?q=laptop`            | Searches for "laptop"                |
| Fragment           | `https://example.com/docs#install`               | Jumps to install section             |
| Localhost          | `http://localhost:3000`                          | Access local dev server              |
| IP Address         | `http://192.168.1.1`                             | Access router or local device        |
| Port               | `http://localhost:8080`                          | Access service on custom port        |
| API Endpoint       | `https://api.example.com/users?id=42`            | Triggers backend query               |
| Encoded URL        | `https://example.com/search?q=hello%20world`     | Searches for "hello world"           |

________________________________________
🧭 Tips for Practicing

Use a local development environment (like VS Code + Live Server or Node.js).

Try building a simple HTML page that reads query strings using JavaScript.

Use tools like Postman or Insomnia to test API endpoints safely.

Avoid sending sensitive data in URLs (e.g., passwords, tokens).

The number of combinations and proprietary behaviors tied to URI schemes, browser support, device types, and installed apps can be overwhelming at first. 
________________________________________
🧭 Why It Feels Complex

URI schemes like geo:, mailto:, tel:, sms:, intent: are designed to trigger specific actions.

-Browser behavior varies: 

-Mobile browsers often support more schemes (e.g., geo: opens maps).

-Desktop browsers may ignore or block them unless an app is registered.

Operating systems handle schemes differently: 

-Android uses intent: URIs.

-iOS uses x-apple-maps: or maps:.

Apps register custom schemes: 

-Spotify might use spotify:track:...

-Zoom might use zoommtg://...
________________________________________
📊 Want a Chart?
Here’s a quick table to help organize some common URI schemes:

| **Scheme**      | **Example**                                | **Purpose**           | **Typical Behavior**                     |
|------------------|-------------------------------------------|------------------------|------------------------------------------|
| `http://` / `https://` | `https://example.com`                     | Web page              | Opens in browser                        |
| `mailto:`       | `mailto:someone@example.com`              | Email                 | Opens default mail app                  |
| `tel:`          | `tel:+1234567890`                         | Phone call            | Opens dialer                            |
| `sms:`          | `sms:+1234567890`                         | Text message          | Opens messaging app                     |
| `geo:`          | `geo:37.786971,-122.399677`               | Location              | Opens maps app (mobile)                 |
| `intent:`       | `intent://...`                            | Android app intent    | Opens specific app (Android only)       |
| `file:`         | `file:///C:/path/to/file.txt`             | Local file            | Opens file (if allowed)                 |
| `data:`         | `data:text/html;base64,...`               | Inline content        | Renders directly in browser             |
| `ftp:`          | `ftp://example.com/file.zip`              | File transfer         | Opens FTP client or browser             |
| `custom:`       | `zoommtg://...`                           | App-specific          | Opens registered app                    |

________________________________________
🧪 What You Can Do
Try these schemes in a mobile browser or create simple HTML links to test behavior.
Use developer tools to inspect how query strings and paths are parsed.

Explore custom schemes used by apps you use — they often have docs for integration.

Just like PowerShell, Bash, or any terminal environment, understanding how URI schemes and address bar inputs work gives you real control over systems, apps, and automation.
________________________________________
🧠 Why This Has Terminal-Like Power
1. Direct Invocation of Services
mailto:, tel:, geo:, zoommtg: — these are like commands that launch apps or trigger actions.
You’re not just browsing — you’re activating system-level behaviors.
1. Scriptable and Automatable
These schemes can be embedded in: 
HTML
Markdown
Terminal scripts
PowerShell or Bash commands
You can use them to automate workflows, like opening meetings, sending emails, or launching maps.
1. Cross-Platform Integration
URI schemes are a universal language across mobile, desktop, and web.
They’re used in: 
App development
Web automation
DevOps pipelines
Security testing (e.g., phishing simulations, URI fuzzing)
1. Security and Networking Insight
Understanding how URLs and schemes work helps you: 
Spot malicious links
Understand redirects and query strings
Debug API calls and webhooks
Trace how frontend inputs trigger backend database queries
________________________________________
🔧 Terminal-Like Use Cases

| **Use Case**        | **Tool or Context**      | **Example**                                      |
|----------------------|---------------------------|---------------------------------------------------|
| Launch Zoom          | PowerShell / HTML        | `Start-Process "zoommtg://..."`                  |
| Open Maps            | Bash / HTML              | `xdg-open "geo:..."`                              |
| Trigger API          | Curl / Postman           | `curl "https://api.example.com/users?id=42"`      |
| Send Email           | HTML / Markdown          | `Email Me`                                       |
| Open Local File      | Terminal / Browser       | `file:///C:/docs/report.pdf`                     |

________________________________________
🧭 Bottom Line
Learning this well is worth it, even if it seems complex at first. It’s part of the same ecosystem of command-line power, web automation, and system integration that makes PowerShell and Bash so valuable.

A command that ties together:
URI schemes (like mailto:, geo:, zoommtg:)
Terminal equivalents (PowerShell, Bash, etc.)
Web automation use cases
Platform-specific behaviors
________________________________________
🧭 URI Scheme + Terminal Command Cheat Sheet

| **Action**           | **URI Scheme**                              | **PowerShell**                                   | **Bash / Linux**                               | **Web Automation Use**       | **Platform Notes**                |
|----------------------|--------------------------------------------|-------------------------------------------------|-----------------------------------------------|--------------------------------|------------------------------------|
| Open website         | `https://example.com`                     | `Start-Process "https://example.com"`           | `xdg-open https://example.com`               | `...`                          | Universal                          |
| Send email           | `mailto:user@example.com`                 | `Start-Process "mailto:user@example.com"`       | `xdg-open "mailto:user@example.com"`         | `mailto:...`                   | Opens default mail app            |
| Call phone           | `tel:+1234567890`                         | `Start-Process "tel:+1234567890"`               | `xdg-open "tel:+1234567890"`                 | `tel:...`                       | Mobile only                       |
| Text message         | `sms:+1234567890`                         | `Start-Process "sms:+1234567890"`               | `xdg-open "sms:+1234567890"`                 | `sms:...`                       | Mobile only                       |
| Open map             | `geo:37.7749,-122.4194`                   | `Start-Process "geo:37.7749,-122.4194"`         | `xdg-open "geo:..."`                         | `geo:...`                       | Mobile preferred                   |
| Join Zoom            | `zoommtg://zoom.us/join?...`              | `Start-Process "zoommtg://..."`                 | `xdg-open "zoommtg://..."`                   | `zoommtg://...`                 | Requires Zoom installed            |
| Open file            | `file:///C:/docs/file.txt`                | `Start-Process "file:///C:/docs/file.txt"`      | `xdg-open file:///home/user/file.txt`        | `file:///...`                    | Local only                         |

________________________________________
🧪 How This Helps
You can test URI schemes in HTML, Markdown, or terminal.

You’ll understand how apps and services integrate across platforms.

You’ll be able to automate workflows using links, scripts, or web triggers.

URI schemes offer a kind of shortcut power that’s especially useful when working from a browser or mobile device, where you don’t have access to a full terminal or shell.
________________________________________
🧠 Why URI Schemes Are Powerful (Like Terminal Commands)

✅ 1. Compact and Direct
URI schemes are short and expressive — like terminal commands.
Example: 
mailto:someone@example.com → opens email
geo:37.7749,-122.4194 → opens maps
zoommtg://... → joins a meeting

✅ 2. No Terminal Needed
You can trigger actions without a command line.
Especially useful on phones, tablets, or locked-down systems.

✅ 3. Cross-Platform Behavior
URI schemes work across: 
Web browsers
Mobile apps
Desktop environments
They’re like universal triggers for system-level actions.

✅ 4. Automation-Friendly
You can embed them in: 
HTML links
Markdown files
QR codes
Email templates
They’re great for low-code automation and user-friendly scripting.
________________________________________
🔁 Terminal vs. URI Scheme (Side-by-Side)
Action	Terminal Command	URI Scheme	Where It Works
Open website	curl https://example.com	https://example.com	Browser, terminal
Send email	mail someone@example.com	mailto:someone@example.com	Browser, apps
Open map	xdg-open "geo:..."	geo:37.7749,-122.4194	Mobile, browser
Join Zoom	Start-Process "zoommtg://..."	zoommtg://...	Desktop, mobile
Call phone	telnet or VoIP tools	tel:+1234567890	Mobile, browser
________________________________________
Full path from code to webpage, including how it interacts with each layer of the IP stack and other key systems:
________________________________________
🛠️ 1. Code Creation
Frontend Code: HTML, CSS, JavaScript — defines structure, style, and behavior.
Backend Code: Python, Node.js, C#, etc. — handles logic, data, and APIs.
Database Queries: SQL, NoSQL — fetches and stores data.
________________________________________
🧪 2. Build & Test (CI/CD Pipeline)
Linting & Unit Tests: Ensures code quality.
Build Tools: Webpack, Babel, etc. compile and bundle code.
Security Scans: Check for vulnerabilities.
Artifact Creation: Generates deployable packages (e.g., Docker images).
________________________________________
🚀 3. Deployment
CI/CD Tools: GitHub Actions, Azure DevOps, Jenkins.
Infrastructure as Code: Terraform, ARM templates.
Cloud Hosting: Azure App Service, Azure Kubernetes Service (AKS), etc.
________________________________________
🌐 4. DNS Resolution (Application Layer)
User enters URL → Browser sends DNS query.
DNS Server returns IP address of the web server.
________________________________________
📡 5. TCP/IP Stack Interaction
🔹 Application Layer (HTTP/HTTPS)
Browser sends HTTP request to server.
Server responds with HTML, CSS, JS, or JSON.
🔹 Transport Layer (TCP)
TCP ensures reliable delivery of packets.
Handshake: SYN → SYN-ACK → ACK.
🔹 Network Layer (IP)
IP routes packets across networks.
Handles addressing and fragmentation.
🔹 Data Link Layer
Ethernet/Wi-Fi frames transmit data between devices on the same network.
🔹 Physical Layer
Electrical signals or radio waves carry bits across cables or air.
________________________________________
🖥️ 6. Web Server Response
Web Server (e.g., Nginx, IIS, Apache) receives request.
Backend App processes logic, queries database, returns response.
Static Files (HTML, CSS, JS) are served directly.
________________________________________
🧠 7. Browser Rendering
Parses HTML → Builds DOM.
Applies CSS → Paints layout.
Executes JS → Adds interactivity.
May make additional API calls (AJAX, fetch).
________________________________________
🔁 8. User Interaction
Clicking, typing, scrolling → Triggers frontend logic.
May send new requests → Repeats the stack cycle.

```mermaid
graph TD
A[Code Written 🧑‍💻] --> B[Build & Test 🔧]
B --> C[CI/CD Pipeline 🚀]
C --> D[Deployment to Server 🖥️]
D --> E[DNS Resolution 🌐]
E --> F[IP Stack Interaction 📡]
F --> G[Web Server Receives Request 🧠]
G --> H[Backend Logic & Database Query 🗄️]
H --> I[Response Sent to Browser 📦]
I --> J[Browser Renders Page 🖥️]
J --> K[User Interacts 🔁]

%% IP Stack Layers as separate nodes
F --> F1[Application Layer (HTTP/HTTPS)]
F1 --> F2[Transport Layer (TCP)]
F2 --> F3[Network Layer (IP)]
F3 --> F4[Data Link Layer (Ethernet/Wi-Fi)]
F4 --> F5[Physical Layer (Cables/Wireless)]
________________________________________
🧭 Bottom Line
Learning URI schemes is worth it, especially if you're working in environments where terminal access is limited. They give you command-like power in a browser-native way.
A project that lets you explore URI schemes interactively — maybe a simple HTML dashboard that triggers different actions using URI links?
Here’s a starter HTML dashboard that uses URI schemes to trigger actions. You can open this in any browser or edit it in VS Code to experiment:
________________________________________
📄 HTML Dashboard with URI Scheme Actions

<!DOCTYPE html>
<html lang="en">
<head>
<meta charset="UTF-8">
<title>URI Scheme Dashboard</title>
<style>
body {
font-family: sans-serif;
padding: 2em;
background: #f4f4f4;
}
h1 {
color: #333;
}
.link-box {
margin: 1em 0;
}
a {
display: inline-block;
padding: 0.5em 1em;
background: #0078D4;
color: white;
text-decoration: none;
border-radius: 5px;
}
a:hover {
background: #005a9e;
}
</style>
</head>
<body>
<h1>📡 URI Scheme Dashboard</h1>

<div class="link-box">
<a href="mailto:someonecomSend Email</a>
</div>

<div class="link-box">
<el:+1234567890Call Phone</a>
</div>

<div class="link-box">
sms:+1234567890Send SMS</a>
</div>

<div class="link-box">
<a href="geo:122.4194Open Map (San Francisco)</a>
</div>

<div class="link-box">
<a href="zoommtg://zoom.us/join?confno=123d=abcdefJoin Zoom Meeting</a>
</div>

<div class="link-box">
<a href="https://www.google.comoffee+shops+near+meSearch Coffee Shops</a>
</div>

<div class="link-box">
<a href="file:///C:/Users/YourName/Documents/exampleLocal File</a>
</div>
</body>
</html>
________________________________________
🧪 How to Use It
Save it as dashboard.html.
Open it in your browser.
Click the buttons to trigger actions — depending on your device and installed apps.
<!DOCTYPE html>
<html lang="en">
<head>
  <meta charset="UTF-8">
  <title>URI Scheme Dashboard</title>
  <style>
    body {
      font-family: sans-serif;
      padding: 2em;
      background: #f4f4f4;
    }
    h1 {
      color: #333;
    }
    .link-box {
      margin: 1em 0;
    }
    a {
      display: inline-block;
      padding: 0.5em 1em;
      background: #0078D4;
      color: white;
      text-decoration: none;
      border-radius: 5px;
      font-weight: bold;
    }
    a:hover {
      background: #005a9e;
    }
  </style>
</head>
<body>
  <h1>📡 URI Scheme Dashboard</h1>

  <div class="link-box">
    <a href="mailto:someone@examplend Email</a>
  </div>

  <div class="link-box">
    <al:+1234567890📞 Call Phone</a>
  </div>

  <div class="link-box">
    <a href="sms890💬 Send SMS</a>
  </div>

  <div class="link-box">
    <a href="geo:37.77494🗺
A prototype of something that could evolve into:
A mobile productivity app
A caregiver support tool
A custom launcher for URI-based actions
Even a low-code/no-code platform for non-tech users
🚀 Pathways to Turn This Into an Android App Today
Here are a few options you can explore right now:
1. Use WebView in Android Studio
You can wrap your HTML dashboard in a simple Android app using WebView:
Install Android Studio
Create a new project
Load your dashboard.html into a WebView
Package and test it on your phone

1. Use Progressive Web App (PWA) Features
Turn your dashboard into a PWA:

Add a manifest file
Enable service workers
Users can “install” it from their browser like an app
This works great for Android and doesn’t require publishing to the Play Store.
1. Use Tools Like Cordova or Capacitor
These let you wrap web code into native apps:
Apache Cordova (older but still useful)
Capacitor (modern, works with frameworks like Vue or React)
________________________________________
💼 Career Paths Where This Skill Pays Off
Here are roles where you could thrive:

| **Role**                          | **What You’d Do**                                      |
|-----------------------------------|---------------------------------------------------------|
| Frontend Developer               | Build user interfaces like this dashboard              |
| Mobile App Developer             | Turn HTML prototypes into Android/iOS apps            |
| UX Engineer                      | Focus on usability and accessibility                   |
| Technical Product Designer       | Combine design and code to build tools people love     |
| Startup Founder or Indie Hacker  | Build and sell your own tools — even small ones can earn! |
